# MediBridge - Doctor Appointment Platform

A modern healthcare platform that connects patients with verified doctors for seamless appointment booking and video consultations.

## ✨ Features

- 🔐 **Secure Authentication** - Powered by Clerk
- 👨‍⚕️ **Doctor Verification** - Admin-approved healthcare professionals
- 📅 **Smart Scheduling** - Easy appointment booking with availability management
- 💬 **Video Consultations** - Integrated video calling via Vonage
- 💳 **Credit System** - Flexible payment and consultation credits
- 📱 **Responsive Design** - Mobile-first approach with Tailwind CSS
- 👑 **Admin Dashboard** - Comprehensive management tools

## 🚀 Tech Stack

- **Framework**: Next.js 15
- **Database**: PostgreSQL with Prisma ORM
- **Authentication**: Clerk
- **UI Components**: Radix UI + Tailwind CSS
- **Video Calling**: Vonage/OpenTok
- **Deployment**: Ready for Vercel/Netlify

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Aashish-Jha-11/MediBridge.git
   cd MediBridge
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env.local
   ```
   
   Configure your `.env.local`:
   ```env
   DATABASE_URL="your_postgresql_url"
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="your_clerk_key"
   CLERK_SECRET_KEY="your_clerk_secret"
   VONAGE_API_KEY="your_vonage_key"
   VONAGE_API_SECRET="your_vonage_secret"
   ```

4. **Set up the database**
   ```bash
   npx prisma migrate dev
   npx prisma generate
   ```

5. **Start the development server**
   ```bash
   npm run dev
   ```

Visit `http://localhost:3000` to see the application.

## 📝 User Roles

- **Patients**: Book appointments, join video calls, manage credits
- **Doctors**: Set availability, conduct consultations, track earnings
- **Admins**: Verify doctors, manage payouts, oversee platform

## 🔧 Database Schema

Key models include:
- **User** - Patients, doctors, and admins
- **Appointment** - Booking and consultation records
- **Availability** - Doctor scheduling
- **CreditTransaction** - Payment tracking
- **Payout** - Doctor earnings management

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Support

For support or questions, please open an issue on GitHub.

---

Built for better healthcare accessibility
