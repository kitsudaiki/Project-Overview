# Kitsunemimi-Project-Overview



## libKitsunemimiCommon 

- **content**: Different commonly used functionalities.

- **current version**: `0.12.1`

- **license**: `MIT`

- **repo-pth**: https://github.com/tobiasanker/libKitsunemimiCommon.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | 6.x | Compiler for the C++ code.
qmake | qt5-qmake | 5.x | This package provides the tool qmake, to build the project



## libKitsunemimiPersistence

- **content**: Functionalities to read and write files and logging.

- **current version**: `0.8.1`

- **license**: `MIT`

- **repo-pth**: https://github.com/tobiasanker/libKitsunemimiPersistence.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | 6.x | Compiler for the C++ code.
qmake | qt5-qmake | 5.x | This package provides the tool qmake, to build the project

#### Required generic libraries

name | repository | version | task
--- | --- | --- | ---
boost-filesystem library | libboost-filesystem-dev | 1.6x | interactions with files and directories on the system
sqlite3 library | libsqlite3-dev | 3.x | handling of sqlite databases

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.12.1 |  https://github.com/tobiasanker/libKitsunemimiCommon.git



## libKitsunemimiJson

- **content**: Parser for the content of json-files.

- **current version**: `0.10.1`

- **license**: `MIT`

- **repo-pth**: https://github.com/tobiasanker/libKitsunemimiJson.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | 6.x | Compiler for the C++ code.
qmake | qt5-qmake | 5.x | This package provides the tool qmake, to build the project
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.12.1 |  https://github.com/tobiasanker/libKitsunemimiCommon.git



## libKitsunemimiIni

- **content**: Parser for the content of ini-files.

- **current version**: `0.4.2`

- **license**: `MIT`

- **repo-pth**: https://github.com/tobiasanker/libKitsunemimiIni.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | 6.x | Compiler for the C++ code.
qmake | qt5-qmake | 5.x | This package provides the tool qmake, to build the project
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.12.1 |  https://github.com/tobiasanker/libKitsunemimiCommon.git



## libKitsunemimiIni

- **content**: Simple but imcomplete converter for jinja2-templates.

- **current version**: `0.7.1`

- **license**: `MIT`

- **repo-pth**: https://github.com/tobiasanker/libKitsunemimiJinja2.git

### Requirements

#### Required build tools

name | repository | version | task
--- | --- | --- | ---
g++ | g++ | 6.x | Compiler for the C++ code.
qmake | qt5-qmake | 5.x | This package provides the tool qmake, to build the project
FLEX | flex | >= 2.6 | Build the lexer-code for all used parser.
GNU Bison | bison | 3.x | Build the parser-code together with the lexer-code.

#### Required kitsunemimi libraries

Repository-Name | Version-Tag | Download-Path
--- | --- | ---
libKitsunemimiCommon | v0.12.1 |  https://github.com/tobiasanker/libKitsunemimiCommon.git
libKitsunemimiJson | v0.10.1 |  https://github.com/tobiasanker/libKitsunemimiJson.git
