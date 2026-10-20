# Shared Expense Management Web App

A web application built to simplify shared living expenses for flatmates and housemates. It tracks who paid for what, automatically calculates outstanding balances, and helps group members settle debts accurately without manual bookkeeping errors.

---

## Project Overview

When multiple people live together in an apartment, tracking shared expenses (electricity, water, Wi-Fi, groceries) often leads to confusion and miscalculations. 

This application provides a simple, centralized platform for housemates to:
- Log expenses paid on behalf of the group.
- Automatically compute individual debts and credits.
- View real-time debt summaries (who owes whom and how much).
- Mark debts as settled when payments are made offline.

---

## Core User Roles

- **Group Creator (Primary Tenant):** Can create a living group, invite members, and access the group's total financial overview.
- **Tenant (Group Member):** Can log new expenses, view their personal debt/credit balance, and mark debts as settled.

---

## Main Application Flow

1. **Group Setup:** Users create or join an existing shared living group.
2. **Expense Logging:** A user logs an expense by entering the amount, description, payer, and selected members sharing the cost.
3. **Automated Calculation:** The system immediately updates individual balances across the group based on equal splits or manually assigned amounts.
4. **Balance Review:** Members check the balance overview to see exact owed amounts.
5. **Settlement:** Once a debt is paid (via cash or bank transfer), a user marks it as **Paid**, updating the balance in real-time.

---

## Core Features & Screens

- **Screen 1 — Group Expense List:** A feed showing all group expenses (payer, amount, description, date) with quick navigation to log new expenses or view balances.
- **Screen 2 — Add New Expense:** Form to input cost details, select payers, and specify participants sharing the expense.
- **Screen 3 — Balance Overview:** A clear summary of debts between all members, featuring a one-click button to mark specific debts as settled.

---

## Project Scope

### Included Features
- Group creation and member invitation.
- Expense logging with custom participant selection.
- Real-time automated balance calculation (equal split or manual entry).
- Detailed expense history and balance breakdown.
- Manual debt settlement tracking.

### Out of Scope
- Direct online payment integration (e-wallets, bank APIs).
- Native mobile applications (Web platform only).
- Multi-currency support.
- In-app messaging or chat features.
- Advanced percentage-based splitting.

---

## Tech Stack

- **Frontend:** React 19, TypeScript, Vite, Tailwind CSS v4, Lucide React, React Router v7
- **Backend / Database:** Supabase (PostgreSQL, Auth)
- **State & Data Fetching:** TanStack Query (`@tanstack/react-query`)

---

## Getting Started

### Prerequisites

Make sure you have Node.js (v18+ recommended) and `npm` installed.

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd expense_management
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up Environment Variables:**
   Create a `.env.local` file in the root directory and fill in your Supabase credentials:
   ```env
   VITE_SUPABASE_URL=your_supabase_project_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. **Run the development server:**
   ```bash
   npm run dev
   ```

5. **Build for production:**
   ```bash
   npm run build
   ```

---

## Author

- **Nguyễn Hoàng Nam** - Student ID: `24120097`