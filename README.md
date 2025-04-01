# 🌿 Prompt Garden

A modern SaaS platform for creating, testing, and deploying AI prompts. Built with Next.js 14 (App Router), TypeScript, and Supabase.

## Features

- 🎯 Create and manage AI prompts with version control
- 🧪 Test prompts across multiple AI models
- 📊 Compare performance, costs, and latency
- 🔄 Version control for prompts
- 🚀 Deploy prompts via Forms/Webhooks
- 📚 Educational resources for prompt engineering
- 🔑 Freemium model with App Keys (Free) and BYOK (Pro)

## Tech Stack

- **Framework:** Next.js 14 (App Router)
- **Language:** TypeScript
- **Database/Auth:** Supabase
- **Styling:** Tailwind CSS
- **Components:** Shadcn/ui
- **State Management:** Zustand
- **Deployment:** Vercel

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/gofarrrr/prompt-garden.git
   cd prompt-garden
   ```

2. Install dependencies:
   ```bash
   pnpm install
   ```

3. Set up environment variables:
   ```bash
   cp .env.example .env.local
   ```
   Fill in your environment variables in `.env.local`

4. Start the development server:
   ```bash
   pnpm dev
   ```

## Environment Variables

Required environment variables:

```bash
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key

# App LLM Keys (for Free Tier)
APP_OPENAI_API_KEY=your_openai_key
# Add other model keys as needed
```

## Project Structure

```
├── app/                 # Next.js App Router pages and layouts
├── components/          # React components
├── lib/                 # Library code, utilities
├── utils/              # Utility functions
├── store/              # Zustand store
├── actions/            # Server actions
├── types/              # TypeScript types
├── supabase/
│   ├── functions/     # Edge Functions
│   └── migrations/    # Database migrations
└── public/             # Static assets
```

## Contributing

Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.