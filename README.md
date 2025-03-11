# HireRoom - Smart Interview Platform 🎯

HireRoom is a modern technical interview platform that combines real-time video calls with an integrated code editor, making technical interviews seamless and efficient.

![HireRoom Logo](public/icon.svg)

## Features ✨

- **Real-time Video Calls** - Smooth video communication using Stream SDK
- **Integrated Code Editor** - Built-in Monaco editor with multiple language support
- **Interview Scheduling** - Easy-to-use interface for scheduling and managing interviews
- **Role-based Access** - Separate interfaces for interviewers and candidates
- **Interview Dashboard** - Track and manage all interviews in one place
- **Pass/Fail System** - Quick evaluation system for interviewers
- **Comments & Feedback** - Structured feedback system for better evaluation
- **Dark/Light Mode** - Comfortable viewing experience with theme support

## Tech Stack 🛠️

- **Frontend Framework**: Next.js 14
- **Styling**: Tailwind CSS
- **UI Components**: Shadcn UI
- **Authentication**: Clerk
- **Database & Backend**: Convex
- **Video SDK**: Stream
- **Code Editor**: Monaco Editor
- **State Management**: React Hooks + Convex
- **Type Safety**: TypeScript

## Getting Started 🚀

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Git

### Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

NEXT_PUBLIC_CONVEX_URL=your_convex_url

NEXT_PUBLIC_STREAM_KEY=your_stream_key
STREAM_SECRET=your_stream_secret
```

### Installation

1. Clone the repository

   ```bash
   git clone https://github.com/shivam-2101/HireRoom-app.git
   cd HireRoom-app
   ```

2. Install dependencies

   ```bash
   npm install
   # or
   yarn install
   ```

3. Start the development server

   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. Start the Convex backend
   ```bash
   npx convex dev
   ```

## Project Structure 📁

```
├── src/
│   ├── app/                 # Next.js app router pages
│   ├── components/         # Reusable components
│   ├── hooks/             # Custom React hooks
│   ├── lib/               # Utility functions
│   └── actions/           # Server actions
├── convex/                # Convex backend
├── public/               # Static assets
└── ...config files
```

## Key Features Explained 🔍

### Interview Flow

1. **Scheduling**: Interviewers can schedule interviews with candidates
2. **Joining**: Both parties join through unique meeting links
3. **Coding**: Real-time code collaboration during interview
4. **Evaluation**: Pass/Fail marking with feedback system

### Role-based Access

- **Interviewers**: Can schedule interviews, evaluate candidates, and provide feedback
- **Candidates**: Can view and join scheduled interviews

### Real-time Features

- Video calls with screen sharing
- Code editor with syntax highlighting
- Real-time compilation and execution
- Instant feedback and comments

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📝

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by Shivam Shukla
