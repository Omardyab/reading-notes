# Reading 11: Numpy & JupyterLab

## NumPy Tutorial: Data Analysis with Python

Numpy is a commonly used data analysis package
data is ssv(semicolon separated values) format
read the data (as the author described)
an example was shown to get the mean: 

        qualities =
        [float(item[-1]) for item in wines[1:]]
        sum(qualities) / len(qualities)

## Numpy 2-Dimensional Arrays
is a matrix,with rows and columns.

the author shows how to create A NumPy Array: 
- Import the numpy package.
- Pass the list of lists wines into the array function, which converts it into a NumPy array.
- Exclude the header row with list slicing.
- Specify the keyword argument dtype to make sure each element is converted to a float. We’ll dive more into what the dtype is later on.

        import csv
        with open("winequality-red.csv", 'r') as f:
        wines = list(csv.reader(f, delimiter=";"))
        import numpy as np
        wines = np.array(wines[1:], dtype=np.float)

other methods : 

        import numpy as np
        empty_array = np.zeros((3,4))
        empty_array

### Using NumPy To Read In Files: 
* Use the genfromtxt function to read in the winequality-red.csv file.
* Specify the keyword argument delimiter=";" so that the fields are parsed properly.
* Specify the keyword argument skip_header=1 so that the header row is skipped.
        
        wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)

the author also mentioned alot of functionality including 
* Indexing NumPy Arrays
* Slicing NumPy Arrays
* Assigning Values To NumPy Arrays

recheck : [link](https://www.dataquest.io/blog/numpy-tutorial-python/)
## JupyterLab

Work with documents and activities such as Jupyter notebooks, text editors, etc in a flexible manner. 

the video is about using JupyterLab
terminals support linux and powershell

image formats are also supported.
* - = to zoom in and out
* [ ] to rotate 
* 0 to reset

json files can be edited

jupyter notebook are new ways to work togother with data and code seamlessly together Jupiter has two modes when a notebook opens you're in command mode which is designed for easily navigating and changing the framework. 

some commands:

        adding a cell above with a
        adding a cell below with b
        c for copy 
        v for paste
        x is for cut
        delete with dd
        z to under
        shift+z redo
        y to change cell format to code
        m to change cell format to markdown
 
M=edit mode
shift + enter run cell 

whatever we use in markdown is applicable as well. 

        *italic*
        **bold**
        - unorderlist 
        1. orderd list
        > for blackquote
        --- horizental line
        `inline code`
        ''' 
        block of code
        '''
        equation sby framing with dollarsign 
        $ x^2 
        typing with url will make it a link 
        www.xyz.com
        or 
        [link](www.xyz.com)

Y to change mode to code: 
 
        x=1
        print(x)
        shift +enter to run it and 1 will be shown
        0 0 to reset 


        



