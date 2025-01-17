#core Flight System (cFS) Memory Manager Application (MM)

## Introduction

The Memory Manager application (MM) is a core Flight System (cFS) application 
that is a plug in to the Core Flight Executive (cFE) component of the cFS.  
  
The MM application is used for the loading and dumping system memory. MM 
provides an operator interface to the memory manipulation functions contained
in the PSP (Platform Support Package) and OSAL (Operating System Abstraction 
Layer) components of the cFS. MM provides the ability to load and dump memory 
via command parameters, as well as, from files. If the operating system 
supports symbolic addressing, MM allows specifying the memory address using a 
symbolic address.   

The MM application is written in C and depends on the cFS Operating System
Abstraction Layer (OSAL) and cFE components.  There is additional MM application
specific configuration information contained in the application user's guide.

User's guide information can be generated using Doxygen (from top mission directory):
```
  make prep
  make -C build/docs/mm-usersguide mm-usersguide
```

## Software Required

cFS Framework (cFE, OSAL, PSP)

An integrated bundle including the cFE, OSAL, and PSP can
be obtained at https://github.com/nasa/cfs

## About cFS

The cFS is a platform and project independent reusable software framework and
set of reusable applications developed by NASA Goddard Space Flight Center.
This framework is used as the basis for the flight software for satellite data
systems and instruments, but can be used on other embedded systems.  More
information on the cFS can be found at http://cfs.gsfc.nasa.gov
