Here’s a detailed high-level project description you can give to Cursor / Claude as a reference for building your app. It’s based on the uploaded Mottazen Habit Tracker architecture and expands it into a scalable production-ready system.

------

# Mottazen — Intelligent Habit & Life Operating System

## Vision

Mottazen is not just a habit tracker.

It is a premium life operating system designed to help users create balance, discipline, self-awareness, and long-term personal growth through:

- Habit tracking
- Progress monitoring
- Behavioral analysis
- Deep life organization
- Psychological reinforcement
- Long-term goal alignment

The app should feel like:

- Apple Health + Notion + GitHub Contributions + Minimal iOS design
- Extremely smooth
- Emotionally motivating
- Minimal friction
- Calm and premium
- Fast and responsive
- Visually intelligent without being overwhelming

The philosophy is:

> “Reduce noise. Increase clarity. Small actions compound into identity.”

------

# Core Product Identity

## Product Type

A:

- Habit tracker
- Life organization system
- Behavioral analytics dashboard
- Personal growth assistant
- Future “Life Purpose OS”

The current version focuses on habits, but the architecture must support future expansion into:

- Goals
- Notes
- Journaling
- Life domains
- Long-term planning
- Purpose mapping
- Routines
- Knowledge management
- Emotional tracking
- AI coaching

------

# Design Philosophy

## UI / UX Principles

The UI should feel:

- Native iOS quality
- Calm
- Minimal
- Premium
- Soft
- Highly readable
- Low cognitive load

Avoid:

- Clutter
- Gamification overload
- Complex dashboards
- Corporate appearance
- Heavy gradients
- Cheap-looking UI

Everything should feel:

- Spacious
- Intentional
- Fluid
- Lightweight

Animations should be:

- Subtle
- Spring-based
- Responsive
- Purposeful

------

# Main App Structure

## Primary Sections

### 1. Log View

Main daily interaction screen.

Purpose:

- Quickly log habits with minimum friction
- See progress instantly
- Encourage consistency

Contains:

- Daily score ring
- Date scroller
- Habit cards
- Compact mode
- Daily notes
- Quick add button

------

### 2. Analysis View

Purpose:

- Show behavioral patterns
- Encourage self-awareness
- Reveal long-term consistency trends

Contains:

- Weekly averages
- Habit performance
- Streaks
- Heatmaps
- Monthly trends
- Best-performing habits
- Completion analytics
- Historical insights

------

### 3. Future Modules (Architecture Ready)

The database and frontend architecture should already support future modules like:

#### Goals System

Hierarchical goals with:

- Parent/child goals
- Weights
- Progress propagation
- Milestones
- Habits linked to goals

#### Journaling

- Daily reflections
- Mood tracking
- AI summaries

#### Life Domains

Examples:

- Health
- Mind
- Finance
- Career
- Relationships
- Spirituality
- Creativity

#### AI Assistant

Future AI layer that:

- Detects patterns
- Suggests improvements
- Identifies weak habits
- Generates summaries
- Detects burnout trends

------

# Habit System

## Habit Types

### Binary Habits

Examples:

- Pray
- Read
- Sleep before midnight

Values:

- Complete / incomplete

------

### Numeric Habits

Examples:

- Water intake
- Creatine
- Gym duration
- Calories
- Steps

Supports:

- Min value
- Max target
- Step increments
- Different scoring modes

------

# Scoring System

## Progressive Scoring

Progress increases gradually based on value.

Example:

- 10/20 water = 50%

------

## Any-Value Counts Mode

Any logged value counts as complete.

Example:

- Any amount of creatine = 100%

Useful for:

- Flexible habits
- Non-linear habits

------

# Habit Categories

Habits belong to categories such as:

- Health
- Mind
- Work
- Movement
- Sleep
- Spirit
- Other

Requirements:

- Custom categories
- Reordering
- Collapsible groups
- Category analytics

------

# Daily System

Each day should support:

- Habit logs
- Completion score
- Notes
- Mood (future)
- Energy levels (future)

The system should feel like:

> “A snapshot of your life that day.”

------

# Logging Experience

The logging flow is the most important part of the app.

Requirements:

- Extremely fast
- One-hand mobile use
- Minimal taps
- No lag
- Immediate visual feedback

Interactions:

- Tap checkboxes
- Increment numbers
- Long press to skip
- Drag reorder
- Swipe-friendly
- Smooth animations

------

# Streak Logic

The app should support:

- Current streak
- Longest streak
- Freeze days
- Skip/rest days
- Smart streak preservation

Skipped days should:

- Not punish the streak
- Be visually differentiated

------

# Analysis System

## Heatmap

GitHub-style contribution heatmap.

Purpose:

- Show consistency visually
- Encourage momentum

Color intensity based on:

- Daily completion %

------

## Weekly Bars

Shows:

- Daily completion over last 7 days

------

## Habit Breakdown

Per habit:

- Completion %
- Consistency
- Average value
- Monthly trends
- Longest streak

------

## Habit Detail Page

Per habit analytics:

- Monthly bars
- Streak stats
- Completion trends
- Historical values
- Best periods
- Weak periods

------

# Notes System

Each day has:

- Freeform notes
- Reflection area

Used for:

- Tracking emotional context
- Understanding failures
- Capturing insights

Future AI should analyze notes.

------

# Mobile-First Architecture

The app must be:

- Mobile-first
- Responsive
- Optimized for iPhone
- Thumb-friendly

Desktop should:

- Expand gracefully
- Use multi-column layout
- Preserve mobile feel

------

# Technical Architecture

## Frontend

Recommended:

- React / Next.js
- TypeScript
- Tailwind
- Framer Motion

Alternative acceptable:

- Pure HTML/CSS/JS for MVP

------

# Backend

Use:

## Supabase

For:

- Authentication
- Database
- Realtime sync
- Row-level security
- Storage

Authentication:

- Google
- Apple
- Email/password

------

# Database Design

The database must be scalable from day one.

Core tables:

## users

Stores:

- Profile
- Preferences
- Theme
- Settings

------

## habits

Stores:

- Name
- Type
- Category
- Reminder
- Score settings
- Order
- Pause state

------

## habit_logs

Stores:

- User
- Habit
- Date
- Value
- Skip status

------

## notes

Stores:

- Date
- Content

------

## categories

Stores:

- Name
- Order
- Collapse state
- Custom metadata

------

# Future Database Expansion

Must support:

- Goals
- Subgoals
- Relationships
- Habit-to-goal linking
- Progress propagation
- AI insights
- Journals
- Mood entries

------

# Performance Requirements

The app must feel:

- Instant
- Native
- Extremely smooth

Requirements:

- Optimistic UI updates
- Local caching
- Offline support
- Fast hydration
- Minimal rerenders

------

# Offline-First Philosophy

Users should be able to:

- Log habits offline
- Continue using app without internet
- Sync automatically later

------

# Export / Import

Support:

- JSON export
- CSV export
- Markdown reports

Import:

- CSV
- JSON

Future:

- Notion export
- Apple Health sync
- Google Fit sync

------

# Psychological Design

The app should subtly encourage:

- Discipline
- Calmness
- Clarity
- Consistency
- Identity transformation

Avoid:

- Toxic productivity
- Aggressive gamification
- Stressful reminders

The user should feel:

> “I’m becoming aligned.”

------

# Long-Term Product Direction

Mottazen should eventually evolve into:

## A complete life operating system.

Potential future systems:

- Goals OS
- AI planning
- Knowledge management
- Emotional intelligence tracking
- Purpose mapping
- Life analytics
- Focus system
- Dopamine management
- Routine builder
- Financial tracking
- Health integration

------

# Visual Inspiration

Use inspiration from:

- Apple Health
- Notion
- Arc Browser
- Linear
- Things 3
- GitHub heatmaps
- iOS widgets

Avoid:

- Generic Material UI dashboards
- Crypto-style dashboards
- Heavy neon gamer UI

------

# Final Development Philosophy

The app should prioritize:

1. Simplicity
2. Speed
3. Clarity
4. Expandability
5. Emotional experience
6. Long-term scalability

Every feature should answer:

> “Does this reduce friction and improve clarity?”

Not:

> “Does this add complexity?”