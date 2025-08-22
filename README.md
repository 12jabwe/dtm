[README.md](https://github.com/user-attachments/files/21940849/README.md)
# 🚀 Modern E-Commerce Multi-Platform System

A comprehensive e-commerce solution with separate frontend/backend architecture, dedicated admin interfaces for Web/iOS/Android, and full OAuth integration.

## 📁 Project Structure

```
ecommerce-system/
├── 📱 mobile-app/               # React Native Mobile App (iOS/Android)
│   ├── app/                     # Mobile app routes
│   ├── components/              # Mobile UI components
│   ├── hooks/                   # Mobile-specific hooks
│   └── package.json             # Mobile dependencies
├── 🌐 web-app/                  # React Web App
│   ├── src/                     # Web app source
│   ├── public/                  # Web assets
│   └── package.json             # Web dependencies
├── 👑 admin-web/                # Admin Web Dashboard
│   ├── src/                     # Admin web interface
│   └── package.json             # Admin web dependencies
├── 📱 admin-mobile/             # Admin Mobile App
│   ├── app/                     # Admin mobile routes
│   └── package.json             # Admin mobile dependencies
├── 🔧 backend/                  # Supabase Backend
│   ├── supabase/                # Supabase configuration
│   ├── functions/               # Edge functions
│   └── database/                # Database schemas
├── 🔗 shared/                   # Shared utilities
│   ├── types/                   # TypeScript types
│   ├── services/                # API services
│   └── constants/               # Shared constants
└── 📋 docs/                     # Documentation
```

## 🚀 Getting Started

### 1. Clone & Setup
```bash
git clone <your-repo>
cd ecommerce-system
npm run setup:all  # Installs all dependencies
```

### 2. Environment Configuration
```bash
cp .env.example .env
# Add your Supabase credentials and OAuth keys
```

### 3. Database Setup
```bash
cd backend
supabase start
supabase db reset
npm run setup:admin
```

### 4. Start Development
```bash
# Terminal 1 - Mobile App
cd mobile-app && expo start

# Terminal 2 - Web App  
cd web-app && npm start

# Terminal 3 - Admin Web
cd admin-web && npm start

# Terminal 4 - Admin Mobile
cd admin-mobile && expo start
```

## 🎯 Platform Access

### 📱 **Mobile App** (Customer)
- **iOS**: Expo Go → Scan QR code
- **Android**: Expo Go → Scan QR code
- **Features**: Shopping, cart, wishlist, checkout

### 🌐 **Web App** (Customer)
- **URL**: http://localhost:3000
- **Features**: Full e-commerce experience

### 👑 **Admin Web Dashboard**
- **URL**: http://localhost:3001
- **Login**: admin@shop.com / admin123
- **Features**: Complete store management

### 📱 **Admin Mobile App**
- **Access**: Separate Expo app for admins
- **Features**: Mobile store management

## 🔐 Authentication Methods

### Customer Login
- ✅ Email/Password
- ✅ Google OAuth
- ✅ Apple Sign-In (iOS)
- ✅ Phone/SMS (Coming soon)

### Admin Login
- ✅ Email/Password (admin@shop.com)
- ✅ Google OAuth (admin accounts)
- ✅ Multi-factor authentication

## 🛠️ Backend Features

### Supabase Integration
- ✅ Real-time database
- ✅ Authentication & OAuth
- ✅ File storage
- ✅ Edge functions
- ✅ Row-level security

### API Endpoints
- 🔗 `/api/products` - Product management
- 🔗 `/api/orders` - Order processing  
- 🔗 `/api/users` - User management
- 🔗 `/api/admin` - Admin operations

## 👑 Admin Dashboard Features

### Product Management
- ✅ Add/Edit/Delete products
- ✅ Multi-image upload
- ✅ Inventory tracking
- ✅ Category management

### Order Management
- ✅ Order processing
- ✅ Shipping management
- ✅ Refund processing
- ✅ Order analytics

### User Management
- ✅ Customer profiles
- ✅ Admin accounts
- ✅ Role management
- ✅ Activity monitoring

### Payment Management
- ✅ Stripe integration
- ✅ PayPal integration
- ✅ Payment analytics
- ✅ Refund management

## 🚀 VS Code Live Preview

### Web Apps
1. **Install**: Live Preview extension
2. **Open**: `web-app/public/index.html`
3. **Preview**: Right-click → "Show Preview"

### Admin Dashboard
1. **Open**: `admin-web/public/index.html`
2. **Preview**: Admin interface in browser

## 📱 Mobile Development

### iOS Simulator
```bash
cd mobile-app
expo start --ios
```

### Android Emulator
```bash
cd mobile-app  
expo start --android
```

## 🔧 Development Commands

```bash
# Install all dependencies
npm run setup:all

# Start all services
npm run dev:all

# Build for production
npm run build:all

# Deploy to production
npm run deploy:all

# Database operations
npm run db:reset
npm run db:seed
npm run db:migrate
```

## 🌟 Key Features

### Multi-Platform
- 📱 Native iOS/Android apps
- 🌐 Progressive Web App
- 👑 Dedicated admin interfaces
- 🔄 Real-time synchronization

### Authentication
- 🔐 Multiple OAuth providers
- 🛡️ Role-based access control
- 📱 Biometric authentication
- 🔒 Session management

### E-Commerce
- 🛒 Shopping cart & wishlist
- 💳 Multiple payment methods
- 📦 Order tracking
- 🎯 Product recommendations

### Admin Management
- 📊 Real-time analytics
- 👥 User management
- 📦 Inventory control
- 💰 Payment processing

## 🚀 Production Deployment

### Vercel (Web Apps)
```bash
npm run deploy:web
npm run deploy:admin
```

### Expo EAS (Mobile Apps)
```bash
npm run build:mobile
npm run deploy:mobile
```

### Supabase (Backend)
```bash
npm run deploy:backend
```

## 🛡️ Security Features

- 🔒 Row-level security (RLS)
- 🛡️ API rate limiting
- 🔐 JWT token validation
- 📱 Biometric authentication
- 🚫 SQL injection protection

## 📞 Support

- 📧 **Email**: support@dopetzcom.com
- 📱 **Phone**: +1 (555) 123-4567
- 💬 **Chat**: Available in admin dashboard
- 📚 **Docs**: `/docs` folder

---

🎉 **Ready to launch your multi-platform e-commerce empire!**
