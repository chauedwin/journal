# Journal using C++ (PIC10C Project)

__Big Picture__
* going to start with a simple console project (can implement GUI using QT in future)
* originally wanted to connect this project with a SQL database, but attempting to use the sqlapi++ libraries proved to be too complicated
  * after downloading the library and reading the documentation, I realized the code wouldn't compile due to issues with linking the correct library files
  * after attempts at debugging, I concluded the issues were out of the scope of this class and decided to use streams instead. 
* will instead store information in files(which will be located in the project directory), future improvements can be made to improve security

__Update 1__
* Outlined a super basic Journal class
  * depends on an Entry class of some sort for now
* Ideas for implementation
  * Journal class to allow changes to "GUI" details
    * These details will be preserved for future uses
    * Save details in a file, which will be accessed and used to create the Journal object before starting app
  * Entry class to write or read entries?
    * Might not need the extra level of organization 
    * regular functions in the main may suffice, and can implement template functions or other tricks that way
    

__References used__
* SQLAPI+ documentation
  * http://www.sqlapi.com/
* Some issues with using SQLAPI+
  * checking error lnk2019
    * https://stackoverflow.com/questions/19886397/how-to-solve-the-error-lnk2019-unresolved-external-symbol-function/46673248
  * attempts to link library files
    * https://social.msdn.microsoft.com/Forums/vstudio/en-US/aa91d7f7-cc79-4b48-b852-94f7f1bd964a/how-use-install-the-sqlapi-library?forum=vcgeneral
* reading a file using delimiters
  * http://www.cplusplus.com/forum/beginner/113465/
