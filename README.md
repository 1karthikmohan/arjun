# Sonar - Social Media App

A modern social media application built with React, TypeScript, and Tailwind CSS that focuses on local connections and social verification.

## 🚀 Features

### Core Functionality
- **User Authentication** - Email/password login with OTP verification
- **Profile Management** - Customizable profiles with cover photos and bios
- **Social Media Verification** - OAuth integration for Instagram, Facebook, LinkedIn, Twitter, and Google
- **Local Discovery** - Radar feature to find nearby users
- **Messaging** - Real-time chat functionality
- **Content Sharing** - Photo/video posts with camera integration
- **Stories** - Temporary content sharing

### Social Verification System
- **OAuth Integration** - Verify ownership of social media accounts
- **Verified Badges** - Visual indicators for verified accounts
- **Trust Building** - Enhanced credibility through verified social presence
- **Multiple Providers** - Support for major social platforms

### Mobile-First Design
- **Responsive Layout** - Optimized for mobile devices
- **Touch Interactions** - Smooth animations and transitions
- **Native Feel** - iOS/Android-like user experience
- **Dark Theme** - Modern dark UI design

-## 🛠 Tech Stack

- **Framework**: Next.js 15 with the App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS with shadcn/ui components
- **Icons**: Heroicons, Tabler Icons
- **State Management**: React Hooks
- **Routing**: Component-based navigation
- **Authentication**: Mock OAuth flows (ready for backend integration)

## 📱 Screens

1. **Welcome Screen** - App introduction and onboarding
2. **Login/Signup** - Authentication with email verification
3. **Radar Screen** - Discover nearby users
4. **Feed Screen** - View posts from all users
5. **Create Post** - Share photos/videos with camera integration
6. **Messages** - Chat with other users
7. **Profile Screen** - User profiles with social verification
8. **Edit Profile** - Update profile information and verify social accounts

## 🔧 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd sonar-social
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:3000`

## 🏗 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── common/         # Common components (Avatar, SocialLinks)
│   ├── messaging/      # Chat-related components
│   ├── post/          # Post-related components
│   ├── profile/       # Profile components
│   ├── radar/         # Radar screen components
│   ├── social/        # Social verification components
│   └── story/         # Stories components
├── screens/            # Main application screens
├── data/              # Mock data and generators
├── hooks/             # Custom React hooks
├── types/             # TypeScript type definitions
├── utils/             # Utility functions
└── styles/            # CSS and styling
```

## 🔐 Social Media Authentication

The app includes a comprehensive social media verification system:

### Supported Platforms
- Instagram
- Facebook
- LinkedIn
- Twitter/X
- Google

### Verification Flow
1. User clicks "Connect" button for a social platform
2. OAuth flow initiates (currently mocked for demo)
3. User authorizes the application
4. Profile URL is retrieved and stored
5. Verified badge is displayed on user profile

### Implementation Notes
- OAuth flows are currently mocked for demonstration
- Ready for backend integration with real OAuth providers
- Secure token handling and profile verification
- Error handling for failed authentications

## 📊 Database Schema

The app is designed to work with the following database structure:

### Users Table
- Basic user information (name, email, bio, etc.)
- Profile and cover photo URLs
- Location data for radar functionality

### Social Accounts Table
- Verified social media accounts
- OAuth tokens and profile URLs
- Verification status and timestamps

### Posts Table
- User-generated content
- Media URLs and captions
- Timestamps and metadata

### Messages Table
- Chat functionality
- Sender/receiver relationships
- Message content and read status

## 🚀 Deployment

### Build for Production
```bash
npm run build
```


### Docker
You can build a production image using the provided `Dockerfile`:
```bash
docker build -t sonar-social .
docker run -p 3000:3000 sonar-social
```

### Progressive Web App
The project is configured as a PWA using `next-pwa`. When built for
production, the app can be installed on mobile devices and works offline.

## 🔮 Future Enhancements

- **Real-time Messaging** - WebSocket integration
- **Push Notifications** - Mobile notifications
- **Advanced Filtering** - Enhanced user discovery
- **Content Moderation** - Automated content filtering
- **Analytics Dashboard** - User engagement metrics
- **Premium Features** - Subscription-based enhancements

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- React team for the amazing framework
- Tailwind CSS for the utility-first styling
- Heroicons and Tabler Icons for beautiful icons
- All contributors and testers

---

**Note**: This is a demo application with mocked authentication flows. For production use, implement proper backend services and real OAuth integrations.