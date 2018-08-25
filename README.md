# What The Hell Is: C++

This project is an experimental concept I came up with as a user guide for C++.
The reader is supposed navigate the guide only through code completions provided by their text-editors/IDEs.

## How does this even work?
A better way to showcase the vision of this project would to provide with an example

For example the reader opened up `open_me_first.cpp`.

The reader writes:
```cpp
a_how_do_I_declare_variables
```
This invokes a macro that prints out the answer for the query.
The point of defining a macro like this is solely the fact that the reader knows that they can lookup beginner level guides using macros starting with `a_`.
All of these usage instructions will be added to the top of `open_me_first.cpp` for ease of reference.

This can be used to add all kinds of useful information. Maybe some easter eggs can also be added :P.

Unfortunately macros are not context aware, which means that we may need to overcome this shortcoming by using `#ifdef` directives inside macro definitions.

## SETUP instructions
These instructions are valid for both contributors and users of this manual.
1. Install [CMake](https://cmake.org/).
2. Clone this repository: `git clone https://github.com/IronicallySerious/wth-is-cpp`
3. Navigate to `wth-is-cpp/` and create a `build/` directory: `cd wth-is-cpp/ && mkdir build`
4. Run CMake: `cd build/ && cmake ..`
5. Execution instructions:
	1. For Linux users:
		1. Navigate to `build/`
		2. Build the project: `make`
		3. Run: `./wth-is-cpp`
	2. For Windows users:
		1. Open `Project.sln` from `wth-is-cpp/build` in Visual Studio (recommended for Intellisense suggestions)
		2. Right click on `wth-is-cpp` project and select `Select as StartUp Project`
		3. Press F5 to build and run.
