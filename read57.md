#  Reading 22: Django Forms: 

        An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server

# Declaring a Form: 
The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types (and some similar parameters). This makes sense because in both cases we need to ensure that each field handles the right types of data, is constrained to valid data, and has a description for display/documentation.

# URL configuration
We can name our captured URL data "pk" anything we like, because we have complete control over the view function (we're not using a generic detail view class that expects parameters with a certain name). However, pk short for "primary key", is a reasonable convention to use!



        urlpatterns += [
        path('book/<uuid:pk>/renew/', views.renew_book_librarian, name='renew-book-librarian'),
        ]

# View
The view has to render the default form when it is first called and then either re-render it with error messages if the data is invalid, or process the data and redirect to a new page if the data is valid. In order to perform these different actions, the view has to be able to know whether it is being called for the first time to render the default form, or a subsequent time to validate data. 

# Example Code!

        import datetime

        from django.shortcuts import render, get_object_or_404
        from django.http import HttpResponseRedirect
        from django.urls import reverse

        from catalog.forms import RenewBookForm

        def renew_book_librarian(request, pk):
        book_instance = get_object_or_404(BookInstance, pk=pk)

        # If this is a POST request then process the Form data
        if request.method == 'POST':

                # Create a form instance and populate it with data from the request (binding):
                form = RenewBookForm(request.POST)

                # Check if the form is valid:
                if form.is_valid():
                # process the data in form.cleaned_data as required (here we just write it to the model due_back field)
                book_instance.due_back = form.cleaned_data['renewal_date']
                book_instance.save()

                # redirect to a new URL:
                return HttpResponseRedirect(reverse('all-borrowed') )

        # If this is a GET (or any other method) create the default form.
        else:
                proposed_renewal_date = datetime.date.today() + datetime.timedelta(weeks=3)
                form = RenewBookForm(initial={'renewal_date': proposed_renewal_date})

        context = {
                'form': form,
                'book_instance': book_instance,
        }

        return render(request, 'catalog/book_renew_librarian.html', context)