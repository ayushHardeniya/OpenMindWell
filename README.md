# OpenMindWell 🌱

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![Built by](https://img.shields.io/badge/Built%20by-Team%20ZenYukti-purple)

**A compassionate, AI-powered mental health support platform**

> ⚠️ **IMPORTANT DISCLAIMER**: OpenMindWell is NOT a substitute for professional mental health care. If you are in crisis, please contact emergency services or a crisis hotline immediately.

## 🌟 Features

- **Anonymous Chat Rooms** - Join peer support groups without revealing identity
- **AI Crisis Detection** - Automatic detection of concerning messages with resource suggestions
- **Private Journaling** - Track mood, thoughts, and personal reflections
- **Habit Tracking** - Build positive daily habits with streak tracking
- **Resource Library** - Curated mental health resources, hotlines, and exercises
- **Volunteer Moderation** - Community-driven safety and support

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Supabase account (free tier)
- HuggingFace account (free tier)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/OpenMindWell.git
cd OpenMindWell
```

2. **Install dependencies**
```bash
npm install
cd backend && npm install && cd ..
cd frontend && npm install && cd ..
```

3. **Set up Supabase**
   - Create a free account at [supabase.com](https://supabase.com)
   - Create a new project
   - Go to SQL Editor and run `database/schema.sql`
   - Enable Anonymous authentication: Authentication → Providers → Anonymous (toggle ON)
   - Disable CAPTCHA for development: Authentication → Settings → Disable CAPTCHA

4. **Configure environment variables**

**Backend** (`backend/.env`):
```env
SUPABASE_URL=your_supabase_project_url
SUPABASE_ANON_KEY=your_anon_key
SUPABASE_SERVICE_KEY=your_service_role_key
HUGGINGFACE_API_KEY=your_hf_token
FRONTEND_URL=http://localhost:3000
PORT=3001
```

**Frontend** (`frontend/.env.local`):
```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_anon_key
NEXT_PUBLIC_API_URL=http://localhost:3001
```

5. **Get API keys**
   - **Supabase**: Project Settings → API (URL, anon key, service_role key)
   - **HuggingFace**: [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens) → New Token (Read access)

6. **Run the application**
```bash
# From root directory
npm run dev
```

- Frontend: http://localhost:3000
- Backend: http://localhost:3001

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/openmindwell.git
cd openmindwell

# Install dependencies
npm install

# Set up environment variables
cp backend/.env.example backend/.env
cp frontend/.env.local.example frontend/.env.local
# Edit .env files with your credentials

# Run both servers
npm run dev
```

Visit http://localhost:3000

## 📚 Documentation

**READ THIS FIRST:** [OPENMINDWELL_PROJECT_GUIDE.md](./OPENMINDWELL_PROJECT_GUIDE.md)

This comprehensive guide contains:
- Complete setup instructions
- Free service account creation
- Deployment guides
- Security considerations
- Contribution guidelines

## 🛠️ Tech Stack

**100% Free Services:**
- **Frontend**: Next.js 14, React, TypeScript, Tailwind CSS → Vercel
- **Backend**: Node.js, Express, WebSocket, TypeScript → Render/Railway
- **Database**: Supabase (PostgreSQL + Auth)
- **AI**: HuggingFace Inference API (emotion detection)

## 📁 Project Structure

```
openmindwell/
├── backend/           # Express API + WebSocket server
├── frontend/          # Next.js application
├── OPENMINDWELL_PROJECT_GUIDE.md
├── CONTRIBUTING.md
└── package.json       # Monorepo scripts
```

## 🔒 Safety Features

- Prominent crisis disclaimers throughout the app
- AI-powered crisis detection on all messages
- Automatic resource suggestions
- User reporting and moderation system
- Anonymous/pseudonymous accounts only
- Row-level security on all data

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

Perfect for:
- 🎓 GSoC, Hacktoberfest, WoC programs
- 💼 Portfolio projects
- 🌍 Making a social impact

## 📞 Crisis Resources

**If you're in crisis:**
- 🇺🇸 **988 Suicide & Crisis Lifeline**: Call/Text 988
- 🇺🇸 **Crisis Text Line**: Text HOME to 741741
- 🌍 **International**: findahelpline.com

## 📄 License

MIT License - See [LICENSE](./LICENSE) for details

## ⚠️ Ethical Use

This platform is designed to:
- ✅ Provide peer support and community
- ✅ Share coping strategies and resources
- ✅ Reduce stigma around mental health

This platform is NOT:
- ❌ A replacement for therapy or medical treatment
- ❌ Qualified to diagnose or treat mental health conditions
- ❌ A crisis intervention service

---

## 🤝 Contributing

We welcome contributions from the community! OpenMindWell is built with the mission to make mental health support accessible to everyone.

**Ways to Contribute:**
- 🐛 Report bugs and issues
- 💡 Suggest new features
- 🔧 Submit pull requests
- 📖 Improve documentation
- 🌍 Translate to other languages

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

**Built with 💙 for mental wellness by Team ZenYukti**

*Remember: Seeking professional help is a sign of strength, not weakness.*
