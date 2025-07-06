# BlackBox - Secure Messaging Application

![BlackBox Logo](https://github.com/rigelshasani/BlackBox/assets/64705055/3c0a1c42-3943-48df-9e01-bc1a3a02a784)

A modern, real-time messaging application built with Next.js, featuring secure authentication, group conversations, and an interactive P5.js background. BlackBox focuses on providing a seamless messaging experience with a unique visual aesthetic.

## 🚀 Features

- **Real-time Messaging**: Instant message delivery using Pusher
- **User Authentication**: Secure login/signup with NextAuth.js
- **Group Conversations**: Create and manage group chats
- **User Management**: Add friends and manage user lists
- **Interactive UI**: Dynamic P5.js background animations
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Message Status**: Track read receipts and message status
- **Image Sharing**: Support for image messages
- **Active Status**: Real-time user online/offline indicators

## 🛠️ Tech Stack

### Frontend
- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS framework
- **React Hook Form** - Form handling and validation
- **Zustand** - State management
- **P5.js** - Interactive graphics and animations

### Backend & Database
- **Next.js API Routes** - Server-side API endpoints
- **Prisma** - Database ORM
- **MongoDB** - NoSQL database
- **NextAuth.js** - Authentication framework
- **Pusher** - Real-time messaging infrastructure

### Authentication & Security
- **bcrypt** - Password hashing
- **NextAuth.js** - OAuth and session management
- **JWT** - Secure token-based authentication

### UI/UX Libraries
- **Headless UI** - Accessible UI components
- **React Icons** - Icon library
- **React Hot Toast** - Toast notifications
- **React Spinners** - Loading indicators
- **React Select** - Enhanced select components

## 📋 Prerequisites

Before running this project, make sure you have:

- **Node.js** (v18 or higher)
- **npm** or **yarn** package manager
- **MongoDB** database (local or cloud)
- **Pusher** account for real-time messaging
- **NextAuth.js** configuration (Google OAuth, etc.)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/rigelshasani/BlackBox.git
cd BlackBox
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Setup

Create a `.env.local` file in the root directory with the following variables:

```env
# Database
DATABASE_URL="your_mongodb_connection_string"

# NextAuth.js
NEXTAUTH_SECRET="your_nextauth_secret"
NEXTAUTH_URL="http://localhost:3000"

# OAuth Providers (Google, GitHub, etc.)
GOOGLE_CLIENT_ID="your_google_client_id"
GOOGLE_CLIENT_SECRET="your_google_client_secret"

# Pusher (Real-time messaging)
PUSHER_APP_ID="your_pusher_app_id"
PUSHER_KEY="your_pusher_key"
PUSHER_SECRET="your_pusher_secret"
PUSHER_CLUSTER="your_pusher_cluster"

# Cloudinary (Image uploads)
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME="your_cloudinary_cloud_name"
```

### 4. Database Setup

```bash
# Generate Prisma client
npx prisma generate

# Push schema to database
npx prisma db push
```

### 5. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## 📁 Project Structure

```
BlackBox/
├── app/                          # Next.js App Router
│   ├── (site)/                   # Public site routes
│   │   ├── component/            # Authentication components
│   │   ├── HomePage.tsx          # Landing page
│   │   └── p5Background.js       # Interactive background
│   ├── actions/                  # Server actions
│   ├── api/                      # API routes
│   │   ├── auth/                 # Authentication endpoints
│   │   ├── conversations/        # Conversation management
│   │   ├── messages/             # Message handling
│   │   └── users/                # User management
│   ├── components/               # Reusable UI components
│   ├── conversations/            # Chat interface
│   ├── context/                  # React contexts
│   ├── hooks/                    # Custom React hooks
│   ├── libs/                     # Utility libraries
│   ├── login/                    # Authentication pages
│   └── users/                    # User management pages
├── prisma/                       # Database schema and migrations
├── public/                       # Static assets
└── middleware.ts                 # Next.js middleware
```

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npx prisma studio` - Open Prisma database GUI

## 👥 Collaborators

- **Aanand Aman**
- **Rigels Hasani**
- **Gaganjeet Singh Vaid**
- **Vrushank Janakkumar**

## 📸 Screenshots

![Login Page](https://github.com/rigelshasani/BlackBox/assets/64705055/46a6359f-0816-42aa-ac05-ea995edd278b)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is developed for the PRJ666 course. All rights reserved.

## 🆘 Support

If you encounter any issues or have questions, please:

1. Check the [Issues](https://github.com/rigelshasani/BlackBox/issues) page
2. Create a new issue with detailed information
3. Contact the development team

---

**Built with ❤️ for PRJ666 Course**
