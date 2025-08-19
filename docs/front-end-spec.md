# VibeWorks Frontend Specification - MVP

Simple, focused interface for architecture office project management with AI assistance.

## MVP Design Goals

1. **Whiteboard View** - Visual overview of all current projects with search and filters
2. **Simple Ribbon Layout** - Creation buttons for new projects/tasks, quick view dropdown
3. **Collapsible AI Chat** - Right-side chatbot for urgent task capture
4. **Basic Navigation** - Simple left nav for MVP functionality
5. **30-Second Task Capture** - Fast input during high-pressure periods

## Design Principles

1. **Simplicity First** - Minimal interface, maximum utility
2. **CAD-Familiar Patterns** - Leverage existing mental models without complexity
3. **Speed Over Features** - Fast task input more important than comprehensive functionality

## MVP Layout Structure

### Main Interface Components

**Top Ribbon (All Functionality):**
- **Search** bar for projects
- **Sort** dropdown (by job number, jobs with tasks, client name, deadline, etc.)
- **Filters** dropdown (job status, stage, client, priority, etc.)
- **+ New Project** button
- **+ New Task** button

**Left Sidebar (Views/Navigation):**
- Project Board (main whiteboard view)
- Task Board (cross-project task view)
- Staff Allocation (capacity overview)
- Settings

**Center Whiteboard (Digital Replica of Office Physical Whiteboard):**
- Project cards arranged in sections like physical whiteboard:
  - **Town Planning** - Early stage projects
  - **Working Drawings** - Documentation projects
  - **Harnest TP** - Harnest town planning
  - **Harnest WD** - Harnest working drawings
  - **Commercial Shop Fitouts** - All shop fitout projects
- Color-coded project status (green/yellow/red)
- Click cards for project detail modals
- Only active projects displayed (archived projects hidden)

**Right Panel (Collapsible AI Chat):**
- AI Chat interface
- Collapse/expand toggle
- Quick task capture from any screen
- Always accessible for urgent email processing

## Core User Flows (MVP)

### Flow 1: Quick Task Capture via AI Chat

**Goal:** 30-second task capture from email/verbal request

**Steps:**
1. Click AI chat panel (always visible on right)
2. Paste email or describe task
3. AI extracts project, task, estimate
4. Confirm and create

### Flow 2: Project Overview (Whiteboard View)

**Goal:** Quick visual scan of all active projects

**Steps:**
1. Open dashboard (default view)
2. Scan project cards on whiteboard
3. Use search/filters if needed
4. Click project for details

### Flow 3: Add New Project

**Goal:** Simple project creation with address

**Steps:**
1. Click "+ New Project" in ribbon
2. Fill basic details (name, client, address, project type)
3. Save and return to whiteboard
4. Project appears in appropriate whiteboard section

## MVP Screen Descriptions

### Main Dashboard (Digital Whiteboard View)

**Inspired by Real Workplace:** Direct replica of the physical whiteboard your boss currently uses in the office, making adoption natural and immediate.

**Layout:**
- Top ribbon: search, filters, action buttons
- Left sidebar: navigation/views
- Center whiteboard: project cards like sticky notes
- Right panel: collapsible AI chat

**Project Cards (Sticky Note Style):**
- Project name and client (bold header)
- Address (street name, suburb)
- Color-coded status indicator (green/yellow/red)
- Assigned staff avatars/initials
- Project type badge (Regular/Harnest/Shop Fitout)
- Auto-organized by whiteboard section

**Whiteboard Features:**
- Projects grouped into 5 main sections:
  - Town Planning (early stage regular projects)
  - Working Drawings (documentation stage regular projects)
  - Harnest TP, Harnest WD (special client sections)
  - Commercial Shop Fitouts (all shop fitout projects)
- Color coding by status (green=stable, yellow=attention, red=urgent)
- Sticky note visual style matching physical whiteboard

### AI Chat Panel (Right Side)

**Features:**
- Always visible but collapsible
- Email paste area
- Chat history
- Quick task creation
- Project search via natural language

### Project Detail Modal

**When clicking a project card:**
- Modal overlay with project details
- Full address and project information
- Task list with create/edit capabilities
- Staff assignment management
- Project status and stage controls
- Close modal to return to whiteboard

## Architecture Project Stages (From Workplace Observation)

Based on direct observation of the physical whiteboard in Fraser's architecture office, projects are organized by these stage abbreviations:

- **WD** - Working Drawings
- **TP** - Town Planning  
- **ID** - Initial Design
- **[Additional stages to be documented based on office practice]**

**Sort Options in Ribbon:**
- By Job Number
- By Jobs with Tasks (projects that have outstanding tasks)
- By Client Name
- By Deadline
- By Priority
- By Assigned Staff

**Note:** Projects remain grouped by stage (WD, TP, ID, etc.) to match the physical whiteboard, but within each stage group they can be sorted by the above criteria.

**Note:** Detailed wireframes to be created in Figma for development phase.
