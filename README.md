# NASTRAN95 documentation

This is the updated Nastran 95 documentation using the markdown language.

## Installation

Copy the files to an environment that has gfortran (GNU Fortran compiler) and make installed. We did this on the Ubuntu platform.

Obtain the files from github using:

```shell
>>> git clone https://github.com/Interster/NASTRAN95.git
```

Run the following commands in Linux in order to compile the source code

```shell
>>> chmod 744 bootstrap
>>> chmod 744 configure
>>> sudo ./bootstrap
>>> sudo make all
```



In order to compile Nastran 95 on Windows, a project needs to be created in an editor such as Codeblocks.  This is more specialized and will not be covered in this manual.



**How to RUN A nastran 95 PROBLEM**

The NASTRAN 95 program uses *.inp files instead of *.BDF files 

Put the *.inp file in the 

NASTRANinstalldirectory/test directory

Then run the testrunner script.

Example:

```shell
>>>./testrunner beam.inp 
```



runs a problem named "beam" 

**How to RUN A nastran 95 PROBLEM in windows**

Declare the nasthome variable first:

*set nasthome=c:\NASTRAN* 

This is best done using the "environment variables from the start menu"

The open up a console in the Nastran install directory (for example c:\NASTRAN)

Now run the “beam.inp” file in the “test” directory, but using the following command:

```shell
>>>nastran.bat ..\test\beam 
```

 runs a problem named "beam.inp"

Note not to add the *.inp extension in the Windows command as this will cause errors.