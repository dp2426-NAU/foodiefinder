# FoodieFinder 🍽️

A comprehensive restaurant discovery platform with user authentication, admin dashboard, and reservation system.

## Features

### Customer Features
- 🔍 Browse and search restaurants by name, cuisine, or location
- 🍔 View detailed restaurant information and menus
- 💳 Make table reservations with payment processing
- 👤 User authentication (email/password)
- 📱 Responsive design for mobile and desktop

### Admin Features
- 🔐 Separate admin authentication
- 🏪 Manage restaurant listings
- 📋 Manage menu items
- ✏️ Full CRUD operations

## Tech Stack

**Frontend:**
- React 18 with TypeScript
- Wouter (routing)
- TanStack Query (data fetching)
- Shadcn/ui + Tailwind CSS (UI components)
- React Hook Form + Zod (form validation)

**Backend:**
- Node.js + Express
- PostgreSQL (Neon serverless)
- Drizzle ORM
- bcrypt (password hashing)
- Express Session (authentication)

## Demo Accounts

### Customer Accounts (Password: `password123`)
- jandhyala.bhavana@example.com
- ranjith.chukkareddy@example.com
- angelica@example.com
- varshitha.reddy@example.com

### Admin Account
- Email: admin@foodiefinder.com
- Password: admin123

## Test Credit Cards

Use these for testing reservations:
- **Visa:** 4111 1111 1111 1111
- **Mastercard:** 5555 5555 5555 4444
- **Expiry:** Any future date (e.g., 12/25)
- **CVV:** Any 3 digits (e.g., 123)

## Local Development

### Prerequisites
- Node.js 18+
- PostgreSQL database

### Installation

```bash
# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your database credentials

# Run database migrations
npm run db:push

# Start development server
npm run dev
```

The app will be available at `http://localhost:5000`

## Environment Variables

```env
DATABASE_URL=your_postgresql_connection_string
SESSION_SECRET=your_session_secret
NODE_ENV=development
```

## Deployment

### Deploy to Vercel

1. Push code to GitHub
2. Connect your GitHub repo to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy!

### Deploy to Replit
- Already configured! Just click "Publish" in Replit

## Project Structure

```
├── client/              # Frontend React app
│   ├── src/
│   │   ├── components/  # Reusable UI components
│   │   ├── pages/       # Page components
│   │   └── hooks/       # Custom React hooks
├── server/              # Backend Express server
│   ├── routes.ts        # API routes
│   └── storage.ts       # Database operations
├── shared/              # Shared types and schemas
│   └── schema.ts        # Drizzle database schema
└── package.json
```

## License

MIT

## Author

**dp2426-NAU**

Built with ❤️ for restaurant discovery

