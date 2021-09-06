#  Reading 24: Permissions:

- Permissions determine whether a request should be granted or denied access.
- Use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.
- used to grant or deny access for different classes of users to different parts of the API.
- Allow access to any authenticated user, and deny access to any unauthenticated user. This corresponds to the IsAuthenticated class in REST framework.
- Or full access to authenticated users, but allow read-only access to unauthenticated user using IsAuthenticatedOrReadOnly.
- If any permission check fails an exceptions an exception will be raised.
- REST framework permissions also support object-level permissioning.

## Setting the permission policy:


        REST_FRAMEWORK = {
        'DEFAULT_PERMISSION_CLASSES': [
                'rest_framework.permissions.IsAuthenticated',
        ]
        }


## API Reference:

        AllowAny=> AllowAny :allow unrestricted access

        IsAuthenticated=> IsAuthenticated: deny permission to any unauthenticated user.

        IsAdminUser=> IsAdminUser: user.is_staff is True in which case permission will be allowed.

## DjangoModelPermissions: 

        POST requests require the user to have the add permission on the model.

        PUT and PATCH requests require the user to have the change permission on the model.

        DELETE requests require the user to have the delete permission on the model.
