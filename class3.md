## why this topic matters as it relates to what you are studying in this module?
# understanding how paython performs file input/output and the different modes for opening afile and different kinds of file content 

# How python performs file input/output

# Python provides several ways to perform file input/output operations. The two main approaches are:

# File Object Method
# In this approach, you first open the file using the built-in open() function. The open() function takes two arguments: the first argument is the file name, and the second argument is the mode in which you want to open the file (read, write, or append).

# Once you have opened the file, you can perform different operations such as reading, writing, or appending to the file using various methods such as read(), write(), and append().

# With Statement
# In the With Statement approach, you use the with statement to open the file, and the file is automatically closed when the block of code inside the with statement is executed. This approach is safer because it ensures that the file is always closed, even if an error occurs.

# Different modes for opening a file
# Python provides several modes for opening a file, depending on what kind of operations you want to perform on the file. The modes are specified as a string argument to the built-in open() function, as the second parameter. Here are the most commonly used modes:

# 'r': Read mode. This is the default mode. It opens the file for reading only. You can read the contents of the file but cannot modify it.

# 'w': Write mode. This mode opens the file for writing only. It overwrites the file if it already exists or creates a new file if it doesn't exist.

# 'a': Append mode. This mode opens the file for writing, but appends the new content at the end of the existing file. If the file does not exist, it creates a new file.

# 'x': Exclusive creation mode. This mode creates a new file, but if the file already exists, it raises a FileExistsError exception.

# 'b': Binary mode. This mode is used for working with binary data, such as images or sound files.

# 't': Text mode. This mode is used for working with text files, and it is the default mode.

# '+': Read and write mode. This mode allows you to read and write to a file. It is mostly used with text files.

# You can also combine modes by using them together as a single string. For example, 'rb' would open the file in binary read mode, while 'w+' would open the file in read and write mode, overwriting the file if it already exists or creating a new file if it doesn't.

# It is important to note that when you are done working with a file, you should close it using the close() method. This will ensure that any changes made to the file are saved, and that the file is released from memory.


# Different kinds of file content, binary or text



## Things I want to know more about
# Handling exceptions
# Raising exceptions
# Testing exceptions