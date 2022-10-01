## Running on Windows

### To install gcc
Step 1: Install Mingw-w64 via Msys2. [https://www.msys2.org](https://www.msys2.org)   
Step 2: Once installed, a Mingw-w64 environment is opened in a window. Install the full Mingw-w64 toolchain   
`pacman -S --needed base-devel mingw-w64-x86_64-toolchain`    
Step 3: Add Mingw-w64 bin folder to your Windows PATH environment variable.     
Step 4: In a new terminal window, to check if gcc has been installed correctly, type
`gcc --version`.    
If you don't see the expected output or g++ or gdb is not a recognized command, make sure your PATH entry matches the Mingw-w64 binary location where the compiler tools are located.

### Run the program
Step 1 : Clone the repository from: [https://github.com/akshitkaranam/CZ4031_Project1](https://github.com/akshitkaranam/CZ4031_Project1.git)    

Step 2 : Open a new terminal window, and navigate to the project directory     
Step 3 :  Compile all the relevant files in the src folder    

```sh
cd src
g++ -std=c++11 -c Address.cpp Record.cpp Block.cpp Storage.cpp Node.cpp InternalNode.cpp LeafNode.cpp AddressNode.cpp BPlusTree.cpp 
```
Step 4 :  Compile all the relevant files in the src folder

```sh
g++ -std=c++11 main.cpp -o main  Address.o Record.o Block.o Storage.o Node.o InternalNode.o LeafNode.o AddressNode.o BPlusTree.o
```
Step 5 : To run the exectuable file

```sh
main
```

## Running on macOS

### Run the program
Step 1 : Clone the repository from: [https://github.com/akshitkaranam/CZ4031_Project1](https://github.com/akshitkaranam/CZ4031_Project1.git)

Step 2 : Open a new terminal window, and navigate to the project directory    
Step 3 :  Compile all the relevant files in the src folder

```sh
cd src
g++ -std=c++11 -c Address.cpp Record.cpp Block.cpp Storage.cpp Node.cpp InternalNode.cpp LeafNode.cpp AddressNode.cpp BPlusTree.cpp 
```
Step 4 :  Compile all the relevant files in the src folder

```sh
g++ -std=c++11 main.cpp -o main  Address.o Record.o Block.o Storage.o Node.o InternalNode.o LeafNode.o AddressNode.o BPlusTree.o
```
Step 5 : To run the exectuable file

```sh
./main
```
