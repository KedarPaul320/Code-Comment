# Code Comment

AI-powered code commenting assistant built with Next.js. Paste code, get clear explanations and inline comments via an API route.

## Project Overview
This project is a modern web application built with Next.js, TypeScript, and Tailwind CSS. It provides an interactive interface for users to submit code and receive AI-generated explanations and inline comments. The backend features a dedicated API route (`/api/code-comment`) for processing code and returning annotated results. The modular structure and use of cutting-edge technologies make it ideal for scalable, maintainable development.

## Technologies Used
- **Next.js**: React-based framework for server-side rendering and API routes
- **TypeScript**: Type-safe development for maintainable code
- **Tailwind CSS**: Utility-first CSS framework for rapid UI styling
- **Node.js**: Runtime environment for server-side logic
- **API Routes**: Custom endpoint for code commenting (`/api/code-comment`)
- **LLM Integration**: Connects to a local or hosted Large Language Model for code analysis and comment generation

## Features
- Paste code and receive AI-generated explanations and inline comments
- Supports multiple programming languages
- Clean, modern UI with Tailwind CSS
- Easily extendable API for custom LLMs/providers
- Ready for deployment to Vercel, Netlify, Docker, or any Next.js-compatible host

## Prerequisites
- Node.js 18+
- npm, pnpm, or yarn

## Quick Start
```bash
# From repo root
cd "Code Comment/nextjs-app"

# Install dependencies
npm install

# Run dev server
npm run dev
# App will be available at http://localhost:3000
```

## Project Structure
```
Code Comment/
  nextjs-app/
    app/
      api/
        code-comment/
          route.ts    # API endpoint for generating code comments
      layout.tsx      # Root layout
      page.tsx        # UI entry
    tailwind.config.js
    package.json
```

## API
- Endpoint: POST `/api/code-comment`
- Body: `{ code: string, language?: string }`
- Response: `{ comments: string }` (shape may vary based on implementation)

See `nextjs-app/app/api/code-comment/route.ts` for exact contract and model configuration.

## Scripts
- `npm run dev`: Start development server
- `npm run build`: Build production bundle
- `npm start`: Run production server
- `npm run lint`: Lint

## Configuration
- Tailwind is pre-configured. Edit `app/globals.css` and component styles as needed.
- Update model/provider settings inside the API route to point to your LLM (local or hosted).

## Deployment
Deploy to any Next.js-compatible host (Vercel, Netlify, Docker, etc.). Ensure required env vars for your LLM/provider are configured.

## License
See the repository root `LICENSE` file.
