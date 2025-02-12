# How to compile

  This section will describe how to compile on the following 3 platforms:

  - [Windows 64-bit](#windows-64-bit)
  - [Mac 64-bit](#mac-64-bit)
  - [Ubuntu](#ubuntu)
## Windows 64-bit  

### CASE 1 : you are using Visual studio 2019

  **Tools needed:**

  | Tool | Description |
  |---|---|
  | Visual studio 2019 | need's a subscription |
  | Cmake | Version > 3.10|
  | git ||
  | Strawberry Perl ||


  **How to build:**

  - Open the `x64 Native Tools Command Prompt for VS 2019`
  - Clone the project using 
  ```
  git clone https://github.com/SoftFever/OrcaSlicer.git
  ```
  - Run:
  ```
  git lfs pull
  ```

  *If you want to build the release version, you need to :*

  - Run :
  ```
  build_release.bat
  ```
  **NB** This script will download and install all relevant dependencies relative to the release version and compile OrcaSlicer.
  - You can then open the `OrcaSlicer.sln` file via `Visual studio 2019` in the `build` folder.

  *If you want to build the debug version, you need to :*

  - Run :
  ```
  build_release.bat debug
  ```
  **NB** This script will download and install all relevant dependencies relative to the debug version and compile OrcaSlicer.
  - You can then open the `OrcaSlicer.sln` file via `Visual studio 2019` in the `build-dbg` folder.

### CASE 2 : you are using Visual studio 2022

  | Tool | Description |
  |---|---|
  | Visual studio 2022 | IDE, Community version is free |
  | Cmake | Version > 3.10 |
  | git | |
  | Strawberry Perl | |

 **How to build:**

  - Open the `x64 Native Tools Command Prompt for VS 2022`
  - Clone the project using 
  ```
  git clone https://github.com/SoftFever/OrcaSlicer.git
  ```
  - Run:
  ```
  git lfs pull
  ```

  *If you want to build the release version, you need to :*

  - Run :
  ```
  build_release_vs2022.bat
  ```
  **NB** This script will download and install all relevant dependencies relative to the release version and compile OrcaSlicer.
  - You can then open the `OrcaSlicer.sln` file via `Visual studio 2022` in the `build` folder.

  *If you want to build the debug version, you need to :*

  - Run :
  ```
  build_release_vs2022.bat debug
  ```
  **NB** This script will download and install all relevant dependencies relative to the debug version and compile OrcaSlicer.
  - You can then open the `OrcaSlicer.sln` file via `Visual studio 2022` in the `build-dbg` folder.

## Mac 64-bit  
  - Tools needed: Xcode, Cmake, git, gettext
  - run `build_release_macos.sh`

## Ubuntu  
  - run `BuildLinux.sh -udisr`