<h1 align="center">✨ The Design Journey ✨</h1>

<p align="center">
  <strong>A modern, responsive, and visually stunning digital portfolio & creative showcase website</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Brand-The_Design_Journey-16f2b3?style=for-the-badge" alt="The Design Journey">
  <img src="https://img.shields.io/badge/Next.js-16.x-black?style=for-the-badge&logo=next.js" alt="Next.js">
  <img src="https://img.shields.io/badge/React-19.x-blue?style=for-the-badge&logo=react" alt="React">
  <img src="https://img.shields.io/badge/Tailwind_CSS-4.x-38B2AC?style=for-the-badge&logo=tailwind-css" alt="Tailwind CSS 4">
  <img src="https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge" alt="License">
</p>

<p align="center">
  <a href="#-overview">Overview</a> •
  <a href="#-contact-details">Contact Details</a> •
  <a href="#-key-features">Features</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-getting-started">Getting Started</a> •
  <a href="#-project-structure">Project Structure</a> •
  <a href="#-configuration">Configuration</a> •
  <a href="#-deployment">Deployment</a>
</p>

---

## 🌟 Overview

**The Design Journey** is a high-performance, dark-themed creative portfolio and digital agency showcase built with **Next.js 16**, **React 19**, and **Tailwind CSS 4**. Designed for modern design studios, creative directors, and digital product builders, it offers interactive Lottie animations, dynamic project highlights, blog integrations, and streamlined contact channels.

---

## 📬 Contact Details

The website is configured with official contact details for **The Design Journey**:

| Channel | Contact Detail |
| :--- | :--- |
| **Brand Name** | **The Design Journey** |
| **Email** | `contact@thedesignjourney.com` |
| **Phone** | `+1 (555) 234-5678` |
| **Address** | 123 Design Avenue, Suite 400, Creative District, New York, NY 10001, USA |
| **GitHub** | [github.com/TheDesignJourney](https://github.com/TheDesignJourney) |
| **LinkedIn** | [linkedin.com/company/the-design-journey](https://linkedin.com/company/the-design-journey) |
| **X / Twitter** | [@TheDesignJourney](https://twitter.com/TheDesignJourney) |
| **Facebook** | [facebook.com/TheDesignJourney](https://facebook.com/TheDesignJourney) |

---

## 🚀 Key Features

- 🎨 **Modern Brand Identity**: Tailored exclusively for **The Design Journey** with futuristic glowing gradients and dark UI aesthetics.
- ⚡ **Next.js 16 & React 19**: Leveraging React Server Components, fast streaming, server actions, and modern App Router patterns.
- 📱 **Streamlined Contact Channels**: Dedicated contact detail section (email, direct phone line, and physical studio address) matching The Design Journey brand.
- 📩 **Interactive Contact System**: Direct messaging form with instant validation, toast notifications, Nodemailer SMTP, and Telegram Bot alert support.
- 💻 **Interactive Hero & Code Studio**: Animated IDE code card presenting the studio’s design-to-code capabilities and technical philosophy.
- 🛠️ **Animated Skills Marquee**: Infinite smooth scrolling tech & tool display powered by `react-fast-marquee`.
- 📂 **Project Showcase**: Rich cards with interactive tags, preview links, and architectural descriptions.
- 📰 **Dev.to Blog Synchronization**: Auto-fetches and displays the latest design and development articles with graceful offline fallbacks.
- 🐳 **Container Ready**: Production and development Docker configurations included out of the box.
- 🔍 **SEO & Analytics Ready**: Metadata API with OpenGraph tags and Google Tag Manager (GTM) support.

---

## 💻 Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Framework** | Next.js 16 (App Router), React 19, React DOM 19 |
| **Styling** | Tailwind CSS 4, SASS / SCSS Modules, PostCSS |
| **Animations & UI** | Lottie Animations (`lottie-react`), `react-fast-marquee`, `react-icons`, `react-toastify` |
| **Backend / API** | Next.js Route Handlers (`/api/contact`), Nodemailer, Axios |
| **DevOps & Tooling** | Docker, Docker Compose, ESLint 9 |

---

## 🏁 Getting Started

### Prerequisites

Ensure you have the following installed:
- **Node.js**: v18.17.0 or higher (Node.js 20+ recommended)
- **Package Manager**: `pnpm` (recommended), `npm`, or `yarn`

```bash
node -v
pnpm -v # or npm -v
```

---

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/TheDesignJourney/the-design-journey.git
   cd the-design-journey
   ```

2. **Install project dependencies:**
   ```bash
   # Using pnpm (recommended)
   pnpm install

   # Or using npm
   npm install
   ```

3. **Configure Environment Variables:**
   ```bash
   cp .env.example .env
   ```
   Edit `.env` with your preferred credentials:
   ```env
   # Public URL
   NEXT_PUBLIC_APP_URL=http://localhost:3000

   # Contact Email (Nodemailer)
   EMAIL_ADDRESS=contact@thedesignjourney.com
   GMAIL_PASSKEY=your_16_character_app_password

   # Telegram Bot (Optional)
   TELEGRAM_BOT_TOKEN=your_telegram_bot_token
   TELEGRAM_CHAT_ID=your_telegram_chat_id

   # Analytics (Optional)
   NEXT_PUBLIC_GTM=GTM-XXXXXXX
   ```

4. **Run the Development Server:**
   ```bash
   pnpm dev
   # or
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser to view **The Design Journey**.

5. **Build for Production:**
   ```bash
   pnpm build
   pnpm start
   ```

---

## 📁 Project Structure

```text
The-Design-Journey/
├── app/
│   ├── api/
│   │   └── contact/route.js        # Contact email & Telegram notification handler
│   ├── blog/                       # Dedicated blog archive page
│   ├── components/
│   │   ├── footer.jsx              # Brand footer with navigation
│   │   ├── navbar.jsx              # Navigation bar featuring The Design Journey
│   │   ├── helper/                 # Lottie animations, GlowCard & ScrollToTop
│   │   └── homepage/
│   │       ├── about/              # "Who We Are" studio bio
│   │       ├── blog/               # Blog posts display
│   │       ├── contact/            # Contact form & contact details
│   │       ├── education/          # Education & milestones
│   │       ├── experience/         # Studio trajectory & timeline
│   │       ├── hero-section/       # Hero banner & studio code block
│   │       ├── projects/           # Showcase cards
│   │       └── skills/             # Skills marquee
│   ├── css/                        # Global & card SCSS styles
│   ├── layout.js                   # Root layout, metadata & GTM provider
│   └── page.js                     # Homepage assembly
├── public/                         # Brand icons, SVGs, and imagery
├── utils/
│   ├── check-email.js              # Email regex validator
│   └── data/
│       ├── contactsData.js         # Contact details & social channels
│       ├── personal-data.js        # Brand information, bios & channels
│       ├── projects-data.js        # Showcase projects data
│       ├── skills.js               # Skills listing
│       ├── experience.js           # Experience records
│       └── educations.js           # Educational background
├── Dockerfile.dev                  # Development Docker container
├── Dockerfile.prod                 # Production Docker multi-stage container
├── docker-compose.yml              # Docker Compose orchestration
├── package.json                    # Project configuration & scripts
└── README.md                       # Documentation
```

---

## ⚙️ Configuration

### Updating Brand & Contact Information

All content is managed through clean data files in the `utils/data/` directory:

- **`utils/data/personal-data.js` & `utils/data/contactsData.js`**:
  ```javascript
  export const personalData = {
    name: "The Design Journey",
    designation: "Creative Design & Digital Studio",
    email: "contact@thedesignjourney.com",
    phone: "+1 (555) 234-5678",
    address: "123 Design Avenue, Suite 400, Creative District, New York, NY 10001, USA",
    // ...
  };
  ```

- **`utils/data/projects-data.js`**: Add, update, or remove portfolio showcase items with tools, live demo links, and descriptions.

---

## 🐳 Docker Deployment

### Using Docker Compose
```bash
# Start container
docker-compose up -d --build

# View logs
docker-compose logs -f

# Stop container
docker-compose down
```

---

## 🚀 Cloud Deployment

### Vercel (Recommended)
1. Push your repository to GitHub.
2. Import the project on [Vercel](https://vercel.com).
3. Set your environment variables in the Vercel dashboard.
4. Deploy with automatic CI/CD on every push.

### Netlify
1. Connect your repository on [Netlify](https://netlify.com).
2. Set build command to `npm run build` and publish directory to `.next`.
3. Add environment variables in **Site Settings** & deploy.

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).

<p align="center">
  Crafted with ❤️ by <strong>The Design Journey</strong>
</p>
