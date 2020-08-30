# Kitsunemimi-Project-Meta

This repository is only to keep an overview of my public and private repositories. With this the version of library requirements should be in sync. Beside this it is for issue tickets, which affect all repositories.

For the case that you ask, why it is named `Kitsunemimi-Project`: Its is not related to the content of the repositories. Originally I searched for a name schema for the libraries to differentiation them from other libraries. For this and because my private domain was already `kitsunemimi.moe`, I decided to name my libraries `libKitsunemimi...` and after some time I decided to make this as to the project name and collect all my sub-projects under this name, because kitsunemimi are moe. ;) 

Contact for questions: tobias.anker@kitsunemimi.moe

## Overview

The following diagramm shows the relations of the library and tools with each other. I know its not a vaild UML-diagramm, but I wanted to reduce the complexety to keep it a bit smaller. 

<p align="center">
  <img src=".pictures/overview.png?raw=true" alt="Overview"/>
</p>

### Sakura-Project

The Sakura-Project provides an automation tool to deploy applications, with high performance thanks to some features like easy parallelism of tasks and a self-created file syntax. It was primary created for the components of the Kyouko-Project and beside this also to automate different tasks on my deployment at home.

See documentation of the latest master-version: [Sakura-Project-Documentation.pdf](https://gitlab.com/kitsudaiki/Sakura-Project-Documentation/builds/artifacts/master/browse?job=build) (this documentation is fall behind the implemetation at the moment, because I have only a very limited amount of time available for my private projects. Sorry :( But SakuraTree reached now the feature-freeze for version 0.3.0, so I will bring the documentation up-to-date in the next weeks.)

[SakuraTree](#SakuraTree)

[libKitsunemimiSakuraNetwork](#libKitsunemimiSakuraNetwork)

[libKitsunemimiSakuraLang](#libKitsunemimiSakuraLang)

### Kyouko-Project (still private)

This is the main-project here, but it is still far away to be usable for any task, so its still private. In the core it provides an artificial neural network based on a concept created by myself. 

[KyoukoMind](#KyoukoMind)

[ToriiGateway](#ToriiGateway)

[MiyuMonitoring](#MiyuMonitoring)

[MiraiControl](#MiraiControl)

[libKitsunemimiKyoukoCommon](#libKitsunemimiKyoukoCommon)

### generic project libraries

Libraries for common usage inside of the Kitsunemimi-Project. 

[libKitsunemimiProjectNetwork](#libKitsunemimiProjectNetwork)

### generic libraries

These simple generic libraries with wrapper, parser and functionalities I often use. Most of these stuff like CLI-argument-parser and so on, already exist in various implementations on github, but I wanded to create my own versions to have maximum control over the requirements and to have only a minimal set of funtions, which I really need.

[libKitsunemimiOpengl](#libKitsunemimiOpengl)

[libKitsunemimiObj](#libKitsunemimiObj)

[libKitsunemimiOpencl](#libKitsunemimiOpencl)

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

- **visibility**: `public`

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

- **visibility**: `public`

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

- **visibility**: `public`

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

- **visibility**: `public`

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

- **visibility**: `public`

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

- **visibility**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiNetwork.git

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

- **visibility**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiArgs.git

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

- **visibility**: `public`

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

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.15.1 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.10.0 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiIni | v0.4.4 | https://github.com/kitsudaiki/libKitsunemimiIni.git


## libKitsunemimiObj

#### Metadata

- **content**: This library provides a simple and minimal wavefront obj-parser and creator to generate the content of such files.

- **current version**: `0.2.3`

- **license**: `MIT`

- **language**: `C++14`

- **visibility**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiObj.git

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

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.13.0 |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | v0.8.2 | https://github.com/kitsudaiki/libKitsunemimiPersistence.git


## libKitsunemimiOpencl

#### Metadata

- **content**: Simple wrapper-library for some commonly used OpenCL-functionallities.

- **current version**: `0.1.0`

- **license**: `MIT`

- **language**: `C++14`

- **visibility**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiOpencl.git

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
opencl-headers  | opencl-headers | 2.x | Header-files for opencl
ocl-icd-opencl-dev | ocl-icd-opencl-dev | 2.x | libraries for opencl

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master |  https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | master | https://github.com/kitsudaiki/libKitsunemimiPersistence.git


## libKitsunemimiOpengl

#### Metadata

- **content**: Simple wrapper-library for some commonly used OpenGL-functionallities.

- **current version**: -

- **license**: `MIT`

- **language**: `C++14`

- **visibility**: `private`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiOpengl.git

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required generic libraries

name | repository | version | task
--- | --- | --- | ---
libglew-dev  | libglew-dev | 2.x | -
libsdl2-dev | libsdl2-dev | 2.x | -

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master |  https://github.com/kitsudaiki/libKitsunemimiCommon.git


## libKitsunemimiProjectNetwork

#### Metadata

- **content**: Self-created session-layer-protocol for network-communication in the Kitsunemimi-projects.

- **current version**: `0.2.0`

- **license**: `Apache 2`

- **language**: `C++14`

- **visibility**: `public`

- **location**: `Github`

- **repo-pth**: https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git

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

- **visibility**: `public`

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

name | repository | version | task
--- | --- | --- | ---
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

- **visibility**: `public`

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

name | repository | version | task
--- | --- | --- | ---
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

- **visibility**: `public`

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

name | repository | version | task
--- | --- | --- | ---
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


## libKitsunemimiKyoukoCommon

#### Metadata

- **content**: Common library for the components of the Kyouko-Project. Primary packet definitions for network-communication between the components.

- **current version**: `-`

- **language**: `C++14`

- **visibility**: `private`

- **location**: `self-hosted Gitlab`

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master | https://github.com/kitsudaiki/libKitsunemimiCommon.git


## KyoukoMind

#### Metadata

- **content**: Provides an artificial neural network based on a concept created by myself. It is way more dynaic than the commonly used deep-learning networks.

- **additional commentary**: Even the concept is already in progress for some years, it is still at the beginning and had only reached the first primitiv proof-of-concept. The first version had a very high dynamic, which provided many fancy possibilities, but it had really bad performance and was not capable to perform on a GPU. So at the moment I try to bring it working again with a reduced version of the concept and am on the way to the second PoC, but there it is possible that it failes and I have to cancel this project.

- **current version**: `0.1.0` (first PoC)

- **language**: `C++14`

- **visibility**: `private`

- **location**: `self-hosted Gitlab`

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

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | master | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiArgs | master | https://github.com/kitsudaiki/libKitsunemimiArgs.git
libKitsunemimiConfig | master | https://github.com/kitsudaiki/libKitsunemimiConfig.git
libKitsunemimiJson | master | https://github.com/kitsudaiki/libKitsunemimiJson.git
libKitsunemimiIni | master | https://github.com/kitsudaiki/libKitsunemimiIni.git
libKitsunemimiNetwork | master | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
libKitsunemimiOpencl | master| https://github.com/kitsudaiki/libKitsunemimiOpencl.git
libKitsunemimiObj | master| https://github.com/kitsudaiki/libKitsunemimiObj.git
libKitsunemimiProjectNetwork | master| https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git
libKitsunemimiKyoukoCommon | master | -



## ToriiGateway

#### Metadata

- **content**: Proxy for networking communication between the components.

- **current version**: -

- **language**: `C++14`

- **visibility**: `private`

- **location**: `self-hosted Gitlab`

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.

#### Required generic libraries

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | master | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiArgs | master | https://github.com/kitsudaiki/libKitsunemimiArgs.git
libKitsunemimiNetwork | master | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
libKitsunemimiProjectNetwork | master | https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git
libKitsunemimiKyoukoCommon | master | -


## MiyuMonitoring

#### Metadata

- **content**: Graphical monitoring tool for visualization of the activity inside of the KyoukoMind-instance.

- **current version**: -

- **language**: `C++14`

- **visibility**: `private`

- **location**: `self-hosted Gitlab`

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++

- QT 5 with QML

#### Required generic libraries

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | master | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiNetwork | master | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
libKitsunemimiProjectNetwork | master | https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git
libKitsunemimiKyoukoCommon | master | -


## MiraiControl

#### Metadata

- **content**: Controlling client to interact with a KyoukoMind-instance.

- **current version**: -

- **language**: `C++14`

- **visibility**: `private`

- **location**: `self-hosted Gitlab`

#### required tools to build

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | >= 6.0 | Compiler for the C++ code.
make | make | >= 4.0 | process the make-file, which is created by qmake to build the programm with g++
qmake | qt5-qmake | >= 5.0 | This package provides the tool qmake, which is similar to cmake and create the make-file for compilation.
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | >= 3.0 | Build the parser-code together with the lexer-code.

#### Required generic libraries

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
ssl library | libssl-dev | 1.1.x | encryption for tls connections

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | master | https://github.com/kitsudaiki/libKitsunemimiCommon.git
libKitsunemimiPersistence | master | https://github.com/kitsudaiki/libKitsunemimiPersistence.git
libKitsunemimiArgs | master | https://github.com/kitsudaiki/libKitsunemimiArgs.git
libKitsunemimiJson | master | https://github.com/kitsudaiki/libKitsunemimiJson.git
libKitsunemimiNetwork | master | https://github.com/kitsudaiki/libKitsunemimiNetwork.git
libKitsunemimiProjectNetwork | master | https://github.com/kitsudaiki/libKitsunemimiProjectNetwork.git
libKitsunemimiKyoukoCommon | master | -
