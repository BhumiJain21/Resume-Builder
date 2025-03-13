# Resume Builder Application

A web-based resume builder with template selection and PDF export capabilities.

## Project Structure

```
├── client/
│   ├── src/
│   │   ├── components/           # React components
│   │   │   ├── ResumeForm.tsx   # Form for editing resume
│   │   │   ├── ResumePreview.tsx # Resume preview with templates
│   │   │   └── ResumeTemplates.tsx # Template selection
│   │   ├── pages/
│   │   │   └── builder.tsx      # Main resume builder page
│   │   └── App.tsx              # Main React application
│   └── index.html
├── server/
│   ├── index.ts                 # Express server setup
│   ├── routes.ts                # API routes
│   └── storage.ts               # Database operations
└── shared/
    └── schema.ts                # Shared types and database schema
```

## Key Features

- Professional resume templates
- Profile picture upload
- PDF export functionality
- Real-time preview
- Sections for:
  - Personal Information
  - Education
  - Experience
  - Skills
  - Certifications
  - Hobbies & Interests

## Technologies Used

- Frontend:
  - React
  - TypeScript
  - TailwindCSS
  - shadcn/ui components
  - react-to-pdf

- Backend:
  - Express
  - PostgreSQL
  - Drizzle ORM

## How to Download the Code

1. From Replit:
   - Click on the "Files" tab in the left sidebar
   - Click the three dots menu (...)
   - Select "Download as zip"

2. Setting up locally:
   - Extract the downloaded zip file
   - Run `npm install` to install dependencies
   - Create a `.env` file with your database configuration
   - Run `npm run dev` to start the development server

## Important Files and Their Purpose

1. `client/src/pages/builder.tsx`
   - Main page component for the resume builder
   - Handles form state and PDF export

2. `client/src/components/ResumeForm.tsx`
   - Form component for entering resume details
   - Handles all input fields and validation

3. `client/src/components/ResumePreview.tsx`
   - Renders the resume preview with different templates
   - Handles styling and layout for the resume

4. `shared/schema.ts`
   - Defines the database schema and TypeScript types
   - Contains validation rules using Zod

5. `server/routes.ts`
   - API endpoints for CRUD operations
   - Handles resume data persistence

6. `server/storage.ts`
   - Database operations using Drizzle ORM
   - PostgreSQL connection and queries

## Environment Variables Required

```env
DATABASE_URL=postgresql://...
PGHOST=...
PGPORT=...
PGUSER=...
PGPASSWORD=...
PGDATABASE=...
```

## Additional Notes

- The application uses a professional beige/brown color scheme
- Images are stored as Base64 strings in the database
- PDF export is handled client-side using react-to-pdf

## Setting up on GitHub

1. Create a new repository on GitHub

2. Initialize git in your local project directory:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin your-github-repo-url
   git push -u origin main
   ```

3. Prerequisites for running locally:
   - Node.js 18 or higher
   - PostgreSQL database
   - NPM or Yarn package manager

4. Local development setup:
   ```bash
   # Install dependencies
   npm install

   # Create and configure .env file
   cp .env.example .env
   # Edit .env with your database credentials

   # Start development server
   npm run dev
   ```

## Deployment

The application can be deployed on platforms that support Node.js applications with PostgreSQL databases. Make sure to:

1. Set up environment variables
2. Install dependencies with `npm install`
3. Build the project with `npm run build`
4. Start the server with `npm start`

## Contributing

Feel free to submit issues and enhancement requests!