# Healthcare Management System 🏥

This project is a simple backend simulation of a Healthcare Management System built using Crow, a C++ web framework. It handles basic functionality like managing patient records and simulates real-time updates with JSON responses.

---

## 📌 Features

- C++ Crow web server
- JSON-based API responses
- Simulated patient management (GET, POST, etc.)
- Annotated routes with `crow::SimpleApp`
- Lightweight and fast execution

---

## 🛠️ Technologies Used

- C++17
- Crow Web Framework (https://github.com/CrowCpp/crow)
- nlohmann/json for JSON handling
- g++ compiler
- Postman or curl for API testing

---

## 📁 Project Structure

```text
healthcare/
├── main.cpp                # Main Crow server code
├── include/
│   ├── crow.h          # Crow header-only framework (place here)
│   └── json.hpp            # nlohmann JSON header
├── README.md
```

---

## 🚀 Installation & Running

### 1. Clone the repository

```bash
git clone https://github.com/AbdellahSbh/Portfolio_Healthcare_System_by_AbdellahSbh.git
cd Portfolio_Healthcare_System_by_AbdellahSbh
```

### 2. Install dependencies

Download and place the following header files in an `include/` folder:

- `crow.h` from https://github.com/CrowCpp/crow
- `json.hpp` from https://github.com/nlohmann/json

---

### 3. Compile the project

```bash
g++ main.cpp -o server -std=c++17 -pthread
```

---

### 4. Run the server

```bash
./server
```

The server will start on:  
```
http://localhost:18080/
```

---

## 📡 API Routes (Examples)

```text
GET    /patients          → Return all patient data in JSON
POST   /add_patient       → Add new patient (JSON input)
GET    /search_patient    → Search patient by name or ID
```

> Note: The actual routes may vary depending on how you implement them in `main.cpp`.

---

## 📝 Notes

- Crow is a lightweight, header-only framework — no external installation needed.
- All data is stored in memory (not connected to a real database).
- Best tested using Postman or curl for sending/receiving JSON.

---

## 📄 License

This project is developed for academic purposes as part of the Programming Clinic module  
at Lancaster University Leipzig – Michaelmas Term 2025.
