# 🤖 Robotics & Engineering Skill Frequency Tracker

A minimalist, high-fidelity web dashboard engineered for roboticists and developers to track tech stack demand dynamically. By compiling and parsing industry job descriptions, this tool aggregates keyword frequencies across custom categories, providing data-driven insight into exactly which competencies to prioritize in your portfolio or resume.

---

## 🚀 Key Features

- **Granular Skill Domains:** Organizes your tracking data into preconfigured categories (Programming Languages, Tools & Frameworks, Simulation Programs, Concepts & Methods, and Preferences/Notices).
- **Persistent Distributed Backing:** Scaled instantly over a real-time, zero-latency Firebase sync layer mapping securely to your authenticated Google credentials.
- **Bi-Modal Skill Extraction Parsing Engine:**
  - **Local Substring Engine:** Parses your text inputs instantly via strict word-boundary regular expressions matching against existing data models.
  - **Groq AI-Driven Extraction Matrix:** Utilizes state-of-the-art open-source LLMs (`llama-3.3-70b-versatile`) to read deep context, identifying semantic variants of active skill matrices and automatically extracting entirely new technical concepts hidden in the job descriptions.

---

## 📈 Getting the Most Benefit From Your Tracker

To build a truly data-driven roadmap for your technical progression, use the following framework:

1. **Targeting an Industry Sector:** Choose 15–20 high-value job openings matching your desired next role (e.g., *Autonomous Navigation Engineer*, *Robotics Software Architect*, *Controls Intern*).
2. **Systematically log positions:** Paste descriptions directly from LinkedIn, Indeed, or company boards into the **Add Job** section.
3. **Analyze & Adapt:** Watch the frequency bars rise. If a tool you don't know (e.g., `EtherCAT`, `Nav2`, or `Docker`) appears across more than 40% of logged vacancies, it represents an immediate gap in your skill stack.
4. **Tailor Your Applications:** Use the generated metric chart to organize your resume. Place the highest frequency tools prominently at the top of your qualifications layout.

---

## 🔑 AI Deep Scan Setup (Adding your Groq API Key)

To unlock automated extraction of *untracked/new skills*, the application securely invokes a Groq AI processing endpoint. This occurs entirely client-side; **your key is never sent to a shared database and remains safely inside your browser's private local storage sandbox layer.**

### Step 1: Secure a Free Groq API Key
1. Navigate to the official developer workspace at **[Groq Console](https://console.groq.com/)**.
2. Sign up or log in using an email address or a developer profile connection.
3. Navigate to the left-hand menu section named **API Keys**.
4. Click **Create API Key**, name it appropriately (e.g., `Robotics Skill Tracker`), and copy the produced key token (it will begin with `gsk_...`).

### Step 2: Inject the Credentials into Your App Dashboard
1. Open your hosted Skill Tracker application in your browser.
2. Click the **⚙ Settings** button in the top navigation panel.
3. Paste the full `gsk_...` key token into the secure password prompt text field.
4. Click **Done**. Your application will now immediately invoke deep structural scanning capabilities every time you select **Find Skills** on a job description text segment.

---

## 🛠 Tech Stack & Architecture

- **Runtime Viewport:** React 18 & `htm` (Lightweight Virtual DOM without an external bundler/node build phase step).
- **Styling Architecture:** Tailwind CSS utility frameworks paired with custom dark-palette variables (`#0F1419`).
- **Database Architecture:** Firebase JS SDK (v10) connecting direct Authentication state objects down to Firestore Document paths mapped by user UID (`/dashboards/{share_code}`).
- **Inference Pipeline Engine:** Groq Developer SDK REST endpoint wrapper applying forced structural dynamic JSON outputs handling schema arrays validation workflows.
  ---
---

## Author

**Omar Desoky**
Mechatronics & Robotics Engineering — Egypt-Japan University of Science and Technology (E-JUST)

[![GitHub](https://img.shields.io/badge/GitHub-desoky5-181717?logo=github)](https://github.com/desoky5)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin)](https://www.linkedin.com/in/omardesoky5/)

---

## License

This project is open source. See [LICENSE](LICENSE) for details.
