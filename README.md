# 🔄 Skill Swap

A peer-to-peer learning platform where users exchange skills instead of paying for courses.

Skill Swap connects people who want to learn with people who want to teach. Users list the skills they can offer and the skills they want to learn, and our AI-powered matching system finds the most compatible learning partners.

---

## 🚀 Problem Statement

Millions of people want to learn new skills but face barriers such as:

* Expensive online courses
* Lack of personalized learning
* Difficulty finding mentors
* Limited opportunities for practical skill exchange

At the same time, many individuals possess valuable skills they are willing to teach but have no easy way to connect with learners.

Skill Swap bridges this gap by enabling a community-driven knowledge exchange ecosystem.

---

## 💡 Solution

Skill Swap creates a skill-based barter system where users can:

* Offer skills they are proficient in
* Discover skills they want to learn
* Get matched with compatible learners and mentors
* Exchange knowledge without monetary transactions
* Build credibility through ratings and reviews

---

## ✨ Key Features

### 👤 User Onboarding

* Create a profile
* Add skills you can teach
* Add skills you want to learn
* Set learning preferences and interests

### 🤖 AI-Powered Matching

* Intelligent compatibility scoring
* Skill complement analysis
* Personalized match recommendations
* AI-generated match explanations

### 🤝 Skill Exchange Requests

* Send swap requests
* Accept or decline requests
* Manage active exchanges
* Track learning progress

### 💬 Real-Time Communication

* One-to-one chat system
* Session coordination
* Resource sharing
* Learning discussions

### ⭐ Review & Rating System

* Post-session feedback
* Skill verification through reviews
* Reputation building
* Community trust enhancement

---

## 🛠️ Tech Stack

### Frontend

* Next.js 14
* React
* Tailwind CSS

### Backend

* Node.js
* Next.js API Routes

### Database

* PostgreSQL
* Prisma ORM

### Authentication

* Clerk Authentication

### AI Integration

* Claude API

### Deployment

* Vercel

---

## 🏗️ System Architecture

```text
User
  │
  ▼
Next.js Frontend
  │
  ├── Clerk Authentication
  │
  ├── AI Matching Service (Claude API)
  │
  └── Backend API
          │
          ▼
      PostgreSQL
         (Prisma)
```

---

## 📂 Project Structure

```text
skill-swap/
├── app/
│   ├── (auth)/
│   ├── dashboard/
│   ├── profile/[id]/
│   ├── matches/
│   └── chat/[id]/
│
├── components/
│   ├── SkillTag.jsx
│   ├── MatchCard.jsx
│   └── SwapRequestModal.jsx
│
├── lib/
│   ├── db.js
│   ├── matching.js
│   └── claude.js
│
├── prisma/
│   └── schema.prisma
│
└── api/
    ├── matches/
    └── swaps/
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/skill-swap.git
cd skill-swap
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file:

```env
DATABASE_URL=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
ANTHROPIC_API_KEY=
```

### Run Database Migration

```bash
npx prisma migrate dev
```

### Start Development Server

```bash
npm run dev
```

---

## 🔍 How AI Matching Works

The matching engine evaluates:

* Skills offered
* Skills requested
* Mutual learning opportunities
* Common interests
* User preferences
* Historical ratings

It then generates:

* Compatibility score
* Match ranking
* Personalized recommendation reason

Example:

> "You can teach Python while learning UI/UX from Sarah. Both users are interested in startup projects and have highly complementary skill sets."

---

## 🎯 Future Enhancements

* Video call integration
* Group learning circles
* Skill certification badges
* Learning roadmaps
* AI learning assistant
* Calendar scheduling
* Community forums
* Mobile application

---

## 🌍 Impact

Skill Swap promotes:

* Accessible education
* Community collaboration
* Lifelong learning
* Skill development
* Knowledge sharing without financial barriers

---

