# Docker 

## 1️⃣ What is Virtualization?
**Virtualization** means running **multiple operating systems on one physical computer**.

### Example
- One laptop  
- Runs **Windows + Linux** at the same time  
- Each OS thinks it has its own computer  

This is done using a **Virtual Machine (VM)**.

### Key points
- Uses a **Hypervisor**
- Each VM has:
  - Full OS
  - Own memory
  - Own CPU share

⚠️ **Problem**: Heavy, slow, high resource usage

---

## 2️⃣ What is a Virtual Machine (VM)?
A **Virtual Machine** is a **software-based computer**.

### Structure
- Hardware
- Hypervisor
- Guest OS (Linux / Windows)
- App + Dependencies

### Drawback
- Needs **full OS**
- Takes **minutes to start**
- Eats **RAM & CPU**

---

## 3️⃣ What is Containerization?
**Containerization** runs applications in **isolated environments**  
👉 WITHOUT installing a full OS for each app.

- Shares the **host OS kernel**
- Only app + required libraries are packed

---

## 4️⃣ What is Docker?
**:contentReference[oaicite:0]{index=0}** is a tool that helps you:
- Build
- Ship
- Run applications  
using **containers**

📦 Think of Docker as a **box** that contains:
- App
- Libraries
- Dependencies
- Config files

Runs the same everywhere.

---

## 5️⃣ Virtual Machine vs Docker Container


::contentReference[oaicite:1]{index=1}


| Feature | Virtual Machine | Docker Container |
|------|----------------|-----------------|
| OS | Full OS | Uses host OS |
| Size | GBs | MBs |
| Speed | Slow | Very fast |
| Boot time | Minutes | Seconds |
| Resource use | High | Low |

---

## 6️⃣ Why Docker?
Docker solves the **“works on my machine”** problem.

### Without Docker
- App works on dev laptop
- Fails on testing
- Breaks in production

### With Docker
- Same container everywhere
- No environment issues

---

## 7️⃣ What did developers use BEFORE Docker?
Before Docker, devs used:

### 1. Manual Setup
- Install Java
- Install DB
- Configure ports
- Fix version conflicts  
❌ Error-prone

### 2. Virtual Machines
- Heavy
- Slow
- Hard to scale

### 3. Configuration Tools
- Ansible
- Puppet  
❌ Complex & time-consuming

---

## 8️⃣ Docker Image
A **Docker Image** is a **blueprint**.

- Read-only
- Contains app + dependencies
- Used to create containers

👉 Example:
- Image = Recipe
- Container = Cooked food

---

## 9️⃣ Docker Container
A **Docker Container** is a **running instance of an image**.

- Lightweight
- Fast
- Isolated
- Can be started/stopped anytime

---

## 🔟 Dockerfile
A **Dockerfile** is a **text file** with instructions.

Example:
- Base OS
- Install dependencies
- Copy code
- Start app

Docker uses it to build images.

---

## 1️⃣1️⃣ Docker Engine
Docker Engine is the **core service** that:
- Builds images
- Runs containers
- Manages networking & storage

---

## 1️⃣2️⃣ Docker Hub
**:contentReference[oaicite:2]{index=2}** is:
- Online repository for images
- Like GitHub but for Docker images

---

## 1️⃣3️⃣ Real-World Example
### Without Docker
- Dev: Node 18
- QA: Node 16
- Prod: Node 14  
❌ App breaks

### With Docker
- Node version inside container
- Same everywhere  
✅ No mismatch

---

## 🧠 One-Line Summary
> Docker lets you run applications **anywhere**, **fast**, and **without environment problems** using containers.

---
