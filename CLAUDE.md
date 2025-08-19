# CLAUDE.md - VibeWorks Project

This file provides comprehensive guidance to Claude Code when working with VibeWorks - an AI-powered project management system for architecture offices.

## Template Foundation

### 🎯 **What This Template Provides**

- **Integrated AI Development Methodologies**: Ready for BMAD Method and modern AI-assisted development
- **MCP Server Integration**: 7 pre-configured servers for enhanced development capabilities
- **Context7 Documentation Management**: Intelligent local-first documentation caching and retrieval
- **Three-Tier Token Optimization**: Strategic escalation from built-ins → Gemini CLI → Serena for maximum efficiency
- **BMAD Method**: Pre-installed agentic development methodology with planning and implementation phases

### 🛠️ **Core MCP Server Integrations**

- **Context7**: Documentation retrieval with local caching (`/context7:*` commands)
- **Serena**: Precision semantic targeting after Gemini bulk analysis (Tier 3 in optimization strategy)
- **Playwright**: AI-powered browser automation using accessibility trees
- **Sequential-thinking**: Structured problem-solving with dynamic thought processes
- **Supabase**: Complete database and project management
- **Brave Search**: Comprehensive web search with fresh results
- **Gemini CLI**: Leverage Gemini's massive context window for large-scale analysis

### 🔄 **Core Development Methodologies**

- **BMAD Method**: Agentic planning (Analyst, PM, Architect) → Development (SM, Dev, QA)
- **Three-Tier Workflows**: Built-ins → Gemini CLI → Serena → Claude Code edits → User reviews
- **Token Optimization**: Strategic tool selection, Gemini's massive context, local-first documentation
- **Context7 Strategy**: Build comprehensive local documentation cache over time

## 🚨 CLAUDE.md Final File Size Requirements

**MANDATORY LIMITS (DO NOT REMOVE THIS SECTION):**

- **Maximum:** 700 lines (HARD LIMIT)
- **Preferred:** 450-600 lines (TARGET RANGE)

**Guidelines for Filling TODO Sections:**

- Keep each section concise and focused
- Use bullet points, not long paragraphs
- Focus on essential information Claude needs
- Move detailed documentation to separate files
- Every line consumes tokens on every interaction

**Token Budget Impact:**

- Bloated files = higher costs
- Too much content = reduced Claude effectiveness
- Aim for "lean and intentional" documentation

## Universal Development Principles

### Core Philosophy

- **KISS (Keep It Simple, Stupid)**: Choose straightforward solutions over complex ones
- **YAGNI (You Aren't Gonna Need It)**: Implement features only when needed
- **Fail Fast**: Check for errors early and raise exceptions immediately
- **Single Responsibility**: Each function, class, and module should have one clear purpose

### File and Code Organization

- **Files**: Never exceed 500 lines of code - refactor by splitting into modules
- **Functions**: Keep under 50 lines with single, clear responsibility
- **Classes**: Under 100 lines representing a single concept
- **Line Length**: Maximum 100 characters (adaptable per language)
- **Modules**: Organize by feature or responsibility, not technical layers

### Testing Philosophy

- **Test-Driven Development**: Write tests first, watch them fail, implement minimal code
- **Test Organization**: Keep tests close to the code they test
- **Coverage**: Aim for 80%+ but focus on critical paths
- **Test Types**: Unit (isolation) → Integration (components) → End-to-end (workflows)

### Error Handling

- **Custom Exceptions**: Create domain-specific exception hierarchies
- **Specific Handling**: Catch specific exceptions, not broad catches
- **Resource Management**: Use context managers for cleanup
- **Logging**: Structured logging with appropriate levels

### Security Guidelines

- **Never commit secrets**: Use environment variables and configuration management
- **Input Validation**: Validate all user input at boundaries
- **Parameterized Queries**: Never concatenate user input into queries
- **Dependencies**: Keep updated and monitor for vulnerabilities
- **Authentication**: Implement proper auth/authz patterns

### Git Workflow

- **Branch Strategy**: `main` (production) ← PR ← `feature/*`, `fix/*`, `docs/*`
- **Commit Messages**: `<type>(<scope>): <subject>` format
- **Never include**: "claude code" or "written by claude" in commit messages
- **Daily Flow**: checkout main → pull → create feature branch → develop → PR → merge

## 📚 Context7 Documentation Management Strategy

**🚨 CRITICAL: Always check local documentation cache before writing any new code!**

#### Available Commands & Token Savings

- **`/context7:retrieve-docs`** - Fetch fresh docs from Context7 and cache in `.claude/docs/`
- **`/context7:read-docs`** - Read from local cache first (90% token savings vs MCP calls)
- **`/context7:list-docs`** - View cached documentation inventory
- **`/context7:refresh-docs`** - Update specific cached docs with fresh versions

#### Local Documentation Structure

`.claude/docs/` organization:

- `libraries/` - Third-party library docs (e.g., `react-hooks-2024-08-16.md`)
- `apis/` - API documentation and schemas (e.g., `supabase-2024-08-16.md`)
- `guides/` - Development guides and tutorials
- `project/` - Project-specific documentation

#### Mandatory Pre-Coding Workflow

**Before writing any new code, ALWAYS follow this sequence:**

1. **`/context7:list-docs`** - Check what's cached locally
2. **`/context7:read-docs [library]`** - Review relevant docs from cache
3. **`/context7:retrieve-docs [missing]`** - Fetch any missing documentation
4. **Build understanding** from documentation patterns and APIs
5. **Write code** following documented patterns

## 🚀 Project Overview

**VibeWorks** is an AI-powered project management system designed specifically for architecture offices. It serves a dual purpose:

- **Workplace Solution**: Solving real project management challenges at Fraser's current architecture office
- **Portfolio Demonstration**: Showcasing modern full-stack development skills for career transition from architecture to IT

**MVP Features:**
- Digital whiteboard replicating physical office organization (5 main sections)
- Basic AI chat overlay for rapid task capture and project queries
- Simplified workflow: Town Planning and Working Drawings sections for regular projects
- Project cards with address, status colors, and modal detail views
- Essential real-time updates for project and task changes

**Target Users:**
- Primary: Fraser's architecture office colleagues (8-12 professional architects)
- Secondary: IT industry hiring managers evaluating portfolio quality

## 🛠️ Technology Stack

**Frontend:**
- Next.js 14+ with App Router (React framework)
- TypeScript (type safety and developer experience)
- Shadcn/ui components (accessible design system)
- Tailwind CSS (utility-first styling)
- Zustand (lightweight state management)

**Backend & Services:**
- Supabase PostgreSQL (database with Row Level Security)
- Supabase Auth (authentication and session management)
- Supabase Real-time (collaborative features)
- Vercel AI SDK (AI integration framework)
- Google Gemini 2.5 Pro (AI processing)

**Development & Deployment:**
- Vercel (hosting and serverless functions)
- Vitest (unit testing)
- Playwright (end-to-end testing)
- ESLint + Prettier (code quality)

## 📁 Project Structure

```
vibeworks/
├── src/
│   ├── app/                    # Next.js App Router
│   │   ├── api/               # API routes (projects, tasks, ai/chat)
│   │   ├── project-board/     # Main whiteboard page
│   │   ├── task-board/        # Cross-project task view
│   │   ├── staff-allocation/  # Staff capacity page
│   │   └── layout.tsx         # Root layout with sidebar nav
│   ├── components/
│   │   ├── ui/                # Shadcn/ui base components
│   │   ├── project-board/     # Whiteboard section components
│   │   ├── modals/            # Project/task detail modals
│   │   ├── ai-chat/           # Basic AI chat overlay
│   │   └── common/            # Shared components
│   ├── stores/               # Zustand state (projects, tasks, ui)
│   ├── lib/                  # API clients and utilities
│   ├── types/                # TypeScript type definitions
│   └── hooks/                # Custom React hooks
├── supabase/                 # Database migrations and schemas
├── docs/                     # Project documentation
├── public/                   # Static assets
└── package.json             # Dependencies and scripts
```

Key principles:
- Feature-based organization over technical layers
- Components co-located with their specific domains
- Shared utilities in lib/ directory

## 📋 MVP Scope & Whiteboard Organization

**5-Section Digital Whiteboard:**
- **Town Planning** - Early stage regular projects
- **Working Drawings** - Documentation stage regular projects  
- **Harnest TP** - Harnest client town planning projects
- **Harnest WD** - Harnest client working drawings projects
- **Commercial Shop Fitouts** - All shop fitout projects regardless of stage

**Project Data Structure:**
- Address fields: street_number, street_name, suburb, postcode
- Project types: 'regular' | 'harnest' | 'shop_fitout' 
- Activity status: 'active' | 'not_active' | 'archived'
- Visual status: 'green' | 'yellow' | 'red' for color coding

**MVP Focus Areas:**
- 3 main pages: Project Board, Task Board, Staff Allocation
- Modal-based project details (no separate project pages)
- Basic AI chat overlay for task creation and queries
- Essential real-time updates only

## 🏗️ Architecture

**System Architecture:**
- **Frontend-First**: Next.js application with API routes for backend logic
- **AI Integration**: Conversational interface for rapid task capture and project queries
- **Real-time Collaboration**: Supabase subscriptions for live updates across users
- **Serverless**: Vercel deployment with edge functions for AI processing

**MVP Components:**
- **Basic AI Chat Service**: Simple task creation and project queries
- **Project Management Engine**: Essential CRUD operations for projects and tasks
- **Digital Whiteboard**: 5-section layout (TP, WD, Harnest TP/WD, Shop Fitouts)
- **Modal Interface**: Project details without separate pages
- **Basic Real-time Updates**: Essential collaborative features only

**Data Flow:**
- User input → AI processing → Database updates → Real-time sync → UI updates
- Email content → AI extraction → Task creation → Assignment → Dashboard visibility

## 📋 Development Environment & Configuration

**Prerequisites:**
- Node.js 18+ with npm
- Supabase CLI for local development
- Git for version control

**Setup Process:**
```bash
git clone [repository]
cd vibeworks
npm install
cp .env.example .env.local
npx supabase init && npx supabase start
npm run dev
```

**Environment Variables:**
```bash
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
GOOGLE_AI_API_KEY=your_gemini_api_key
```

**Configuration Management:**
- Environment-specific settings in .env files
- Supabase configuration in supabase/config.toml
- TypeScript configuration in tsconfig.json
- Tailwind configuration in tailwind.config.js

## 🔧 Language-Specific Tooling

**Package Management:**
- npm for dependency management
- package.json scripts for common tasks

**Development Tools:**
- ESLint + TypeScript ESLint for code quality
- Prettier for consistent formatting
- Tailwind CSS for styling
- PostCSS for CSS processing

**Build System:**
- Next.js built-in bundler with automatic optimization
- Vercel deployment pipeline
- TypeScript compilation checking

## 🧪 Testing Strategy

**Testing Framework:**
- Vitest for unit and integration tests
- Playwright for end-to-end testing
- React Testing Library for component testing

**Test Organization:**
- Unit tests co-located with components (`__tests__/` folders)
- Integration tests in `tests/integration/`
- E2E tests in `tests/e2e/`

**Coverage Requirements:**
- 80%+ test coverage on critical paths
- AI chat functionality fully tested
- Project CRUD operations covered
- Real-time collaboration scenarios tested

## 📚 API Documentation

**Core Endpoints:**
- `POST /api/ai/chat` - AI assistant conversations
- `POST /api/ai/process-email` - Email content processing
- `GET/POST /api/projects` - Project management
- `GET/POST /api/projects/[id]/tasks` - Task management
- `GET /api/capacity/dashboard` - Office capacity overview

**Authentication:**
- Supabase Auth with Bearer tokens
- Row Level Security for data isolation
- Protected routes with middleware

**Request/Response Formats:**
- JSON-based API with TypeScript interfaces
- Zod validation for request schemas
- Standardized error responses

## 🚀 Deployment

**Deployment Pipeline:**
- Production: Automatic Vercel deployment from main branch
- Preview: Automatic deployment from feature branches
- Database: Supabase managed PostgreSQL with migrations

**Environment Configuration:**
- Development: localhost:3000 with local Supabase
- Production: vibeworks.vercel.app with production Supabase
- Environment variables managed through Vercel dashboard

**Monitoring:**
- Vercel Analytics for performance metrics
- Supabase dashboard for database monitoring
- Built-in Next.js error boundaries

## 📖 Project-Specific Guidelines

**Architecture Office Context:**
- Always consider 7-stage project lifecycle when building features
- Prioritize speed over complexity for task capture workflows
- Design for CAD-familiar mental models and interaction patterns
- Focus on practical workplace adoption over feature completeness

**AI Integration Standards:**
- Maintain <3 second response times for AI processing
- Design prompts for architecture office terminology and workflows
- Ensure AI responses are actionable and context-aware
- Always provide fallback options for AI failures

**Performance Requirements:**
- Dashboard load time <2 seconds
- Support 8-12 concurrent users without degradation
- Real-time updates within 100ms
- Mobile responsive but desktop-optimized

## 🔗 Dependencies

**Core Framework:**
- next@^14.0.0 - React framework with App Router
- react@^18.0.0 - UI library
- typescript@^5.0.0 - Type safety

**UI & Styling:**
- @radix-ui/react-* - Accessible component primitives
- tailwindcss@^3.4.0 - Utility-first CSS
- lucide-react - Icon library

**Backend & Database:**
- @supabase/supabase-js - Database client
- @supabase/auth-helpers-nextjs - Auth integration

**AI Integration:**
- ai@^3.0.0 - Vercel AI SDK
- @google/generative-ai - Gemini API client

**State Management:**
- zustand@^4.4.0 - Lightweight state management

## 🛠️ Development Tools & Commands

**Development Commands:**
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npm run type-check` - Run TypeScript compiler

**Database Operations:**
- `npx supabase start` - Start local Supabase
- `npx supabase db reset` - Reset local database
- `npx supabase db push` - Push schema changes
- `npx supabase gen types typescript` - Generate TypeScript types

**Testing:**
- `npm run test` - Run unit tests
- `npm run test:e2e` - Run Playwright tests
- `npm run test:watch` - Run tests in watch mode

**Debugging Tools:**
- React DevTools browser extension
- Next.js built-in debugger
- Supabase dashboard for database queries
- Vercel Functions dashboard for API monitoring

### Three-Tier Token Optimization Strategy

**MANDATORY: Follow this escalation strategy for maximum token efficiency**

#### **Tier 1: Claude Code Built-ins** (Start Here)

- **Tools**: `Grep`, `Glob`, `Read`, `LS`
- **Use for**: Small projects, known file locations, simple pattern searches

#### **Tier 2: Gemini CLI** (Scale Up for Large Analysis)

- **Massive Context**: 1M+ token window for bulk analysis
- **Use for**: Large codebase exploration, architectural understanding, "analyze entire codebase" queries
- **Strategy**: Leverage Gemini's generous context limits to save Claude Code tokens
- **Perfect for**: Planning phases, comprehensive code reviews, alternative perspectives

#### **Tier 3: Serena MCP** (Precision Targeting)

- **Use for**: Precise symbol-level navigation when Gemini identifies specific targets
- **Tools**: `search_for_pattern`, `get_symbols_overview`, `find_symbol`, `write_memory`
- **Strategy**: Semantic analysis without full file reads after Gemini bulk discovery

#### **Decision Matrix**

- **Small/Medium projects**: Tier 1 → Direct Claude Code editing
- **Large codebases**: Tier 2 (Gemini bulk) → Tier 3 (Serena precision) → Claude Code editing
- **Unknown structure**: Tier 2 exploration → Tier 3 navigation → implementation

### Integration with MCP Servers

- **Context7**: **MANDATORY** - Always use `/context7:read-docs` before coding, `/context7:retrieve-docs` to build comprehensive local documentation cache
- **Gemini CLI**: **Tier 2** - Use for large-scale code analysis and architectural feedback to save Claude Code tokens
- **Serena**: **Tier 3** - Leverage semantic search for precision targeting after Gemini discovery
- **Playwright**: Document any browser automation or testing workflows
- **Sequential-thinking**: Use for complex architectural decisions and structured problem-solving
- **Supabase**: Document database schemas and migration patterns
- **Brave Search**: Research best practices and current solutions

## 📚 Useful Resources

**Framework Documentation:**
- Next.js App Router documentation
- React 18 documentation with hooks and concurrent features
- TypeScript handbook and best practices
- Supabase documentation for database and auth

**Component Libraries:**
- Shadcn/ui component documentation
- Radix UI primitives documentation
- Tailwind CSS utility classes reference

**AI Integration:**
- Vercel AI SDK documentation
- Google Gemini API documentation
- Best practices for conversational interfaces

**Architecture References:**
- Architecture office project management best practices
- CAD software interface design patterns
- Real-time collaboration implementation guides

---

**This is a living document.** Update and improve it as VibeWorks evolves and new patterns emerge during development. The focus remains on solving real workplace challenges while demonstrating professional development capabilities.