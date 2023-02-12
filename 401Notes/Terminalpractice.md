Basic Navigation

  pwd - print working directory - Shows you where you currently are
  ls - lists everything within your current location
  [] items mean they are optional arguments but are not required to run the command
  -l indicates we are going to do a long listing which includes:
    First character indicates whether it is a normal file ( - ) or directory ( d )
    Next 9 characters are permissions for the file or directory.
    The next field is the number of blocks.
    The next field is the owner of the file or directory.
    The next field is the group the file or directory belongs to. 
    Following this is the file size.
    Next up is the file modification time.
    Finally we have the actual name of the file or directory.

  Paths - absolute and relative - The means to get to a certain file or directory in the system.
    Absolute: Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )

    Relative: Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.
  
  cd - stands for change directory

  Tab Completion - When you begin to type a command, you can hit tab and it will autofill the rest of the command for you. If nothing happens, it means there's multiple options and you need to hit tab again to go through them.

  Linux is..
     extensionless -> Using file[path] allows us to determine what the file type is.
     case sensitive
    
 Spaces -> valid but must be careful with them so that we are not causing one item to look like two separate commands
    
 Quotes -> anything inside quotes is considered a single item. Quotes are beneficial to signify a single item with spaces between it.
    
 Escape characters -> \ escapes (or nulifies) the special meaning of the next character

 " -a " shows hidden files and directories

 Manual Pages

 "The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept"

To access..
 man<command to look up> 
 To look up key words..
  man -k <search term>

Making a Directory

  mkdir [options] <Directory>
    -p tells mkdir to make parent directories as needed
    -v makes mkdir tell us what it is doing

Removing a Directory
  rmdir [options] <Directory>

Creating a blank file
  touch [options] <filename>

Copying a file or directory
  cp [options] <source> <destination>
  "Using the -r option, which stands for recursive, we may copy directories. Recursive means that we want to look at a directory and all files and directories within it, and for subdirectories, go into them and do the same thing and keep doing this"

Moving a file or directory
  mv [options] <source> <destination>
  Can also be used to rename a file or directory in the process of moving it

Removing a file or non empty direcories
  rm [options]<file>

TO NOTE ..
  "whenever we refer to a file or directory on the command line it is in fact a path. As such it may be specified as either an absolute or relative path. This is pretty much always the case so remember this important point."

Source: https://ryanstutorials.net/linuxtutorial/
