# Converso | LMS SaaS Platform

Converso is a SaaS-based Learning Management System designed to provide continuous, on-demand learning through AI-powered interaction. The platform features an AI voice companion that allows learners to ask questions naturally at any time, removing hesitation, scheduling limits, and dependency on human availability. The focus is on real-time understanding rather than passive content consumption, enabling learners to engage actively with concepts the moment confusion arises.

## Features

- **Secure Authentication & User Management:** Users can sign up, sign in, and manage their profiles securely using Clerk.  
- **Subscription & Billing:** Access to premium content is controlled through subscription tiers, managed by Clerk Billing.  
- **AI-Powered Voice Learning:** Vapi AI Voice Agent allows students to interact in real-time, ask questions naturally, and receive instant feedback.  
- **Interactive Learning Sessions:** Students can engage with course content and ask follow-up questions through the AI companion.  
- **Form Validation & Type Safety:** All forms are validated with React Hook Form and Zod, ensuring accurate data submission.  
- **Modern UI & Accessibility:** The interface is built using ShadCN and TailwindCSS for responsiveness and accessibility.  
- **Error Monitoring:** Sentry is integrated to track errors and monitor application performance.  
- **Scalable Architecture:** Built with Next.js App Router and React Server Components for optimized performance and maintainability.

## Technology Stack

- **Frontend:** Next.js, React Server Components  
- **Backend / Database:** Supabase  
- **UI / Styling:** TailwindCSS, ShadCN  
- **Authentication & Billing:** Clerk  
- **AI Integration:** Vapi AI Voice Agent  
- **Forms & Validation:** React Hook Form, Zod  
- **Monitoring:** Sentry  
- **Language:** TypeScript  
- **Deployment:** Vercel  

## Architecture

Converso follows a client–server architecture leveraging Next.js App Router and React Server Components. The frontend is rendered efficiently with server components, while interactive features use client components. Clerk handles authentication, subscription management, and role-based access control. Supabase manages persistent data and storage. Vapi AI Voice Agent is integrated for real-time learning interactions. Shared Zod schemas enforce data validation across client and server boundaries. Sentry monitors performance and runtime errors, while deployment is managed on Vercel with environment-specific configurations.

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/David900Jason/converso-lms-platform/
```

2. Install dependencies:
```bash
pnpm dev
```

3. Create a ```.env``` file with the following variables:
```
# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# Clerk - Custom Auth
NEXT_PUBLIC_CLERK_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_SIGN_IN_FALLBACK_REDIRECT_URL=
NEXT_PUBLIC_CLERK_SIGN_IN_FALLBACK_REDIRECT_URL=

# Supabase
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_DEFAULT_KEY=

# Vapi
NEXT_PUBLIC_VAPI_WEB_TOKEN=

# Sentry
SENTRY_AUTH_TOKEN=
```

## Role & Responsibilities
I designed and implemented the full system architecture, integrated frontend and backend layers, implemented authentication and billing logic, integrated the AI voice agent, enforced validation and monitoring, and managed deployment. Emphasis was placed on modularity, reusability, and production-ready code.


## Live Demo

Check out the live application here: [https://converso-lms-platform.vercel.app/](Link here)
