# tinyRedis
![Go Version](https://img.shields.io/badge/Go-1.22+-blue)
![Contributions](https://img.shields.io/badge/contributions-welcome-brightgreen)

![tinyRedis Logo](logo.png)

**tinyRedis** is a minimalistic Redis server clone written in Go. This project is lightweight, efficient, and fully compatible with the Redis protocol, making it ideal for **educational purposes**.

> ⚠️ **Disclaimer:** tinyRedis is intended as a learning tool. It is not production-ready and may lack advanced features and security guarantees of Redis.

---

## 📖 Table of Contents
- [Features](#-features)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [Examples](#-examples)
- [Comparison with Redis](#-comparison-with-redis)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)

---

## ⚡ Features
- **Redis Protocol Compatibility**: Works with standard Redis clients.
- **Lightweight Design**: Core functionality with minimal overhead.
- **Written in Go**: Uses Go's concurrency model for efficient multi-connection handling.
- **Educational**: Great for understanding how a key-value store works internally.

---

## 🚀 Getting Started

### Prerequisites
- Install [Go 1.22+](https://go.dev/dl/)

### Installation
```bash
git clone https://github.com/robitec97/tinyRedis.git
cd tinyRedis
go run main.go
```

---

## 🛠 Usage

Start the server:
```bash
go run main.go
```

Connect with `redis-cli`:
```bash
redis-cli -p 6379
```

---

## 📊 Examples
```bash
SET hello world
OK
GET hello
"world"
```
---

## 🔎 Comparison with Redis

| Feature         | Redis | tinyRedis |
|-----------------|-------|-----------|
| SET/GET         | ✅    | ✅        |
| DEL             | ✅    | ✅        |
| AOF Persistence | ✅    | ✅ (basic) |
| Pub/Sub         | ✅    | ❌        |
| Clustering      | ✅    | ❌        |

---

## 🛣 Roadmap
- [ ] Improve persistence reliability
- [ ] Implement Pub/Sub
- [ ] Add support for transactions
- [ ] Add clustering support

---

## 🤝 Contributing
Contributions, issues, and feature requests are welcome!

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License
This project is licensed under the Apache License 2.0.  
You are free to use, modify, and share this project, but you must give **appropriate credit** to the original author [robitec97](https://github.com/robitec97).
