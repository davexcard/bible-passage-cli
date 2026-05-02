# 📖 Bible Passage CLI (Go)

A simple command-line application written in Go to search, read, and save Bible passages.

This project is designed as a backend-focused learning exercise, with an emphasis on clean architecture, API consumption, and data persistence.

---

## 🚀 Features

### ✅ MVP

* Search Bible passages by reference (e.g., `John 3:16`)
* Search by keyword (e.g., `love`, `faith`)
* Display passage text in the terminal
* Save favorite passages locally
* View saved favorites

### 🔜 Future Improvements

* Add tags/categories to passages
* Personal notes for each passage
* Filter by book or testament
* Daily reading feature
* REST API version
* Simple web interface

---

## 🛠️ Tech Stack

* Language: Go (Golang)
* CLI: Standard library or Cobra (optional)
* Storage: JSON file or SQLite
* API: Public Bible API

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/bible-cli.git
cd bible-cli
```

### 2. Initialize Go modules

```bash
go mod init github.com/your-username/bible-cli
go mod tidy
```

### 3. Build the project

```bash
go build -o bible-cli ./cmd
```

---

## ▶️ Usage

### Search by reference

```bash
./bible-cli search "John 3:16"
```

### Search by keyword

```bash
./bible-cli search "love"
```

### Save a passage to favorites

```bash
./bible-cli save "John 3:16"
```

### View favorites

```bash
./bible-cli favorites
```

---

## 🧠 Project Structure

```
bible-cli/
│
├── cmd/                # CLI entry point
│   └── root.go
│
├── internal/
│   ├── api/            # External Bible API integration
│   ├── storage/        # File or DB handling
│   ├── services/       # Business logic
│
├── data/               # Local storage (JSON/SQLite)
├── main.go
├── go.mod
├── README.md
```

---

## 🌐 Data Source

You can use a free public Bible API:

* https://bible-api.com/
* https://scripture.api.bible/

Example request:

```
https://bible-api.com/john%203:16
```

---

## 🎯 Learning Goals

* Build a real CLI application in Go
* Practice HTTP requests and JSON parsing
* Implement local data persistence
* Structure a project using clean architecture principles
* Prepare for backend and DevOps workflows

---

## 📌 Notes

* Keep the scope small (20–40 hours max)
* Focus on functionality over complexity
* Write meaningful commit messages
* Document your decisions as you build

---

## 📄 License

This project is licensed under the MIT License.
