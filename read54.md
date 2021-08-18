# Reading 19:Automation

Regex or Regular Expressions:sequence of characters used to check whether a pattern exists in a given text or not.
import re to be able to use it. 

|Special Characters | Match                 |
|-----------|-------------------------------|
|Period .   | Single character except the newline |
|caret ^| The start of the string|
|$ |The end of string|
|[abc] | a or b or c|
|[a-zA-Z0-9]|Any letter from (a to z) or (A to Z) or (0 to 9)|
|\ | Backslash|
|\w Lowercase 'w'| Matches any single letter, digit, or underscore|
|\W Uppercase 'W'|Matches any character not part of \w (lowercase w)|
|\s - Lowercase 's'|single whitespace character like: space, newline, tab, return|
|\S - Uppercase 'S'| Any character not part of \s (lowercase s)|
|\d - Lowercase d| decimal digit 0-9.|
|\D - Uppercase d| Any character that is not a decimal digit|
|\t - Lowercase t| Tab|
|\n - Lowercase n| Newline|
|\r - Lowercase r| Return|
|\A - Uppercase a| Only at the start of the string and it work across multiple lines as well|
|\Z - Uppercase z| at the end of the string|
|\b - Lowercase b| only the beginning or end of the word|


|Repetitions | Checks if               |
|-----------|-------------------------------|
|+ | The character appears one or more times starting from that position|
| *| The character appears zero or more times starting from that position.
| ? | The character appears exactly zero or one time starting from that position|
|{x} |Repeat exactly x number of times|
|{x,} |Repeat at least x times or more|
|{x, y}| Repeat at least x times but no more than y times|


# shutil — High-level File Operations :Copy and archive files 

    
    import glob
    import shutil

    print('BEFORE:', glob.glob('shutil_copyfile.*'))

    shutil.copyfile('shutil_copyfile.py', 'shutil_copyfile.py.copy')

    print('AFTER:', glob.glob('shutil_copyfile.*'))

    $ python3 shutil_copyfile.py

    BEFORE: ['shutil_copyfile.py']
    AFTER: ['shutil_copyfile.py', 'shutil_copyfile.py.copy']


refer to this to check the codes :https://pymotw.com/3/shutil/ 