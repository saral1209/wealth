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

```mermaid
graph TD
    A[User Interaction] --> B[Frontend - React/Next.js UI]
    B --> C{API Requests}
    C --> D[Backend - Next.js API Routes + Prisma]
    D --> E[Supabase PostgreSQL]
    D --> F[Gemini AI - Receipt Scanning & Insights]
    D --> G[Arcjet - Security / Rate Limiting]
    D --> H[Inngest - Serverless & Cron Jobs]
    B --> I[Clerk - Authentication & User Management]

------






| **Security**              | Arcjet                     | Rate limiting, bot protection, and API security.                       |
| **Deployment**            | Vercel                     | Hosting and deployment platform for the app.                           |
