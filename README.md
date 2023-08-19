# Code formatting RFCs

This repository exists to decide on a code style for [C/C++ code](https://whvcse-robot-lab.github.io/wiki/Standard/CodeStyles/Cpp/), 
to be enforced by `clang-format`,`clang-tidy` tool.
Accepted RFCs live in the directory and form a specification for formatting tools.`.clang-format`,`.clang-tidy`

## Format All The Things!
This repository contains a bash script that will run `clang-format -i` on your code.

Features:
* Find the right path to `clang-format` on Linux, which may encode the LLVM version in the `clang-format` filename
* Fixes files recursively
* Detects the most common file extensions used by C/C++ projects

## Usage

### Step 1
Move the `.clang-format` from the current repository to your project directory.

### Step 2
#### Manual Formatting
Run script:

```bash
clang-format-all src/
```

#### Automated Formatting

Use the built-in or available plugins in your integrated development environment (IDE) or code editor to automate code formatting.

* [CLion](https://www.jetbrains.com/help/clion/clangformat-as-alternative-formatter.html#clion-support)
* [Visual Studio Code](https://code.visualstudio.com/docs/cpp/cpp-ide)
* ...

## TODO
* Support for `Windows` platform
* Support for `clang-tidy` tools

## Acknowledgments

We would like to extend our sincere appreciation to the following projects and individuals for their invaluable contributions and inspiration:
- [eklitzke/clang-format-all](https://github.com/eklitzke/clang-format-all)
- [SJTU-Robomaster-Team/style-team](https://github.com/SJTU-RoboMaster-Team/style-team/tree/main)
