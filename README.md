# MockMate AI 🤖💼

Ace Your Tech Interview with AI-Powered Simulations.

**MockMate AI** is an advanced interview simulation platform designed to help job seekers practice technical rounds. By leveraging **Google's Gemini AI**, the application analyzes your resume and the specific job description to generate tailored questions, conducts a real-time voice or text-based interview, and provides instant, scored feedback on your performance.

## 🚀 Key Features

* **📄 Smart Resume Parsing:** Extracts skills and experience from PDF resumes to tailor the difficulty and context of the interview.
* **🎯 Job-Specific Questions:** Generates 5 unique technical questions based on the intersection of your resume and the provided Job Description (JD).
* **🗣️ Voice Mode (Speech-to-Text):** An interactive interview experience where the AI speaks questions and listens to your answers using browser-native Speech Synthesis and Recognition.
* **💬 Chat Mode:** A traditional text-based interface for users who prefer typing.
* **📊 Instant Analysis & Scoring:** Evaluates every answer for confidence, keywords, and technical accuracy, providing a final score and constructive feedback.
* **🎨 Modern UI:** Built with React, Vite, and TailwindCSS featuring glassmorphism effects and smooth animations.

---

## 🛠️ Tech Stack

### Frontend
* **Framework:** [React 19](https://react.dev/) + [Vite](https://vitejs.dev/)
* **Styling:** [TailwindCSS](https://tailwindcss.com/)
* **State Management:** React Context API
* **APIs:** Web Speech API (Synthesis & Recognition)

### Backend
* **Server:** [Flask](https://flask.palletsprojects.com/) (Python)
* **AI Model:** [Google Gemini 2.5 Flash Lite](https://ai.google.dev/)
* **PDF Processing:** PyPDF2
* **Utilities:** Dotenv, Flask-CORS

---

## ⚙️ Installation & Setup

Follow these steps to get the project running on your local machine.

### Prerequisites
* [Node.js](https://nodejs.org/) (v16 or higher)
* [Python](https://www.python.org/) (v3.9 or higher)
* A **Google Gemini API Key** (Get it [here](https://aistudio.google.com/app/apikey))

### 1. Clone the Repository
```bash
git clone [https://github.com/Kush0319/MockMate-AI.git](https://github.com/Kush0319/MockMate-AI.git)
cd MockMate-AI

```

### 2. Backend Setup

Navigate to the backend folder and set up the Python environment.

```bash
cd Backend

# Optional: Create a virtual environment
python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

```

**Configure Environment Variables:**
Create a `.env` file inside the `Backend/` directory and add your API key:

```env
GEMINI_API_KEY=your_actual_api_key_here
PORT=5000

```

Start the Backend server:

```bash
python app.py

```

*The backend should now be running at `http://127.0.0.1:5000`.*

### 3. Frontend Setup

Open a new terminal, navigate to the frontend folder, and install dependencies.

```bash
cd Frontend

# Install node modules
npm install

# Start the development server
npm run dev

```

*The frontend will usually launch at `http://localhost:5173`.*

---

## 📖 How to Use MockMate AI

1. **Launch the App:** Open the frontend URL in your browser (Chrome is recommended for the best Voice API support).
2. **Setup Interview:**
* Enter your **First Name** and **Last Name**.
* **Upload your Resume** (PDF format).
* Paste the **Job Description (JD)** for the role you are targeting.
* Click **Start Interview**.


3. **Choose Mode:**
* **Chat Mode:** Type your answers in a messenger-style interface.
* **Voice Mode:** The AI will speak the question. Click the microphone button to record your answer. Say "Yes" when prompted to begin.


4. **The Interview:** Answer the 5 generated technical questions.
5. **Get Results:** After the final question, the AI analyzes your session and generates a comprehensive score (0-100%) along with specific feedback on your performance.

---

## 📂 Project Structure

```text
mockmate-ai/
├── Backend/
│   ├── app.py                # Main Flask application entry point
│   ├── utils.py              # Helper functions (PDF parsing, Gemini integration)
│   └── requirements.txt      # Python dependencies
│
└── Frontend/
    ├── src/
    │   ├── components/       # Reusable UI components (ChatInterface, SetupForm, etc.)
    │   ├── context/          # React Context (InterviewContext)
    │   ├── services/         # API service configurations
    │   ├── App.jsx           # Main layout manager
    │   └── main.jsx          # DOM entry point
    ├── tailwind.config.js    # Tailwind configuration
    └── vite.config.js        # Vite configuration

```

---

## 👥 The Team

We are passionate developers building the future of AI interviews.

* **Samarth Bhavsar** - *Backend Developer*
* **Kush Bhatt** - *Frontend Developer*

---