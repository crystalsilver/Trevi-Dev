# Trevi-Develop

[![Swift 2.2](https://img.shields.io/badge/Swift-2.2-orange.svg?style=flat)](https://developer.apple.com/swift/)
[![Mac OS X](https://img.shields.io/badge/platform-osx-lightgrey.svg?style=flat)](https://developer.apple.com/swift/)
![Apache 2](https://img.shields.io/badge/license-Apache2-blue.svg?style=flat)

## Overview
An xcode workspace for OSX developers. The worksapce contains projects related with project Trevi.  
See more at [Trevi Community's GitHub repo](https://github.com/Trevi-Swift).

## Versioning
Trevi-Develop follows the semantic versioning scheme. The API change and backwards compatibility rules are those indicated by SemVer.

## Usage
1. Clone repository.
  
  ```bash
  $ git clone https://github.com/Trevi-Swift/Trevi-Dev.git --recursive
  ````
  
  or
  
  ```bash
  $ git clone https://github.com/Trevi-Swift/Trevi-Dev.git
  $ cd Trevi-Dev
  $ git submodule init
  $ git submodule update
  ```

2. Build libuv. Choose one of ways to build libuv :
    
    - On the system directory.  
        
        ```bash
        $ git clone https://github.com/libuv/libuv.git
        $ cd libuv
        $ sh autogen.sh
        $ ./configure
        $ make
        $ make check
        $ make install
        ```
        
        or using homebrew :
        
        ```bash
        $ brew install --HEAD libuv
        ```
        
        More details : Build Instructions on [libuv](https://github.com/libuv/libuv)

  - On the project directory.
        
        ```bash
        $ make -C ./swift-libuv
        ```

## License
This library is licensed under Apache 2.0. Full license text is available in [LICENSE](LICENSE.txt).