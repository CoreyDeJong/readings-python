## Python Regular Expression
 - Regular expressions are used to identify whether a pattern exists in a given sequence of characters (string) or not
 - regex is used for manipulating textual data, which is often a pre-requisite for data science projects that involve text mining.
 - The match() function returns a match object if the text matches the pattern. Otherwise it returns None.
 - repitions checks for multiple occurrences
 - When a special character matches as much of the search sequence (string) as possible, it is said to be a "Greedy Match"
 - the search() function checks for a match anywhere in the string.
 - When you need to use an expression several times in a single program, using the compile() function to save the resulting regular expression object for reuse is more efficient. 

 ## Shutil
  - The shutil module includes high-level file operations such as copying and archiving
  - `import shutil`
  - `shutil.copytree(src=source_folder_name_here, dst=destination_folder_name_here)