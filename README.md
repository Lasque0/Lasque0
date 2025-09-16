<h1 align="center">
  <span style="color:#FF3131; font-weight:bold;">Lasque</span>
</h1>
<h3 align="center" style="color:#ff0000;">C++ Junior Developer</h3>

---

### ⚙️ Tech Stack

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" title="C++" alt="C++" width="60" height="60" />
</p>

---

### 🧠 <span style="color:#FF3131;">About Me</span>

<blockquote>
  <p><strong style="color:#FF5555;">┌──────────────────────────────</strong></p>
  <p><strong style="color:#FF5555;">│</strong> 🌍 From Turkey</p>
  <p><strong style="color:#FF5555;">│</strong> 👨‍💻 Focused on low-level programming</p>
  <p><strong style="color:#FF5555;">│</strong> ⚙️ Loves building desktop tools</p>
  <p><strong style="color:#FF5555;">│</strong> 🧠 Always learning & pushing limits</p>
  <p><strong style="color:#FF5555;">└──────────────────────────────</strong></p>
</blockquote>

---

### 💻 Sample C++ Code: File Read & Write

```cpp
#include <iostream>
#include <fstream>
#include <string>

int main() {
    std::string filename = "example.txt";

    // Writing to file
    std::ofstream outFile(filename);
    if (!outFile) {
        std::cerr << "Unable to open file!" << std::endl;
        return 1;
    }
    outFile << "Hello, Lasque0!" << std::endl;
    outFile << "This file was written by C++." << std::endl;
    outFile.close();

    // Reading from file
    std::ifstream inFile(filename);
    if (!inFile) {
        std::cerr << "Unable to open file!" << std::endl;
        return 1;
    }

    std::string line;
    std::cout << "File contents:" << std::endl;
    while (std::getline(inFile, line)) {
        std::cout << line << std::endl;
    }
    inFile.close();

    return 0;
}
