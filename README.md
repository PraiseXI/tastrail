# RatePlate Template

A template for building mobile and web applications using Expo, Supabase, PowerSync, and Clerk authentication. This template provides a solid foundation for creating offline-first applications with real-time synchronization capabilities.

## Tech Stack

- **Expo (React Native)**: Cross-platform mobile development
- **Supabase**: PostgreSQL database and backend services
- **PowerSync**: Offline-first data synchronization
- **Clerk**: Authentication and user management

## Environment Setup

Create a `.env` file in the root directory with the following variables:

```bash
# Clerk Authentication
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key

# Supabase Configuration
EXPO_PUBLIC_SUPABASE_URL=your_supabase_project_url
EXPO_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key

# PowerSync Configuration
EXPO_PUBLIC_POWERSYNC_URL=your_powersync_url
EXPO_PUBLIC_POWERSYNC_TOKEN=your_powersync_token
```

### How to get these values:

1. **Clerk Keys**:
   - Sign up at [clerk.com](https://clerk.com)
   - Create a new application
   - Get your publishable key from the Clerk dashboard

2. **Supabase Keys**:
   - Create a project at [supabase.com](https://supabase.com)
   - Go to Project Settings > API
   - Copy the URL and anon key

3. **PowerSync Configuration**:
   - Set up PowerSync in your Supabase project
   - Get the sync URL and token from your PowerSync dashboard

## Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```

2. Set up your environment variables as described above

3. Start the development server:
   ```bash
   npx expo start
   ```

## Project Structure

```
app/
├── _layout.tsx        # Root layout with authentication setup
├── (tabs)/           # Tab-based navigation
├── components/       # Reusable components
├── hooks/           # Custom hooks
├── lib/             # Utility functions and configurations
└── store/           # PowerSync store configuration
```

## Features

- Offline-first architecture with PowerSync
- Real-time data synchronization
- Secure authentication with Clerk
- Type-safe database operations
- Cross-platform compatibility

## Development Guidelines

- Follow SOLID principles
- Maintain clear logging for debugging
- Keep the codebase modular and maintainable
- Use the PowerSync local store as the primary data source
- Ensure proper synchronization between local and remote databases

## Learn More

- [Expo Documentation](https://docs.expo.dev/)
- [Supabase Documentation](https://supabase.com/docs)
- [PowerSync Documentation](https://docs.powersync.com)
- [Clerk Documentation](https://clerk.com/docs)

## License

MIT
