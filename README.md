# aiboro.ai

Action: file_editor create /app/README_GITHUB.md --file-text "# AIBoro - AI Agency Website

![AIBoro](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)
![React](https://img.shields.io/badge/React-19.0.0-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-0.110.1-green)

Premium AI automation agency website with modern design, full-stack functionality, and conversion-focused features.

## ✨ Features

### Frontend
- 🎨 **Premium Dark Theme** - Modern black background with cyan/blue gradients
- 📱 **Fully Responsive** - Perfect on all devices (mobile, tablet, desktop)
- ⚡ **Smooth Animations** - Glassmorphism effects and hover interactions
- 🎯 **Conversion-Focused** - Multiple CTAs and lead capture forms
- 🔧 **Modern Tech Stack** - React 19, Tailwind CSS, shadcn/ui components

### Sections
- ✅ Sticky Navigation with smooth scroll
- ✅ Hero Section with animated background
- ✅ Trusted By logos
- ✅ Services (6 AI services)
- ✅ Industries (8 target industries)
- ✅ How It Works (5-step process)
- ✅ Portfolio (success stories)
- ✅ Benefits (6 key advantages)
- ✅ Testimonials (client reviews)
- ✅ Pricing (3 tiers)
- ✅ FAQ (accordion)
- ✅ Contact Form (with backend)
- ✅ Strong CTA sections
- ✅ Comprehensive Footer
- ✅ WhatsApp floating button

### Backend
- 🔒 **Secure API** - FastAPI with input validation
- 💾 **MongoDB Storage** - Contact form submissions saved
- ✅ **Validation** - Email validation, field length checks
- 🚀 **Fast & Scalable** - Async operations

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ and npm/yarn
- Python 3.9+
- MongoDB (local or Atlas)

### Frontend Setup
```bash
cd frontend
yarn install
yarn start
```

Frontend runs on `http://localhost:3000`

### Backend Setup
```bash
cd backend
pip install -r requirements.txt

# Create .env file with:
# MONGO_URL=your_mongodb_connection_string
# DB_NAME=aiboro
# CORS_ORIGINS=http://localhost:3000

uvicorn server:app --reload --host 0.0.0.0 --port 8001
```

Backend runs on `http://localhost:8001`

## 📦 Tech Stack

### Frontend
- **Framework**: React 19
- **Styling**: Tailwind CSS
- **Components**: shadcn/ui
- **Icons**: Lucide React
- **HTTP Client**: Axios
- **Routing**: React Router DOM
- **Notifications**: Sonner (toast)

### Backend
- **Framework**: FastAPI
- **Database**: MongoDB with Motor (async)
- **Validation**: Pydantic
- **CORS**: Starlette middleware

## 🌐 Deployment

See [DEPLOYMENT_GUIDE.md](./DEPLOYMENT_GUIDE.md) for detailed deployment instructions including:
- GitHub Pages deployment
- Full-stack deployment (Render + GitHub Pages)
- Vercel deployment
- Environment configuration

## 📁 Project Structure

```
aiboro-website/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/          # shadcn components
│   │   │   ├── Navigation.jsx
│   │   │   ├── Hero.jsx
│   │   │   ├── Services.jsx
│   │   │   ├── Industries.jsx
│   │   │   ├── HowItWorks.jsx
│   │   │   ├── Portfolio.jsx
│   │   │   ├── Benefits.jsx
│   │   │   ├── Testimonials.jsx
│   │   │   ├── Pricing.jsx
│   │   │   ├── FAQ.jsx
│   │   │   ├── Contact.jsx
│   │   │   ├── CTA.jsx
│   │   │   └── Footer.jsx
│   │   ├── hooks/
│   │   ├── mock.js         # Static content data
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── tailwind.config.js
├── backend/
│   ├── server.py
│   ├── requirements.txt
│   └── models/
├── README.md
├── DEPLOYMENT_GUIDE.md
└── .gitignore
```

## 🎨 Design Features

- **Color Scheme**: Black, White, Cyan (#0EA5E9), Blue gradients
- **Typography**: Modern, clean sans-serif fonts
- **Components**: Glassmorphism cards with hover effects
- **Animations**: Fade-in, smooth scrolling, pulse effects
- **Mobile**: Hamburger menu, optimized layouts

## 🔧 API Endpoints

### POST /api/contact
Submit contact form
```json
{
  \"name\": \"string (required, min 2 chars)\",
  \"email\": \"string (required, valid email)\",
  \"phone\": \"string (optional)\",
  \"businessName\": \"string (optional)\",
  \"message\": \"string (required, min 10 chars)\"
}
```

### GET /api/contact
Retrieve all contact submissions (admin use)

## 🧪 Testing

Backend includes comprehensive test suite:
```bash
cd backend
pytest backend_test.py
```

All tests passing: ✅ 10/10 (100%)

## 📝 Environment Variables

### Frontend (.env)
```env
REACT_APP_BACKEND_URL=http://localhost:8001
```

### Backend (.env)
```env
MONGO_URL=mongodb://localhost:27017/
DB_NAME=aiboro
CORS_ORIGINS=http://localhost:3000
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- Design inspired by modern SaaS websites
- Icons from Lucide React
- UI components from shadcn/ui
- Built with React and FastAPI

## 📞 Contact

For business inquiries: contact@aiboro.com

---

**Built with ❤️ for AI automation agencies**
"
Observation: Create successful: /app/README_GITHUB.md