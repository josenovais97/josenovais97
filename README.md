<div align="center">
  <img src="header.svg?v=5" width="100%" alt="José Novais Header" />

  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Segoe+UI&weight=600&size=22&pause=1000&color=06B6D4&center=true&vCenter=true&width=600&lines=Full-Stack+Developer;Building+Software+%2B+Hardware+Systems;Based+in+Guimar%C3%A3es%2C+Portugal;If+it+can+be+built%2C+I+want+to+build+it" alt="Typing SVG" />
  </a>
  <br/><br/>
  <a href="https://www.linkedin.com/in/jose-novais97/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:josenovais97@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</div>

---

### 🧠 About Me

- 🎓 **Telecommunications and Informatics Engineering** graduate — University of Minho, Guimarães, Portugal.
- 🌍 Based in **Guimarães, Portugal**.
- 🔭 Currently developing a **full-stack web application with Django** — focusing on REST APIs, robust backend architecture, and data management.
- 🔌 Passionate about the intersection of **software and hardware** — from IoT sensors to the cloud.
- 🛠️ Hands-on with **microcontrollers** (Arduino, ESP8266) and embedded systems.
- ⚙️ Interested in building **scalable systems, real-time architectures, and hardware-integrated platforms**.
- 🌱 Currently deepening my knowledge in **system design, scalability, and distributed systems**.

---

### 🚀 Featured Work

🔒 **Infrastructure Observability Portal (Private)**
- Django + REST API + authentication
- Real-time features using WebSockets with Redis (pub/sub architecture)
- Designed backend architecture, database schema, and production deployment with Nginx + Gunicorn
- Demo available upon request

<details>
<summary><b>👁️ View System Architecture</b></summary>

```mermaid
graph TD
    Browser[🖥️ User Browser] -->|HTTPS - Port 443| Nginx[Nginx]

    subgraph Application
        Nginx -->|HTTP - Port 8000| Gunicorn[Gunicorn\nWSGI]
        Nginx -->|WS - Port 8001| Daphne[Daphne\nASGI]

        Gunicorn --> Django[Django Views]
        Daphne --> Channels[Django Channels\nConsumers]
        Django --> ORM[Django ORM]
        Channels --> ORM
        Django --> Cache[Redis Cache\nDedup · Analytics · Templates]
        Django --> SMTP[Gmail SMTP\nAlert emails]
        Django --> Hooks[Outbound Webhooks\nHMAC-SHA256 signed]
    end

    subgraph Persistence
        ORM --> DB[(MariaDB\nnonius_db)]
        Channels --> RedisChannels[(Redis\nChannel Layer)]
    end

    subgraph Fleet
        Django --> SSH[Paramiko SSH\nAgentless]
        Channels --> SSH
        SSH --> IS1[IS Server 1]
        SSH --> IS2[IS Server 2]
        SSH --> ISN[IS Server N]
    end
```

</details>
<br/>

🔌 **[NEXCAR: IoT Vehicle Monitoring System](https://github.com/josenovais97/NEXCAR-Real-Time-IoT-Vehicle-Control-and-Monitoring-Platform)**
- ESP8266 + MQTT communication
- Real-time data ingestion and backend integration
- Designed for scalable, low-latency communication using MQTT and real-time messaging
  
---

### 🛠️ Languages & Tools

**Backend & Web**
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white"/>
  <img src="https://img.shields.io/badge/Django%20REST-ff1709?style=for-the-badge&logo=django&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/HTMX-336699?style=for-the-badge&logo=htmx&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white"/>
</p>

**Real-Time & Infrastructure**
<p align="left">
  <img src="https://img.shields.io/badge/WebSockets-010101?style=for-the-badge&logo=socket.io&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge&logo=gunicorn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
</p>

**Systems & Embedded**
<p align="left">
  <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black"/>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white"/>
  <img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white"/>
  <img src="https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
</p>

---

### 📊 GitHub Stats

<div align="center">
  <img src="https://streak-stats.demolab.com?user=josenovais97&theme=tokyonight&hide_border=true" alt="GitHub Streak" height="170"/>
  
  <img src="https://github-readme-stats-iota-peach-9codjpiahv.vercel.app/api/top-langs/?username=josenovais97&layout=compact&theme=tokyonight&hide_border=true&v=1" alt="Top Languages" height="170"/>
</div>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,100:4F46E5&height=100&section=footer&text=Let's%20build%20something%20great!&fontSize=20&fontColor=ffffff&fontAlignY=65" width="100%"/>
</div>
