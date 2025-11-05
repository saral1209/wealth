**💰 Wealth – AI-Powered Full Stack Finance Platform**

Track, manage, and optimize your finances effortlessly with AI-driven insights.

[live demo : https://aurion-ai-finance-platform.vercel.app/]

screenshots : 

<img width="1250" height="643" alt="wealth1" src="https://github.com/user-attachments/assets/028577e3-d1eb-4da0-a09b-f66419d1b540" />

<img width="1075" height="626" alt="wealth2" src="https://github.com/user-attachments/assets/ee141043-a920-425d-a74c-7d526b3f9dd1" />

<img width="1365" height="645" alt="wealth3" src="https://github.com/user-attachments/assets/489d6f99-d352-4f61-8ab3-420558fb272c" />

**📝 Project Description**

Wealth is a full-stack AI-driven personal finance
platform that allows users to track income and expenses, manage multiple accounts, and receive AI-powered financial insights. The platform automates financial tracking and reporting, making money management simple and intelligent.

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

## 📂 Folder Structure 

The core folder structure of this Next.js project is organized as follows:

```bash
📦 ai-finance-platform/
├── 📂 app/
│   ├── 📂 (auth)/
│   │   ├── 📂 sign-in/
│   │   │   ├── 📂 [[...sign-in]]/
│   │   │   │   └── 📄 page.jsx
│   │   ├── 📂 sign-up/
│   │   │   ├── 📂 [[...sign-up]]/
│   │   │   │   └── 📄 page.jsx
│   │   └── 📄 layout.jsx
│   ├── 📂 api/
│   ├── 📂 dashboard/
│   ├── 📂 account/
│   ├── 📂 transactions/
│   ├── 📄 layout.jsx
│   └── 📄 page.jsx
├── 📂 components/
│   ├── 📂 ui/
│   └── 📁 custom-components/
├── 📂 public/
│   ├── 🖼️ logo.png
│   └── 🖼️ banner.jpeg
├── ⚙️ .env
├── ⚙️ middleware.js
├── 📜 package.json
└── ⚙️ other-config-files/



Folder Descriptions

app/ → Core directory using Next.js App Router. Contains routes, layouts, and pages.

(auth)/ → Handles Clerk authentication pages like sign-in and sign-up.

api/ → API routes for backend logic and data handling.

dashboard/ → Main user dashboard showing insights and financial overview.

account/ → User account settings like username, profile photo, etc.

transactions/ → Manage, view, and add income/expense transactions.

components/ → Reusable UI parts built using Shadcn UI and custom React components.

public/ → Static assets like images and icons.

.env → Environment variables (e.g., Clerk, Supabase, Gemini AI keys).

middleware.js → Protects routes and manages authentication redirects.

package.json → Project dependencies and npm scripts.

other-config-files/ → Additional setup/configuration files (e.g., ESLint, Prettier).



⚡ **Installation & Setup Instructions**

```bash
# 1️⃣ Install dependencies
npm install
# or yarn / pnpm

# 2️⃣ Add environment variables in .env
# Clerk & Supabase credentials
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=...
CLERK_SECRET_KEY=...
DATABASE_URL=...
DIRECT_URL=...

# 3️⃣ Initialize UI & Prisma
npx shadcn-ui@latest init
npx shadcn-ui@latest add button badge card checkbox dialog input tooltip
npx prisma db push
npx prisma generate

# 4️⃣ Run dev server
npm run dev


🧠 **What I Learned**

Built a full-stack AI finance platform using **Next.js, Tailwind CSS, Shadcn UI, Supabase, Prisma, and Clerk**.  
Integrated **AI features** (receipt scanning & insights) and automated tasks with **Inngest**.  
Implemented **secure authentication**, robust **form handling**, **data management**, and deployed seamlessly on **Vercel**.


⚔️ **Challenges Faced**

- Linking Clerk, Supabase, Prisma & Inngest for smooth full-stack integration.  
- Implementing AI receipt scanning & automated insights with Gemini AI.  
- Ensuring responsive UI with Shadcn UI + Tailwind CSS.  
- Securing APIs with Arcjet and validating forms using React Hook Form + Zod.



🔮 **Future Enhancements**


- 💹 **Investment Tracking:** Add stock, crypto, and asset tracking via financial APIs.  
- 🎯 **Goal-Based Planning:** Let users set savings goals and track progress.  
- 📊 **Advanced Analytics:** Provide deeper insights, forecasting tools, and richer data visualizations.  
- 🌍 **Multi-Currency Support:** Manage transactions across global currencies.  
- ⏰ **Bill Reminders & Automation:** Track upcoming bills and automate payments.  
- 🔗 **Third-Party Integrations:** Connect securely with banks, credit cards, and tax tools.  
- 📚 **Financial Education:** Offer in-app learning and budgeting tips.  
- 🧠 **Expanded AI Capabilities:** Proactive insights, fraud detection, and smarter NLP interactions.  
- ⚙️ **Performance Optimization:** Scale efficiently for large datasets and high traffic.  




