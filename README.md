# 🦷 Oralix — Premium Dental Clinic Website

A modern, high-end dental clinic website built with HTML, CSS, and Three.js — featuring 3D animations, an appointment booking system, WhatsApp integration, and Google Maps.

> **Live site:** https://vyomprajapatii.github.io/oralix-dental-website  
> **GitHub Repo:** https://github.com/vyomprajapatii/oralix-dental-website

---

## ✨ Features

### 🎨 Design
- Premium, professional dental clinic aesthetic
- Full-screen hero with 3D animated tooth scene (Three.js)
- CSS 3D transforms on every card, button, and interactive element
- Scroll-triggered fade-up animations
- Fully responsive — works on mobile, tablet, and desktop

### 📞 Contact & Booking
- **2 booking forms** — hero quick-book card + dedicated contact section
- **FormSubmit.co integration** — form data goes directly to clinic email (no backend needed)
- **Sticky Call Now button** — appears on scroll, opens phone dialer instantly
- **Sticky WhatsApp button** — opens WhatsApp with pre-filled message
- **Google Maps embed** — with directions, call, and WhatsApp quick links

### 🤖 3D Animations
- **Three.js hero scene** — 3D tooth, orbiting mini-teeth, torus rings, floating particles
- **Blue + amber pulsing lights** — ambient atmosphere
- **Mouse-interactive camera** — subtle parallax follow on cursor movement
- **CSS 3D flips** — service numbers, icons, team card avatars all flip on hover
- **Floating tooth icons** — ambient background animation

### 📱 Sections
1. Hero + Quick Appointment Form
2. Trust Stats Strip ($8B+ managed, 65 IPOs, etc.)
3. About the Clinic
4. Services (4 departments)
5. How It Works — 4-step process
6. Before & After Gallery
7. Team Members
8. Patient Safety
9. Client Testimonials
10. CTA Banner
11. Visit Us — Google Maps + Address Strip
12. Contact Form + Info
13. Footer with Newsletter

---

## 🚀 Setup

### 1. Update the clinic details

Search and replace these placeholders in `oralix-replica.html`:

| Find | Replace With |
|---|---|
| `YOUR_EMAIL@domain.com` | Clinic's email address |
| `+919876543210` | Clinic's real phone number |
| `Oralix` | Your clinic name |
| Google Maps embed `src` | Your actual clinic location embed URL |

### 2. Activate booking emails (free)

The forms use [FormSubmit.co](https://formsubmit.co) — a free form-to-email service:

1. Replace `YOUR_EMAIL@domain.com` with your real email in the `action=""` attribute
2. Submit any form — you'll receive a confirmation email
3. Click the link in that email to activate auto-forwarding

### 3. Set up Google Maps

1. Go to Google Maps → search your clinic location
2. Click **Share** → **Embed a map**
3. Copy the `<iframe src="...">` URL
4. Replace the `src` in the map section

### 4. (Optional) Add WhatsApp Auto-Reply

For automated WhatsApp booking confirmations to both customer and clinic owner, see the **[WhatsApp Server Setup Guide](#option-a--baileys-free)** below.

---

## 📁 File Structure

```
oralix-dental-website/
├── oralix-replica.html    ← The complete website (single file)
├── README.md              ← You are here
└── LICENSE               ← MIT License
```

---

## 🛠️ WhatsApp Booking System (Optional)

For automated WhatsApp messages on every booking submission.

### Option A — Free (Baileys / Your Own Server)

```bash
# Install
npm install express body-parser cors whatsapp-web.baileys qrcode

# Run
node server.js   # Scan QR with clinic WhatsApp → live!
```

See full setup guide in the repository Wiki.

### Option B — Professional (Always Online)

| Service | Best For | Setup |
|---|---|---|
| **Wati** (₹999/month) | Indian clinics, non-technical | Easiest — paste widget code |
| **Gupshup** | India + analytics | Dashboard + JS snippet |
| **Twilio** | Developers, multi-channel | API keys + code |

---

## 📄 License

MIT — free to use, modify, and deploy for any purpose.
