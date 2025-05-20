# Labor_ArithmetischerBaum

## Project Description

This project implements an arithmetic expression parser and evaluator. It can process mathematical expressions in three different formats:
- Prefix notation
- Infix notation 
- Postfix notation 

## Build Instructions

### Prerequisites

- CMake (version 3.22 or higher)
- C++ compiler supporting C++17 standard

### Building the Project

#### TLDR (copy paste)
Windows (CMD)
```powershell
powershell -command "clear; mkdir build; cd build; cmake ..; cmake --build .; cd ..; ./build/LaborRechenBaum.exe '|' '((2+3)*(5+(4*4)))+(7*8-(9/3)+(10/10))'; rm -r ./build"
```

Windows (Powershell)
```powershell
clear; mkdir build; cd build; cmake ..; cmake --build .; cd ..; ./build/LaborRechenBaum.exe "|" "((2+3)*(5+(4*4)))+(7*8-(9/3)+(10/10))"; rm -r ./build
```

Linux
```sh
cls; mkdir build && cd build && cmake .. && cmake --build . && cd .. && ./build/LaborRechenBaum "|" "((2+3)*(5+(4*4)))+(7*8-(9/3)+(10/10))" && rm -r ./build
```


#### Using Command Line

1. **Create a build directory (if it doesn't exist):**

```powershell
mkdir build
cd build
```

2. **Generate build files with CMake:**

```powershell
cmake ..
```

3. **Build the project:**

```powershell
cmake --build .
```

### Examples Windows

```powershell
# Infix notation example
./build/LaborRechenBaum.exe | "((2+3)*(5+(4*4)))+(7*8-(9/3)+(10/10))"

# If no arguments are provided, the program will prompt for input
./build/LaborRechenBaum.exe
```

### Example Linux / WSL

```sh
# Infix notation example
./build/LaborRechenBaum "|" "((2+3)*(5+(4*4)))+(7*8-(9/3)+(10/10))"

# If no arguments are provided, the program will prompt for input
./build/LaborRechenBaum
```