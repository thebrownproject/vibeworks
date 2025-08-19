# 🏗️ VibeWorks

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Next.js](https://img.shields.io/badge/Next.js-14+-black.svg)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue.svg)](https://www.typescriptlang.org/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-green.svg)](https://supabase.com/)
[![AI Powered](https://img.shields.io/badge/AI-Gemini%202.5%20Pro-orange.svg)](https://ai.google.dev/)

> **AI-Powered Project Management for Architecture Offices** - Transforming "vibes-based" project management into systematic, data-informed planning while respecting familiar workflows.

---

## 📋 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [💡 The Problem](#-the-problem)
- [✨ Our Solution](#-our-solution)
- [🚀 Key Features](#-key-features)
- [🛠️ Technology Stack](#️-technology-stack)
- [📱 Live Demo](#-live-demo)
- [⚡ Quick Start](#-quick-start)
- [📁 Project Structure](#-project-structure)
- [🧪 Development](#-development)
- [🚀 Deployment](#-deployment)
- [🎨 Screenshots](#-screenshots)
- [📊 Impact & Validation](#-impact--validation)
- [🧑‍💻 Career Transition Story](#-career-transition-story)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🎯 Project Overview

VibeWorks is an AI-powered project management system designed specifically for architecture offices. Born from real workplace challenges, it transforms the typical "vibes-based" project management approach into systematic, data-informed planning while maintaining the familiar workflows that architects already understand.

**Dual Purpose:**
- **🏢 Workplace Solution**: Actively solving project management challenges at a Victorian architecture office
- **💼 Portfolio Demonstration**: Showcasing modern full-stack development skills during Fraser Brown's transition from architecture to IT

**Real-World Validation**: Unlike theoretical portfolio projects, VibeWorks is validated through actual workplace implementation, user adoption, and measurable productivity improvements.

---

## 💡 The Problem

Architecture offices across Victoria operate with "vibes-based" project management that creates significant operational challenges:

### 🚨 Critical Pain Points
- **📞 Documentation Gap**: Verbal requests and phone calls create undocumented urgent work
- **👥 Visibility Crisis**: Management lacks real-time insight into "hours to next stage"
- **📈 Forecasting Impossibility**: Capacity planning relies on guesswork without systematic time tracking
- **🔧 Tool Resistance**: Previous attempts with platforms like Notion failed due to complexity

### 📊 Quantified Impact
- Projects consistently delayed due to urgent interruptions, not poor estimates
- Monday morning capacity assessment requires manual polling of staff
- Communication gaps occur when phone calls bypass documentation systems
- Stressed staff avoid updating systems during busy periods

---

## ✨ Our Solution

VibeWorks addresses these challenges through a streamlined digital whiteboard that replicates the physical office organization, enhanced by AI assistance for rapid task capture.

### 🎯 Core Concept
- **📋 Digital Whiteboard Replica**: Mirrors existing physical whiteboard with zero learning curve
- **🤖 AI Chat Overlay**: Simple chatbot for 30-second task creation and project queries
- **⚡ Essential Features Only**: Focused on core workflow needs without feature bloat

### 🏗️ Familiar Organization
**5-Section Digital Whiteboard:**
- **Town Planning** - Early stage regular projects
- **Working Drawings** - Documentation stage regular projects
- **Harnest TP** - Harnest client town planning projects
- **Harnest WD** - Harnest client working drawings projects
- **Commercial Shop Fitouts** - All shop fitout projects

---

## 🚀 Key Features

### 🤖 AI-Powered Task Management
- **Email Processing**: Copy-paste emails for instant task extraction
- **Project Identification**: AI identifies relevant projects and suggests assignments
- **Time Estimation**: Smart estimates based on project stage and historical data

### 📊 7-Stage Project Lifecycle
- **Concept Design** → **Schematic Design** → **Design Development**
- **Construction Documentation** → **Building Permit** → **Tender Documentation** → **Final Working Drawings**
- Real-time "hours to next stage" visibility

### 🎨 CAD-Familiar Interface
- **Ribbon-style Navigation**: Familiar patterns matching Revit/AutoCAD
- **Properties Panels**: Project cards with intuitive organization
- **Reduced Resistance**: Zero learning curve for CAD-comfortable staff

### ⏰ Monday Morning Dashboard
- **Real-time Capacity**: Instant visibility into staff availability
- **Project Status**: Complete overview of all active projects
- **Management Insights**: Eliminates manual polling and guesswork

---

## 🛠️ Technology Stack

### 🎨 Frontend Excellence
- **⚛️ Next.js 14**: App Router with server-side rendering and performance optimization
- **📘 TypeScript**: Type safety and modern development patterns
- **🎨 Shadcn/ui + Tailwind CSS**: Accessible component design system
- **🔄 Zustand**: Lightweight state management

### 🔧 Backend & Services
- **🗄️ Supabase PostgreSQL**: Database with Row Level Security
- **🔐 Supabase Auth**: Authentication and session management
- **⚡ Supabase Real-time**: Collaborative features and live updates
- **🤖 Vercel AI SDK**: AI integration framework
- **🧠 Google Gemini 2.5 Pro**: AI processing and natural language understanding

### 🚀 Development & Deployment
- **☁️ Vercel**: Hosting and serverless functions
- **🧪 Vitest**: Unit testing framework
- **🎭 Playwright**: End-to-end testing
- **✅ ESLint + Prettier**: Code quality and formatting

---

## 📱 Live Demo

🔗 **[View Live Application](https://vibeworks.vercel.app)** *(Coming Soon)*

*Current Status: MVP Development Phase - Workplace testing in progress*

---

## ⚡ Quick Start

### Prerequisites
- Node.js 18+ with npm
- Supabase CLI for local development
- Git for version control

### Installation

```bash
# Clone the repository
git clone https://github.com/thebrownproject/vibeworks.git
cd vibeworks

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env.local
# Edit .env.local with your Supabase and AI API keys

# Initialize Supabase
npx supabase init
npx supabase start

# Start development server
npm run dev
```

### Environment Variables

```bash
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
GOOGLE_AI_API_KEY=your_gemini_api_key
```

---

## 📁 Project Structure

```
vibeworks/
├── 📄 README.md                    # This file
├── 📋 CLAUDE.md                    # Claude Code project instructions
├── 📦 package.json                 # Dependencies and scripts
├── 📂 src/
│   ├── 📱 app/                     # Next.js App Router
│   │   ├── 🔌 api/                # API routes (projects, tasks, ai/chat)
│   │   ├── 📋 project-board/      # Main whiteboard page
│   │   ├── ✅ task-board/         # Cross-project task view
│   │   ├── 👥 staff-allocation/   # Staff capacity page
│   │   └── 🎨 layout.tsx          # Root layout with sidebar navigation
│   ├── 🧩 components/
│   │   ├── 🎨 ui/                 # Shadcn/ui base components
│   │   ├── 📋 project-board/      # Whiteboard section components
│   │   ├── 🖼️ modals/            # Project/task detail modals
│   │   ├── 🤖 ai-chat/           # AI chat overlay
│   │   └── 🔄 common/            # Shared components
│   ├── 🗃️ stores/                # Zustand state management
│   ├── 📚 lib/                    # API clients and utilities
│   ├── 📝 types/                  # TypeScript definitions
│   └── 🎣 hooks/                  # Custom React hooks
├── 🗄️ supabase/                  # Database migrations and schemas
├── 📖 docs/                       # Project documentation
├── 🖼️ public/                    # Static assets
└── ⚙️ claude-configs/             # Claude Code configurations
```

---

## 🧪 Development

### Available Scripts

```bash
# Development
npm run dev              # Start development server
npm run build           # Build for production
npm run start           # Start production server

# Code Quality
npm run lint            # Run ESLint
npm run type-check      # Run TypeScript compiler

# Database
npx supabase start      # Start local Supabase
npx supabase db reset   # Reset local database
npx supabase db push    # Push schema changes

# Testing
npm run test            # Run unit tests
npm run test:e2e        # Run Playwright tests
npm run test:watch      # Run tests in watch mode
```

### Development Workflow

1. **Feature Development**: Create feature branch from `main`
2. **Local Testing**: Use local Supabase instance for development
3. **Code Quality**: ESLint and TypeScript strict mode compliance
4. **Testing**: Unit and integration tests required
5. **Pull Request**: Code review and automated testing
6. **Deployment**: Automatic deployment via Vercel

---

## 🚀 Deployment

### Production Environment
- **Hosting**: Vercel with automatic deployments from `main` branch
- **Database**: Supabase managed PostgreSQL with Sydney region
- **Domain**: Custom domain with SSL certificate
- **Monitoring**: Vercel Analytics and Supabase dashboard

### Environment Configuration
- **Development**: `localhost:3000` with local Supabase
- **Production**: `vibeworks.vercel.app` with production Supabase
- **Environment Variables**: Managed through Vercel dashboard

---

## 🎨 Screenshots

*Screenshots coming soon as MVP development progresses*

### 📋 Digital Whiteboard
*Main interface showing the 5-section project organization*

### 🤖 AI Chat Interface
*Simple overlay for rapid task creation and project queries*

### 📊 Monday Morning Dashboard
*Real-time capacity and project status overview*

---

## 📊 Impact & Validation

### 🎯 Workplace Success Metrics
- **📈 Target Adoption**: 80% of colleagues using daily within first month
- **⏰ Efficiency Goal**: Reduce Monday planning from 30+ to 12 minutes
- **📝 Capture Rate**: 90% of urgent interruptions systematically documented
- **⚡ Speed Requirement**: Task capture under 30 seconds during high-pressure periods

### 🏢 Real-World Validation
- **👥 User Base**: 8-12 professional architects and designers
- **📍 Location**: Victorian architecture office (Fraser's current workplace)
- **🔄 Feedback Loop**: Direct access for user research and iterative improvement
- **📊 Metrics**: Sustained usage over 3+ months demonstrating lasting value

### 💼 Portfolio Impact
- **🎯 Technical Demonstration**: Modern React/TypeScript/Supabase implementation
- **🤝 User-Centered Design**: Real user feedback and adoption evidence
- **📈 Business Value**: Quantifiable productivity improvements
- **🌟 Professional References**: Supervisor and colleague testimonials

---

## 🧑‍💻 Career Transition Story

### 🏗️ Architecture → 💻 IT

**Fraser Brown** is transitioning from architecture to IT, leveraging domain expertise to create practical software solutions. VibeWorks represents the culmination of this journey - applying newly acquired programming skills to solve real workplace challenges.

### 🎯 Why This Project Matters

**Domain Expertise Application:**
- Deep understanding of architecture office workflows and pain points
- Translation of industry-specific challenges into technical requirements
- User experience design informed by CAD software familiarity

**Technical Skills Demonstration:**
- Modern full-stack development with React, TypeScript, and Supabase
- AI integration and natural language processing
- Database design reflecting complex project relationships
- Professional development practices and deployment automation

**Real-World Problem Solving:**
- Genuine workplace challenges with measurable business impact
- User research and iterative development with actual colleagues
- Change management and technology adoption in professional environment

### 🚀 Portfolio Differentiation

Unlike bootcamp projects or tutorials, VibeWorks demonstrates:
- **🎯 Practical Problem Solving**: Real workplace inefficiencies with measurable solutions
- **👥 User-Centered Development**: Authentic user feedback and adoption validation
- **🏢 Business Value Creation**: Quantifiable productivity improvements and supervisor endorsement
- **🔄 Industry Knowledge Transfer**: Architecture expertise applied to software development

---

## 🤝 Contributing

We welcome contributions to improve VibeWorks! This project serves both as a practical workplace solution and a portfolio demonstration.

### 🛠️ Areas for Contribution
- **🎨 UI/UX Improvements**: Enhance the CAD-familiar interface patterns
- **🤖 AI Features**: Improve email processing accuracy and task extraction
- **📊 Analytics**: Better capacity planning and productivity metrics
- **🧪 Testing**: Expand test coverage and end-to-end scenarios
- **📖 Documentation**: Improve setup guides and architecture documentation

### 📝 How to Contribute

1. **🍴 Fork** the repository
2. **🌿 Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **✅ Test** your changes thoroughly
4. **💬 Commit** with clear messages (`git commit -m 'Add amazing feature'`)
5. **🚀 Push** to your branch (`git push origin feature/amazing-feature`)
6. **📝 Open** a Pull Request with detailed description

### 🐛 Reporting Issues

Found a bug or have a suggestion? [Open an issue](https://github.com/thebrownproject/vibeworks/issues) with:
- Clear description of the problem or enhancement
- Steps to reproduce (for bugs)
- Expected vs actual behavior
- Your environment details (browser, OS, etc.)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **🏢 Architecture Office Colleagues**: For honest feedback and real-world validation
- **🤖 [Anthropic](https://anthropic.com)**: For Claude AI and development assistance
- **⚛️ [Vercel](https://vercel.com)**: For Next.js framework and deployment platform
- **🗄️ [Supabase](https://supabase.com)**: For PostgreSQL backend and real-time features
- **🧠 [Google](https://ai.google.dev/)**: For Gemini AI processing capabilities
- **🎨 [Shadcn](https://ui.shadcn.com/)**: For accessible component design system

---

<div align="center">

**Transforming Architecture Office Management, One Project at a Time**

⭐ Star this repository • 🍴 Fork it • 📢 Share it

[🚀 Get Started](#-quick-start) • [📖 View Documentation](docs/) • [🐛 Report Issues](https://github.com/thebrownproject/vibeworks/issues)

*Built with ❤️ by Fraser Brown during his Architecture → IT transition*

</div>