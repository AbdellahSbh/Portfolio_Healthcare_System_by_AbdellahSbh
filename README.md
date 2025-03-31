# Healthcare Management System

This is a C++ backend project using the Crow web framework. It simulates a simple healthcare API that manages patient information and handles JSON input/output using nlohmann's JSON library.

---

## Features

- Define and store patient data (name, age, gender, ID, diagnosis)
- Handle HTTP requests using Crow routing
- JSON-based responses for easy testing and integration
- In-memory data handling (no persistent storage)

---

## Technologies Used

- **Language:** C++
- **Framework:** Crow (header-only C++ web framework)
- **JSON Library:** [nlohmann/json](https://github.com/nlohmann/json)
- **Compiler:** g++ (C++17), tested on Windows (should work on Linux/macOS)

---

## Project Structure

. ├── app/ │ └── main.cpp # Core logic and route handlers ├── .vscode/ │ └── tasks.json # VSCode build tasks (optional) ├── README.md

## Installation and Running

1. **Download Dependencies**

   - `crow_all.h` or `crow.h` from: https://github.com/CrowCpp/Crow
   - `json.hpp` from: https://github.com/nlohmann/json

   Place them either next to `main.cpp` or in an `include/` folder.

2. **Compile the project**

```bash
g++ app/main.cpp -o server -std=c++17 -pthread

Run the server
./server
The server will run on http://localhost:18080

You can use Postman, curl, or browser (for GET requests)
