libsmbmm is a simple C++ interface to the C libsmbclient library provided by the Samba project.

It allows you to simply use windows SMB networks using C++. It only depends on libsmbclient and supports almost all the operations that libsmbclient does (I haven't tested printing).

Caveat: Some evil C pointer magic remains, but you don't have to deal with memory allocation. Specifically you are **not** responsible for deleting the smbc\_dirent**from SMBDir::Read().**

The library is pretty simple - just 2 files (smbmm.h and smbmm.cpp). Just download them from SVN trunk, add them to your project and use the classes/functions in smbmm.h

The API should be fairly obvious from looking at smbmm.h.

If you have any problems email me, or use the issue tracker.