# 🌟 Project Name

Welcome to **Docker-Compose trial**! 🚀 Here we are learning how to use docker compose and writing some installation steps
---

## 🛠️ Manual Installation

### 1️⃣ Install Prerequisites
Make sure you have **Node.js** installed on your system. If not, download and install it from [Node.js official website](https://nodejs.org/en/download). ✅

### 2️⃣ Clone the Repository 🌀
```sh
git clone https://github.com/LOSTBOY-IS-DED/Docker-compose-trail.git
cd projectname
```

### 3️⃣ Install Dependencies 📦
```sh
npm install
```

### 4️⃣ Start the Database Locally 🗄️
#### Option 1: Using Docker 🐳
```sh
docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
```
#### Option 2: Use Neon Tech (Cloud Database) ☁️
- Head over to [Neon Tech](https://neon.tech/) and create a new PostgreSQL database.
- Copy the connection credentials and update your **.env** file.

### 5️⃣ Configure the Environment 🌍
Edit the `.env` file and update the database credentials:
```env
DATABASE_URL=your_database_url_here
```

### 6️⃣ Run Database Migrations & Generate Prisma Client ⚡
```sh
npx prisma migrate dev
npx prisma generate
```

### 7️⃣ Build & Start the Application 🚀
```sh
npm run build
npm run start
```

---

## 🛠️ Docker Installation





## 🛠️ Docker-Compose Installation



## 🎯 You're All Set!
Congratulations! 🎉 Your project is now running. Happy coding! 💻🔥

---

## ❤️ Contributing
Write the installation commands for docker installation and docker-compose. 🤝

---
