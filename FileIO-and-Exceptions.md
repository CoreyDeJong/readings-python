## Reading and Writing Files in Python
 - `file = open('dog_breeds.txt')` to open a file
 - `file.close()` to close a file
  - `with open('dog_breeds.txt') as file :` will automatically close the file, even if an error occurs
 - `python3 reading.py` will execute the reading.py file in you terminal
 - `content = file.readlines(10)` will read 10 characters from the file
 - `This is the first line\r\n` the extra `\r` is needed for windows users
 - writelines allow multiple strings to be committed to an open file
 - append using `a` 
    - `with open('dog_breeds.txt', 'a') as a_writer:a_writer.write('\nBeagle')`
 - `os.path.join` for creating paths for either mac or windows
 - A file with have 3 sections, header(metadata,...), content(what we see/create/destroy!) and end of file(special character that endicates it is the end of the file)

## Exceptions in Python
 - exception means you have correct syntax
 - `raise Exception(f'a;djfkajs;dkfl)` will be similar to a console.log show the `Exception(f'fakdfj;alskdf)` statement when the code is targeted
 - try: the code that is attempting to run
 - except: this code if there is an exception
 - else: this code if there is no exceptions that have occurred
 - finally: this code is always run 