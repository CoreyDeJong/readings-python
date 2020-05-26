## Data Science in a Nutshell
- Unstructured Data: It does not have a predefined data model. It can be available in audio, video and text format.
- Structured Data: It is mostly available in a text format which originates from databases or specific file formats like CSV (Comma Separated Values
- machine learning is when patterns are identified in data by machine
- Artificial Intelligence is then when the machine will make decisions on the patterns of the data


## What is Jupyter Lab
- JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.
- JupyterLab also offers a unified model for viewing and handling data formats. JupyterLab understands many file formats (images, CSV, JSON, Markdown, PDF, Vega, Vega-Lite, etc.)
- runs python 3


## Numpy Tutorial
 - NumPy is a commonly used Python data analysis package
 - uses multidimensional arrays
 - We can create a NumPy array using the `numpy.array` function
 - column/row selection = NumPy is zero-indexed, meaning that the index of the first row is 0, and the index of the first column is 0. If we want to work with the fourth row, we’d use index 3, if we want to work with the second row, we’d use index 1, and so on.
 - slice = If we instead want to select the first three items from the fourth column, we can do it using a colon (:). A colon indicates that we want to select all the elements from the starting index up to but not including the ending index.
 - Assigning values = `wines[1,5] = 10`
 - Broadcasting = Unless the arrays that you’re operating on are the exact same size, it’s not possible to do elementwise operations. In cases like this, NumPy performs broadcasting to try to match up elements.