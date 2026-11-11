<div align="center">

  # ⚜️ Inventory Manager & POS ⚜️
  <div align="right">
  <a href="README.md">🇧🇷 Leia em Português</a>
</div>

<br>

  <p align="center">
    <strong>Cloud-Based Inventory Management, Technical Sheet, and Point of Sale System</strong>
  </p>

  <p align="center">
    <a href="https://conferindoestoque.vercel.app/">
      <img src="https://img.shields.io/badge/Acess_Application-Live_Demo-FF8C00?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
    </a>
  </p>

  <!-- Badges em tons de Preto, Laranja e Dourado -->
  <p align="center">
    <img src="https://img.shields.io/badge/Java-17+-FF8C00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
    <img src="https://img.shields.io/badge/Spring_Boot-3.x-111111?style=for-the-badge&logo=springboot&logoColor=FF8C00" alt="Spring Boot" />
    <img src="https://img.shields.io/badge/Security-JWT-DAA520?style=for-the-badge&logo=jsonwebtokens&logoColor=black" alt="JWT" />
    <img src="https://img.shields.io/badge/PostgreSQL-Neon-FFD700?style=for-the-badge&logo=postgresql&logoColor=black" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/Render-BACKEND-FF8C00?style=for-the-badge&logo=render&logoColor=white" alt="Render Backend" />
    <img src="https://img.shields.io/badge/Vercel-Frontend-000000?style=for-the-badge&logo=vercel&logoColor=DAA520" alt="Vercel" />
  </p>

</div>

## About the Project

The **Inventory Manager & POS** is a fullstack solution developed to automate and optimize the control of supplies, beverages, and final products in food establishments. 

The system automatically calculates product technical sheets, proportionally deducting supplies from inventory with every sale made at the Point of Sale (POS), ensuring operational precision, financial control, and total data security.

---

## 🍔🧡 Main Features

### **Authentication & Profiles**
- **JWT Stateless:** Secure sessions without server-side state storage.

- **Access Recovery:** Password reset flow via a unique Security PIN per user.

- **Data Isolation:** Each account has restricted access exclusively to its own inventory.


### **Inventory & Supplies Management**
- **Base Supplies:** Registration and quantity control by grams, liters, units, etc.

- **Items & Single Beverages:** Independent management with automatic balance updates.

- **Addition Write-offs:** Quick logs for individual stock deductions.


### **Technical Sheet & Recipes**
- **Burger Composition:** Dynamic association of multiple supplies to a single product.

- **Inventory Validation:** Preventive check of raw material availability before recipe registration.


### **Point of Sale (Smart POS)**
- **1-Click Sale:** Agile interface for sales registration.

- **Automatic Proportional Deduction:** When selling a product, all ingredients from its technical sheet are instantly debited from inventory.


---

## Architecture & Technologies

The application follows a decoupled architecture model (**Decoupled SPA + REST API**), ensuring high scalability and low latency:

> 📱 **Frontend (Vercel)**
> `Vanilla JS` • `HTML5 / CSS3`
>
> 🔻 *REST Requests / HTTPS (JWT)*
>
> ⚙️ **Backend (Clever Cloud)**
> `Java 17` • `Spring Boot 3` • `Spring Security`
>
> 🔻 *JDBC Connection / SSL*
>
> 🗄️ **Database (Neon Tech)**
> `PostgreSQL Serverless`

---

## ✨ **[Click to test the site!](https://conferindoestoque.vercel.app/)** ✨

---
## How to Run the Project Locally

If you want to clone this repository and run the project on your machine:

1. Make sure Docker is installed on your system.

2. From the project root, build the Docker image locally:

   ```bash
   docker build -t meu-app-java .
   ```

3. Start the container, mapping the ports:

   ```bash
   docker run -p 8080:8080 meu-app-java
   ```

4. Open your browser and go to: http://localhost:8080

## The CI/CD Pipeline (GitHub Actions)

The automation pipeline was set up to eliminate any manual deployment work. It works like this:

1. **Trigger:** The developer runs `git push` on the main branch (`main`).
2. **Environment:** GitHub Actions starts an isolated virtual machine with `ubuntu-latest`.
3. **Authentication:** The pipeline logs in to Docker Hub using secure credentials (Repository Secrets).
4. **Build & Push:** The Dockerfile is read, the Java code is compiled inside the container, and the final image is pushed to Docker Hub with two tags:

   * `latest` (for the most recent version).
   * A tag with the SHA (unique identifier) of that specific commit, for history.

## Running from the Cloud (Portability)

Thanks to Docker Hub, you don't need to clone this code to run the application. On any server or computer in the world that has Docker installed, just run:

```bash
docker run -d -p 8080:8080 --name meu-servidor-java JustBruder/my-docker:latest
```

* View the app logs:

  ```bash
  docker logs meu-servidor-java
  ```

* Stop the app:

  ```bash
  docker stop meu-servidor-java
  ```

---

### 💻 Contate-me / Let's Connect

<p align="center">
  <a href="https://www.linkedin.com/in/ingrid-bruder" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-C71585?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:ibruder83@gmail.com">
    <img src="https://img.shields.io/badge/Email-C71585?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://www.instagram.com/Cyber.Bruder" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-C71585?style=for-the-badge&logo=instagram&logoColor=white" />
  </a>
  <a href="https://www.tiktok.com/@Cyber.Bruder" target="_blank">
    <img src="https://img.shields.io/badge/TikTok-C71585?style=for-the-badge&logo=tiktok&logoColor=white" />
  </a>
</p>

<div align="center">
  <sub>Developed by Bruder ✨</sub>
</div>
<div align="center">
  <sub>🌷🐱 Clean code and MEOW </sub>
</div>
