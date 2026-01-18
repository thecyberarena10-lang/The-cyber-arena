 🛡️ The Cyber Arena

The Cyber Arena is a custom-built Capture The Flag (CTF) platform designed to test and recruit potential teammates for hackathons. It features a 3-stage challenge system, a real-time dashboard, and an automated email notification system for successful candidates.

Live Demo: [Insert your Render link here, e.g., https://cyber-arena.onrender.com]

 🚀 Features

* **Interactive Dashboard:** Users can track their progress through 3 distinct stages.
* **3-Tier Challenge System:**
    * **Stage 1 (Web):** Tests HTML inspection and basic logic.
    * **Stage 2 (Scripting):** Tests Python/Bash automation skills.
    * **Stage 3 (System):** Tests Linux privileges and file analysis.
* **Automated Recruitment:** Upon completing all stages, the system automatically triggers an SMTP email via the Backend to welcome the user to the team.
* **Secure Authentication:** User registration and login system with hashed passwords.


 🛠️ Tech Stack

This project was built using a **Zero-Cost Architecture**:

* **Backend:** Python (Flask)
* **Frontend:** HTML5, CSS3, Jinja2 Templating
* **Database:** PostgreSQL (Neon.tech) / SQLite (Local)
* **Automation:** Python `smtplib` (Gmail API)
* **Hosting:** Render (Web Service)


 📂 Project Architecture

The application follows a Model-View-Controller (MVC) pattern:

1.  **The Interface:** Static HTML/CSS pages served via Flask.
2.  **The Logic:** Python routes handle flag verification (`/submit-flag`) and database updates.
3.  **The Trigger:** A backend check runs after every submission. If `progress == 100%`, the `send_congratulations_email()` function is executed.

---

## ⚙️ Installation & Local Setup

To run this project locally on your machine:

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/your-username/the-cyber-arena.git](https://github.com/your-username/the-cyber-arena.git)
    cd the-cyber-arena
    ```

2.  **Create a Virtual Environment**
    ```bash
    python -m venv venv
    # Windows
    venv\Scripts\activate
    # Mac/Linux
    source venv/bin/activate
    ```

3.  **Install
