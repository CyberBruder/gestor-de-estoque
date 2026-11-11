<div align="center">

  # ⚜️ Inventory Manager & POS ⚜️

  <p align="center">
    <strong>Cloud-Based Inventory Management, Technical Sheet, and Point of Sale System</strong>
  </p>

  <p align="center">
    <a href="https://conferindoestoque.vercel.app/">
      <img src="https://img.shields.io/badge/Acessar_Aplicação-Live_Demo-FF8C00?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
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

<hr />

🇧🇷 [Leia em português](README.md)

<hr />

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

<div align="center">

### 💻 Contate-me / Let's Connect

<p align="center">
  <a href="https://www.linkedin.com/in/ingrid-bruder" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-C71585?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:ibruder83@gmail.com">
    <img src="https://img.shields.io/badge/Email-C71585?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>
</div>

<div align="center">
  <sub>Desenvolvido por JustBruder ✨</sub>
</div>
<div align="center">
  <sub>🌷 Security by Design </sub>
</div>
