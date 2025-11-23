# Swasthya Sakhi

Swasthya Sakhi is a comprehensive healthcare management tool designed to empower Community Health Workers (CHWs) in rural India. It facilitates patient management, provides AI-driven health assistance, and ensures seamless data synchronization for better healthcare delivery.

## 🚀 Features

- **Patient Management**: 
  - Record and track patient details efficiently.
  - Manage case histories and follow-ups.
  - Categorize patients (e.g., Pregnant Women, High Risk, Referrals).
- **AI Health Assistant**: 
  - Integrated AI assistant (powered by Gemini) to answer medical queries.
  - Supports voice and image inputs for ease of use.
  - Provides protocol-based guidance following WHO and Indian RCH standards.
- **Real-time Dashboard**: 
  - View live statistics on active cases, follow-ups, and high-risk patients.
  - Real-time updates using Supabase subscriptions.
- **Multilingual Support**: 
  - Built-in support for multiple languages to cater to diverse regions.
- **Offline Capable**: 
  - Designed for low-connectivity environments (PWA ready).

## 🛠️ Tech Stack

### Frontend
- **Framework**: [React](https://reactjs.org/) with [Vite](https://vitejs.dev/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) & [shadcn/ui](https://ui.shadcn.com/)
- **State Management**: [TanStack Query](https://tanstack.com/query/latest)
- **Routing**: [React Router](https://reactrouter.com/)
- **Forms**: React Hook Form + Zod
- **Internationalization**: i18next

### Backend
- **Platform**: [Supabase](https://supabase.com/) (BaaS)
- **Database**: PostgreSQL
- **Edge Functions**: Deno (TypeScript)
- **AI Integration**: Google Gemini 2.5 Flash via Lovable Gateway

## 📂 Project Structure

```
Swasthya-sakhi/
├── src/
│   ├── components/      # Reusable UI components and feature modules
│   ├── hooks/           # Custom React hooks (e.g., useCases)
│   ├── i18n/            # Internationalization configuration
│   ├── integrations/    # Supabase client and type definitions
│   ├── pages/           # Main application pages (Index, Auth, etc.)
│   └── lib/             # Utility functions
├── supabase/
│   ├── functions/       # Edge functions (e.g., ai-health-assistant)
│   └── migrations/      # Database schema migrations
└── public/              # Static assets
```

## ⚡ Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or bun
- A Supabase project

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Swasthya-sakhi
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory and add your Supabase credentials:
   ```env
   VITE_SUPABASE_URL=your_supabase_project_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. **Run the Development Server**
   ```bash
   npm run dev
   ```

## 🔧 Scripts

- `npm run dev`: Start the development server.
- `npm run build`: Build the application for production.
- `npm run lint`: Run ESLint to check for code quality issues.
- `npm run preview`: Preview the production build locally.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License.
