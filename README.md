# Kitsunemimi-Projects



## libKitsunemimiCommon 

- **content**: Simple C++ library with commenly used functions for memory-handling, thread-handling, data representation and testing. 

- **current version**: `0.15.0`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiCommon.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.



## libKitsunemimiPersistence

- **content**: Functionalities to read and write files and logging.

- **current version**: `0.8.2`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiPersistence.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required generic libraries

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
sqlite3 library | libsqlite3-dev | 3.x | handling of sqlite databases

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git



## libKitsunemimiJson

- **content**: Parser for the content of json-files.

- **current version**: `0.10.2`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiJson.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git



## libKitsunemimiIni

- **content**: Parser for the content of ini-files.

- **current version**: `0.4.3`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiIni.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git



## libKitsunemimiJinja2

- **content**: Simple but imcomplete converter for jinja2-templates.

- **current version**: `0.7.2`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiJinja2.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiJson | v0.10.2 |  https://github.com/kitsudaiki/libKitsunemimiJson.git



## libKitsunemimiNetwork

- **content**: Provides unix-domain-sockets, tcp-sockets and tls-encrypted tcp-sockets.

- **current version**: `0.6.2`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiNetwork.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.8.2 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git



## libKitsunemimiArgs

- **content**: Parser for cli-arguments.

- **current version**: `0.1.3`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiArgs.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.8.2 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git



## libKitsunemimiConfig

- **content**: Parser for cli-arguments.

- **current version**: `0.2.2`

- **license**: `MIT`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiConfig.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.8.2 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiIni | v0.4.3 | https://github.com/kitsudaiki/libKitsunemimiIni.git



## libKitsunemimiProjectNetwork

- **content**: Self-created session-layer-protocol for network-communication in the Kitsunemimi-projects.

- **current version**: `-`

- **license**: `Apache 2`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.12.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.8.1 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiNetwork | v0.6.1 | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
