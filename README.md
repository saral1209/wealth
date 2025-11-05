**💰 Wealth – AI-Powered Full Stack Finance Platform**

Track, manage, and optimize your finances effortlessly with AI-driven insights.


---

**📝 Project Description**

Wealth is a full-stack AI-driven personal finance platform that allows users to track income and expenses, manage multiple accounts, and receive AI-powered financial insights. The platform automates financial tracking and reporting, making money management simple and intelligent.

## ⚙️ Tech Stack

| Category                  | Technology / Tool           | Purpose / Description                                                   |
|---------------------------|----------------------------|------------------------------------------------------------------------|
| **Frontend**              | React 19                   | Core library for building dynamic user interfaces.                     |
|                           | Next.js 15                 | React framework for SSR, routing, and API routes.                      |
|                           | Tailwind CSS               | Utility-first CSS framework for responsive styling.                    |
|                           | Shadcn UI                  | Pre-built, reusable, and customizable UI components.                   |
|                           | React Hook Form + Zod      | Efficient form management and schema-based validation.                 |
| **Backend & Database**    | Supabase                   | PostgreSQL database for storing and managing data.                     |
|                           | Prisma ORM                 | ORM for interacting with the database efficiently.                     |
| **Authentication**        | Clerk                      | User management, authentication, and authorization.                    |
| **AI / Integration**      | Google Gemini AI           | AI-powered receipt scanning and monthly financial insights.            |
| **Task Scheduling / Workflow** | Inngest               | Background jobs, cron jobs, and automated workflows (e.g., budget alerts). |

-------

## 💰 Project Overview

**Wealth – AI-Powered Full Stack Finance Platform** helps users efficiently manage personal finances across multiple accounts.  

Key capabilities include:  
- Track income and expenses with multi-account support.  
- Categorize transactions and monitor spending habits.  
- Receive AI-powered insights for smarter financial decisions.  
- Automate transaction entry via AI receipt scanning.  
- Generate monthly financial reports and budget alerts.  

Designed for individuals who want an **intelligent, automated, and user-friendly finance platform** to stay on top of their financial health.

------

## ✨ Key Features

This AI-Powered Finance Platform offers a comprehensive set of features to manage personal finances efficiently:

- **Income & Expense Tracking:** Track income and expenses across multiple accounts.  
- **Smart Categorization & AI Receipt Scanning:** Automatically categorize transactions; scan receipts to enter expenses easily.  
- **Recurring Transactions:** Schedule recurring payments and income for automation.  
- **Budget Management System:** Set budgets and receive email alerts when nearing limits.  
- **Interactive Charts & Visualizations:** Analyze daily transactions and long-term spending trends with intuitive charts.  
- **AI-Powered Monthly Reports:** Receive personalized monthly insights via email to improve financial decision-making.  
- **User Authentication & Account Management:** Secure login/signup with profile management.  
- **Bulk Transaction Management:** Filter, sort, and manage multiple transactions efficiently.  
- **Security Features:** Rate limiting and bot protection using Arcjet for secure and safe usage.

  ---------

  ## 🧠 System Architecture / Project Overview

The "Wealth" platform is a full-stack AI finance platform with clear communication between frontend, backend, database, and third-party services.

### 🔹 Architecture Overview

- **Frontend (React 19 + Next.js 15 + Tailwind CSS + Shadcn UI):**  
  Users interact with the UI; handles authentication via Clerk and sends requests to backend API routes.

- **Backend (Next.js API Routes + Prisma ORM):**  
  Handles business logic, database queries, AI requests (Gemini AI), and user authentication via Clerk. Arcjet provides rate limiting and bot protection.

- **Database (Supabase PostgreSQL):**  
  Stores user accounts, transactions, budgets, and other application data. Prisma ORM facilitates queries and data modeling.

- **Serverless Functions & Cron Jobs (Inngest):**  
  Executes background tasks like budget alerts, recurring transactions, and AI-generated monthly reports.

- **Third-Party Services:**  
  - Clerk → Authentication  
  - Gemini AI → AI-powered receipt scanning & financial insights  
  - Arcjet → Security & rate limiting  

### 🔄 Communication Flow (Mermaid Diagram)


    A[User Interaction] --> B[Frontend - React/Next.js UI]
    B --> C{API Requests}
    C --> D[Backend - Next.js API Routes + Prisma]
    D --> E[Supabase PostgreSQL]
    D --> F[Gemini AI - Receipt Scanning & Insights]
    D --> G[Arcjet - Security / Rate Limiting]
    D --> H[Inngest - Serverless & Cron Jobs]
    B --> I[Clerk - Authentication & User Management]


| **Security**              | Arcjet                     | Rate limiting, bot protection, and API security.                       |
| **Deployment**            | Vercel                     | Hosting and deployment platform for the app.                           |

------

## 6️⃣ 📂 Folder Structure 

The core folder structure of this Next.js project is organized as follows:


├── app/
│   ├── (auth)/
│   │   ├── sign-in/
│   │   │   ├── [[...sign-in]]/
│   │   │   │   └── page.jsx
│   │   ├── sign-up/
│   │   │   ├── [[...sign-up]]/
│   │   │   │   └── page.jsx
│   │   └── layout.jsx
│   ├── api/
│   ├── dashboard/
│   ├── account/
│   ├── transactions/
│   ├── layout.jsx
│   └── page.jsx
├── components/
│   ├── ui/
│   └── (Your custom components)
├── public/
│   ├── logo.png
│   └── banner.jpeg
├── .env
├── middleware.js
├── package.json
└── (other configuration files)

----


## ⚡ Installation & Setup Instructions

Install Dependencies

Navigate into the project directory and install all necessary Node.js packages:

npm install

Set Up Environment Variables

Create a .env file in the root directory with your Clerk and Supabase credentials.

Clerk Setup

1. Go to Clerk and create a new application.

2. Copy your Public Key and Secret Key.

3. Add to .env:

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pkyourpublic_key
CLERK_SECRET_KEY=skyoursecret_key
NEXT_PUBLIC_CLERK_SIGNIN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGNUP_URL=/sign-up

**Supabase Setup**

1. Go to Supabase and create a new project.

2. Copy the connection string for Prisma from Project Settings → Database → Connection String.
3. Add to .env:

DATABASE_URL="postgresql://postgres:[YOUR_PASSWORD]@db.[yourprojectid].supabase.co:5432/postgres?pgbouncer=true&connection_limit=1"
DIRECT_URL="postgresql://postgres:[YOUR_PASSWORD]@db.[yourprojectid].supabase.co:5432/postgres?schema=public"

Initialize Shadcn UI Components

Initialize Shadcn UI in your project:
npx shadcn-ui@latest init
Choose New York for style.
Select yes for CSS variables for theming.
Use Legacy peer deps for React 19 compatibility.
Then, add components:
npx shadcn-ui@latest add button badge calendar card checkbox dialog dropdown-menu input popover progress select switch table tooltip

> Again, choose use Legacy peer deps if prompted.

**Set Up Prisma**
Generate the Prisma client and push your schema to Supabase:
npx prisma db push
npx prisma generate

**Run the Development Server**
Start the Next.js development server:
npm run dev
The application should now be running at http://localhost:3000.
You can log in using your Clerk authentication setup.


