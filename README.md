# Kitsunemimi-Projects-Meta

This repository is only to keep an overview of my repositories. With this the version of library requirements should be in sync and this project is for issue tickets, which affect all repositories.

## Overview

### Sakura-Project

[SakuraTree](#SakuraTree)

[libKitsunemimiSakuraNetwork](#libKitsunemimiSakuraNetwork)

[libKitsunemimiSakuraLang](#libKitsunemimiSakuraLang)

### generic project libraries

[libKitsunemimiProjectNetwork](#libKitsunemimiProjectNetwork)

### generic libraries

[libKitsunemimiConfig](#libKitsunemimiConfig)

[libKitsunemimiArgs](#libKitsunemimiArgs)

[libKitsunemimiNetwork](#libKitsunemimiNetwork)

[libKitsunemimiJinja2](#libKitsunemimiJinja2)

[libKitsunemimiIni](#libKitsunemimiIni)

[libKitsunemimiJson](#libKitsunemimiJson)

[libKitsunemimiPersistence](#libKitsunemimiPersistence)

[libKitsunemimiCommon](#libKitsunemimiCommon)


## Repositories

### libKitsunemimiCommon 

#### Metadata

- **content**: Simple C++ library with commenly used functions for memory-handling, thread-handling, data representation and testing. 

- **current version**: `0.15.1`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiCommon.git

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.



### libKitsunemimiPersistence

#### Metadata

- **content**: This library contains all my functions for interactions with the storage. At the moment its the smalest of my projects and only contains functionality to read, modify and write binaray- and text- files, handle an sqlite3-database and write log-files.

- **current version**: `0.10.0`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiPersistence.git

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
sqlite3 library | libsqlite3-dev | 3.x | handling of sqlite databases (only when build with sqlite)

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git



## libKitsunemimiJson

#### Metadata

- **content**: Parser for the content of json-files.

- **current version**: `0.10.3`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiJson.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git



## libKitsunemimiIni

#### Metadata

- **content**: Parser for the content of ini-files.

- **current version**: `0.4.4`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiIni.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git



## libKitsunemimiJinja2

#### Metadata

- **content**: Simple but imcomplete converter for jinja2-templates.

- **current version**: `0.7.3`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiJinja2.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiJson | v0.10.3 |  https://github.com/kitsudaiki/libKitsunemimiJson.git



## libKitsunemimiNetwork

#### Metadata

- **content**: This is a small library for network connections. It provides servers and clients for unix-domain-sockets, tcp-sockets and ssl encrypted tcp-sockets.

- **current version**: `0.6.4`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiNetwork.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git



## libKitsunemimiArgs

#### Metadata

- **content**: Small and easy to use parser for CLI-arguments.

- **current version**: `0.2.0`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiArgs.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.20.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git



## libKitsunemimiConfig

#### Metadata

- **content**: Parser for cli-arguments.

- **current version**: `0.2.3`

- **license**: `MIT`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiConfig.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiIni | v0.4.4 | https://github.com/kitsudaiki/libKitsunemimiIni.git



## libKitsunemimiProjectNetwork

#### Metadata

- **content**: Self-created session-layer-protocol for network-communication in the Kitsunemimi-projects.

- **current version**: `0.2.0`

- **license**: `Apache 2`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git

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
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiNetwork | v0.6.4 | https://github.com/kitsudaiki/libKitsunemimiNetwork.git


## libKitsunemimiSakuraLang

#### Metadata

- **content**: This is the parser-library for SakuraTree (https://github.com/kitsudaiki/SakuraTree) to parse all project-specific files.

- **current version**: `0.3.1`

- **license**: `Apache 2`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiSakuraLang.git

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | >= 3.0 | Build the parser-code together with the lexer-code.

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.15.1 | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git


## libKitsunemimiSakuraNetwork

#### Metadata

- **content**: The network-library for SakuraTree (https://github.com/kitsudaiki/SakuraTree) to connect all components and transfer commands and files.

- **current version**: `0.1.0`

- **license**: `Apache 2`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiSakuraNetwork.git

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | >= 3.0 | Build the parser-code together with the lexer-code.

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.15.1 | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiNetwork | v0.6.4 | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
libKitsunemimiProjectNetwork | v0.2.0 | https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git
libKitsunemimiSakuraLang | v0.3.1 | https://github.com/kitsudaiki/libKitsunemimiSakuraLang.git



## SakuraTree

#### Metadata

- **content**: This is/should become a simple-to-use and fast automation tool to deploy tools and files on multiple nodes.

- **current version**: `0.3.0-ff`

- **license**: `Apache 2`

- **language**: `C++14`

- **state**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/SakuraTree.git

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | >= 3.0 | Build the parser-code together with the lexer-code.
xxd | xxd | >= 1.10 | converts text files into source code files

#### Required generic libraries

boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.15.1 | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiArgs | v0.2.0 | https://github.com/kitsudaiki/libKitsunemimiArgs.git
libKitsunemimiConfig | v0.2.3 | https://github.com/kitsudaiki/libKitsunemimiConfig.git
libKitsunemimiJson | v0.10.3 | https://github.com/kitsudaiki/libKitsunemimiJson.git
libKitsunemimiJinja2 | v0.7.3 | https://github.com/kitsudaiki/libKitsunemimiJinja2.git
libKitsunemimiIni | v0.4.4 | https://github.com/kitsudaiki/libKitsunemimiIni.git
libKitsunemimiNetwork | v0.6.4 | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
libKitsunemimiProjectNetwork | v0.2.0 | https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git
libKitsunemimiSakuraLang | v0.3.1 | https://github.com/kitsudaiki/libKitsunemimiSakuraLang.git
libKitsunemimiSakuraNetwork | v0.1.0 | https://github.com/kitsudaiki/libKitsunemimiSakuraNetwork.git

