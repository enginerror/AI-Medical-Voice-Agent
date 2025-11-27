# 🩺 AI Medical Voice Agent

An AI-powered medical assistant built with **Next.js** that enables real-time, voice-based healthcare interactions. This project simulates a virtual medical assistant capable of understanding patient symptoms through voice, asking intelligent follow-up questions, and responding naturally using AI-driven speech.

## 🚀 Features

- 🎙️ Real-time speech-to-text conversion
- 🤖 AI-driven medical reasoning
- 🗣️ Natural text-to-speech voice responses
- 🔐 Secure user authentication with Clerk
- 🗂️ Persistent data storage using Neon PostgreSQL
- ⚡ High-performance server components
- 📱 Fully responsive modern UI

## 🛠️ Tech Stack

### Frontend

- Next.js (App Router)
- React
- TypeScript
- Tailwind CSS

### Backend & APIs

- AssemblyAI – Speech-to-Text
- OpenAI / LLM API – Medical reasoning
- Murf AI – Text-to-Speech

### Authentication & Database

- Clerk Authentication
- Neon PostgreSQL
- Prisma ORM

### Deployment

- Vercel

## 📁 Project Structure

```bash
ai-medical-agent/
├── app/                # Next.js app router
├── components/         # Reusable UI components
├── lib/                # Helpers & API clients
├── actions/            # Server actions
├── public/             # Static assets
├── prisma/             # Database schema
├── styles/             # Global styles
└── README.md
```

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/ai-medical-voice-agent.git
```

### 2️⃣ Install 

```bash
npm install
```

### 3️⃣ Configure Environment Variables

Create a .env.local file in the root directory

```bash
# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

# Database
DATABASE_URL=your_neon_postgres_url

# AI Services
ASSEMBLYAI_API_KEY=your_assemblyai_api_key
OPENAI_API_KEY=your_openai_api_key
MURF_API_KEY=your_murf_api_key
```

### 4️⃣ Database Migration

```bash
npx prisma migrate dev
```

### 5️⃣ Run the Development Server

```bash
npm run dev
```

## 🧠 Application Flow

1. User signs in securely using **Clerk**
2. User speaks medical symptoms via **microphone**
3. Speech is transcribed using **AssemblyAI**
4. AI analyzes inputs and generates a response
5. Response is converted to speech using **Murf AI**
6. Conversations are stored securely in **Neon Database**

## 🛡️ Medical Disclaimer

⚠️ This application is intended for educational and demonstration purposes only.
It does not provide medical diagnosis or treatment and must not be used as a substitute for professional medical advice.

## 🤝 Contributing

Contributions are always welcome!

1. Fork the repository
2. Create a feature branch  
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes
   ```bash 
   git commit -m "Add feature"
   ```
4. Push to the branch
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request

## 🧪 Testing

```bash
npm run test
```

## 📦 Deployment

```bash
vercel --prod
```

## 📄 License

This project is licensed under the **MIT License**.

## 👨‍💻 Author

Ayaan Murshed Khan

Final Year Computer Science Engineering Student
Full Stack & AI Developer

📎 LinkedIn: https://linkedin.com/in/ayaan-murshed-khan

🌐 Portfolio: https://enginerror.vercel.app

### ⭐ If you find this project helpful, don’t forget to give it a star!
