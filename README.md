# E-Commerce Store

A modern, full-stack e-commerce platform built with cutting-edge web technologies. This project features a clean, responsive design with robust authentication, product management, and a seamless shopping experience.

## 🚀 Features

- **Modern UI/UX**: Built with Next.js 15 and TailwindCSS for a responsive, mobile-first design
- **Authentication**: Secure user authentication with Better Auth supporting email/password and social logins
- **Product Management**: Dynamic product catalog with filtering, sorting, and search capabilities
- **Shopping Cart**: Persistent cart functionality with state management via Zustand
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Image Optimization**: Next.js Image component for optimized image loading
- **TypeScript**: Fully typed codebase for better development experience

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript, TailwindCSS
- **Backend**: Next.js API Routes, Drizzle ORM
- **Database**: PostgreSQL (Neon compatible)
- **Authentication**: Better Auth
- **State Management**: Zustand
- **Styling**: TailwindCSS
- **Icons**: Lucide React
- **Development**: ESLint, TypeScript

## 📋 Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/en) (version 18 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [Git](https://git-scm.com/)
- PostgreSQL database (local or cloud-hosted like Neon)

## 🚀 Quick Start

1. **Clone the repository**
\\\ash
git clone https://github.com/jigsaw1270/ecommerceNikeStore.git
cd ecommerceNikeStore
\\\

2. **Install dependencies**
\\\ash
npm install
\\\

3. **Set up environment variables**
\\\ash
cp .env.local.example .env.local
\\\

Edit \.env.local\ with your actual values:
- \DATABASE_URL\: Your PostgreSQL connection string
- \NEXTAUTH_SECRET\: A random string for JWT signing
- \NEXTAUTH_URL\: Your application URL (http://localhost:3000 for development)

4. **Set up the database**
\\\ash
# Generate database migrations
npm run db:generate

# Push schema to database
npm run db:push

# Seed the database with sample data
npm run db:seed
\\\

5. **Start the development server**
\\\ash
npm run dev
\\\

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🗄️ Database Commands

\\\ash
# Generate new migration files
npm run db:generate

# Push schema changes to database
npm run db:push

# Run database migrations
npm run db:migrate

# Open Drizzle Studio (database GUI)
npm run db:studio

# Seed database with sample data
npm run db:seed
\\\

## 📁 Project Structure

\\\
├── src/
│   ├── app/                    # Next.js app directory
│   │   ├── (auth)/            # Authentication routes
│   │   ├── (root)/            # Main application routes
│   │   ├── api/               # API routes
│   │   └── globals.css        # Global styles
│   ├── components/            # Reusable UI components
│   ├── lib/                   # Utility functions and configurations
│   │   ├── actions/           # Server actions
│   │   ├── auth/             # Authentication configuration
│   │   ├── db/               # Database configuration and schema
│   │   └── utils/            # Helper utilities
│   └── store/                # Zustand state management
├── public/                   # Static assets
├── drizzle/                 # Database migrations
└── static/                  # Upload directory
\\\

## 🔧 Configuration

### Database Schema

The application includes the following main entities:
- Users and Authentication
- Products and Variants
- Categories and Brands
- Shopping Cart
- Orders and Payments
- Reviews and Wishlists

### Authentication

Configured with Better Auth supporting:
- Email/Password authentication
- Session management
- Cookie-based sessions
- Configurable social providers

## 🚀 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Configure environment variables in Vercel dashboard
4. Deploy automatically on every push

### Other Platforms

The application is compatible with any Node.js hosting platform:
- Railway
- Render
- Digital Ocean
- AWS
- Google Cloud Platform

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (\git checkout -b feature/amazing-feature\)
3. Commit your changes (\git commit -m 'Add amazing feature'\)
4. Push to the branch (\git push origin feature/amazing-feature\)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🐛 Issues

If you encounter any issues or have questions, please create an issue in the GitHub repository.

## ⭐ Support

If you find this project helpful, please consider giving it a star on GitHub!
