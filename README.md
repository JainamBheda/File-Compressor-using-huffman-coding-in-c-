# File Compressor and Decompressor in C++

A simple command-line file compressor and decompressor implemented in C++ using the Huffman coding algorithm. This project demonstrates techniques in data compression, file I/O, and modern C++ practices (C++17). The primary goal is to efficiently compress and decompress text files using Huffman encoding, which is widely used for lossless data compression.

---

## 📋 Table of Contents

- [Features](#-features)
- [Prerequisites](#-prerequisites)
- [Building](#-building)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Examples](#-examples)
- [Future Improvements](#-future-improvements)
- [Contributing](#-contributing)
- [License](#-license)
- [Acknowledgments](#-acknowledgments)
- [Conclusion](#-conclusion)

---

## 🔍 Features

- **Huffman Encoding & Decoding**: Lossless compression using Huffman trees.
- **Modular Design**: The project is divided into well-defined classes that focus on specific functionalities like frequency counting, tree construction, and file I/O.
- **CMake Support**: Cross-platform compilation support through CMake, making it easy to build on any system.
- **Command-Line Interface**: Simple and intuitive commands for compressing and decompressing files.
- **File Integrity**: Ensures that the decompressed file matches the original file in terms of content.

---

## 🛠️ Prerequisites

To build this project, you need:

- A C++17-compatible compiler:
  - **g++** (Linux/macOS)
  - **clang++** (macOS)
  - **MSVC** (Windows)
- **CMake** (optional, but recommended for managing the build)
- **Git** for cloning the repository.

---

## ⚙️ Building

### 1. Using g++ directly

```bash
# Clone the repo
git clone https://github.com/JainamBheda/file_compressor_decompressor_in_c++.git
cd file_compressor_decompressor_in_c++

# Compile all source files
# On Linux/macOS:
g++ -std=c++17 \
  FrequencyCounter.cpp \
  Huffman.cpp \
  HuffmanUtility.cpp \
  Node.cpp \
  main.cpp \
  -o huffman

# On Windows (PowerShell or CMD):
g++ -std=c++17 FrequencyCounter.cpp Huffman.cpp HuffmanUtility.cpp Node.cpp main.cpp -o huffman.exe
```

## 📂 Project Structure

- FrequencyCounter.cpp: Contains the logic for counting the frequency of characters in the input text.

- Huffman.cpp: Implements the Huffman encoding and decoding algorithms.

- HuffmanUtility.cpp: Utility functions for file I/O and other helper operations.

- Node.cpp: Defines the node structure used in the Huffman tree.

- main.cpp: The entry point for the program, responsible for handling the command-line interface.

## 🚀 Future Improvements
- Multithreading Support: Implement parallel processing to speed up compression and decompression for larger files.

- Error Handling: Add better error handling for edge cases like corrupted files or unsupported formats.

- Graphical User Interface (GUI): Provide a GUI for users who prefer not to use the command line.

- Support for Other Compression Algorithms: Integrate other popular compression algorithms like LZ77 or Run-Length Encoding (RLE).

## 🤝 Contributing

We welcome contributions! If you'd like to improve the project, feel free to fork the repository, create a branch, and submit a pull request.

## 🙏 Acknowledgments
https://en.wikipedia.org/wiki/Huffman_coding for providing the foundation for lossless data compression.

## 🎯 Conclusion
This file compressor and decompressor project is an effective demonstration of how Huffman coding can be applied to text file compression. It highlights the power of lossless data compression, helping reduce file sizes for easier storage and transmission. With a modular design and simple command-line interface, this project serves as a solid foundation for learning and implementing compression algorithms in C++. Future improvements can expand its functionality, making it a more versatile tool for various use cases.
