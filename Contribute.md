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

Here’s your **README.md** file with the complete Docker installation guide. 🚀  

I'll format it properly so you can copy-paste it directly into your **README.md** file.  

---

```md
# 🌟 Project Name

Welcome to **Docker-Compose Trial**! 🚀 This guide will help you install Docker, set up PostgreSQL, and run your project inside a Docker container.  

---

## 🛠️ Docker Installation  

Follow these steps to install Docker on your system.  

### 🐧 Install Docker on Linux (Ubuntu/Debian)  
```sh
sudo apt update
sudo apt install -y docker.io
sudo systemctl start docker
sudo systemctl enable docker
```
Verify installation:  
```sh
docker --version
```

### 🍏 Install Docker on macOS  
1. Download **Docker Desktop** from [Docker’s official website](https://docs.docker.com/desktop/setup/install/mac-install/).  
2. Install it and follow the setup instructions.  
3. Run Docker Desktop and ensure it's running.  
4. Verify installation:  
   ```sh
   docker --version
   ```

### 🖥️ Install Docker on Windows  
1. Download **Docker Desktop** from [Docker’s official website](https://docs.docker.com/desktop/setup/install/windows-install/).  
2. Install and restart your system if required.  
3. Open Docker Desktop and ensure it's running.  
4. Verify installation:  
   ```sh
   docker --version
   ```

---
## 🛠️ Using Docker to Run PostgreSQL  

Once Docker is installed, start a PostgreSQL container:  
```sh
docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
```
This will:  
✅ Run PostgreSQL in a container.  
✅ Expose it on port `5432`.  
✅ Set the password to `mysecretpassword`.  

---

## 🛠️ Build & Run the Application with Docker  

### 1️⃣ Build the Docker Image 🏗️  
Run the following command inside your project directory:  
```sh
docker build -t my-app .
```

### 2️⃣ Start the Docker Container 🚀  
```sh
docker run -p 3000:3000 my-app
```
Now your application should be running inside a Docker container on port `3000`. 🎉

---

## 🛠️ Docker-Compose Installation

Install docker and docker compose 

Run
```sh
docker compose up
```



## ❤️ Contributing
Write the installation commands for docker and docker compose ...

---
