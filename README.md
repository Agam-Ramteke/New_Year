# 🎉 New Year Surprise

A delightful single-page Next.js site to celebrate the New Year with a special surprise message, beautiful animations, and confetti!

## ✨ Features

- 🎨 Beautiful design with festive colors and rounded cards
- 🎭 Smooth animations using Framer Motion
- 🎊 Confetti celebration on gift reveal
- 📱 Fully responsive and mobile-first
- ♿ Accessible with keyboard navigation and ARIA labels
- 🔔 Toast notifications for user feedback
- 🖼️ Photo grid for memories
- 📋 Copy message functionality

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm/yarn/pnpm

### Installation

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for Production

```bash
# Create production build
npm run build

# Start production server
npm start
```

### Other Commands

```bash
# Run linter
npm run lint

# Format code
npm run format

# Run tests
npm test
```

## 🎨 Customization

### Edit the Message

Edit the message content in `data/message.ts` to wish a Happy New Year:

```typescript
export const messageData = {
  title: 'Happy New Year 2026! 🎆',
  subtitle: 'Here is to new beginnings and amazing moments.',
  body: `As the clock strikes midnight, I want to wish you...`,
  // ...
};
```

### Change Colors

Update CSS variables in `styles/globals.css` for a festive look:

```css
:root {
  --bg: #0f172a;        /* Dark Blue/Black */
  --primary: #fbbf24;   /* Gold */
  --accent: #f87171;    /* Red/Pink */
  --text: #f8fafc;      /* White */
}
```

### Replace Images

Replace placeholder images in `components/PhotoGrid.tsx` or add your own images to `public/assets/`.

## 🚢 Deployment

### Deploy to Vercel (Recommended)

1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project" and import your repository
4. Vercel will automatically detect Next.js and deploy

**One-click deploy:**
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=YOUR_REPO_URL)

### Deploy to Render

1. Create a new account at [render.com](https://render.com)
2. Click "New +" → "Web Service"
3. Connect your GitHub repository
4. Use these settings:
   - **Build Command:** `npm run build`
   - **Start Command:** `npm start`
   - **Environment:** Node

## 📁 Project Structure

```
new-year-surprise/
├── components/
│   ├── Hero.tsx           # Hero section with animation
│   ├── MessageCard.tsx    # Animated message card
│   ├── PhotoGrid.tsx      # Photo grid/carousel
│   └── Confetti.tsx       # Confetti animation
├── data/
│   └── message.ts         # Message content (editable)
├── lib/
│   └── toast.ts           # Toast notifications
├── pages/
│   ├── _app.tsx           # App wrapper
│   └── index.tsx          # Main page
├── public/
│   └── assets/
│       └── crown.svg      # Icon asset (can be replaced with sparkle star)
├── styles/
│   └── globals.css        # Global styles & CSS variables
└── package.json
```

## 🛠️ Tech Stack

- **Next.js 14** - React framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Utility-first styling
- **Framer Motion** - Smooth animations
- **React Hot Toast** - Toast notifications

## 📝 License

Made with 💕 for the New Year
