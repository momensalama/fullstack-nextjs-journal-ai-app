# Journal AI App

A modern journaling app that uses AI to analyze your entries and track your mood over time. Write honestly, and let AI help you understand your emotional patterns.

[Live Demo](https://fullstack-nextjs-journal-ai-app.vercel.app)

![overview image](./public/overview.jpg)

## Features

**Smart Journaling**

- Create and edit journal entries with autosave
- AI analyzes each entry to detect mood, identify subjects, and score sentiment
- Automatic color coding based on emotional tone
- Concise summaries of your entries

**Visual Insights**

- Interactive charts showing mood trends over time
- Historical sentiment analysis
- Average sentiment score tracking
- Color-coded entry cards for quick visual reference

**AI-Powered**

- Natural language processing for entry analysis
- Ask questions about your journal history
- Supports multiple AI models (Groq and Gemini via LangChain)

## Tech Stack

- **Framework:** Next.js 15.3.2 with React 19
- **Language:** TypeScript
- **Database:** PostgreSQL with Prisma ORM
- **Authentication:** Clerk
- **AI:** LangChain, Google Gemini, Groq
- **Charts:** Recharts
- **Styling:** Tailwind CSS
- **Validation:** Zod

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/momensalama/fullstack-nextjs-journal-ai-app.git
cd fullstack-nextjs-journal-ai-app
```

2. Install dependencies:

```bash
npm install
```

3. Set up environment variables:
   Create a `.env` file in the root directory:

```bash
DATABASE_URL="your_postgresql_connection_string"
CLERK_SECRET_KEY="your_clerk_secret_key"
GROQ_API_KEY="your_groq_api_key"
GEMINI_API_KEY="your_gemini_api_key"
```

4. Set up the database:

```bash
npx prisma migrate dev
npx prisma generate
```

5. Run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
├── app/                    # Next.js app router pages and layouts
│   ├── (dashboard)/       # Protected dashboard routes
│   ├── components/         # React components
│   └── generated/          # Generated Prisma client
├── prisma/                 # Database schema and migrations
├── utils/                  # Utility functions and AI integration
└── public/                 # Static assets
```

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

MIT License - see LICENSE file for details.
