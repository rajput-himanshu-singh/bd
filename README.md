# 🎂 A Birthday Celebration for Ichha 🎈✨

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Canvas Confetti](https://img.shields.io/badge/Canvas_Confetti-FF69B4?style=flat)](https://www.npmjs.com/package/canvas-confetti)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An interactive birthday celebration for **Ichha**, sent with warm wishes from **Himanshu**. Built with vanilla HTML5, CSS3, JavaScript, and HTML5 Canvas particle effects, it includes six playful universes, a memory gallery, a magic wish reveal, a sliceable birthday cake, and a celebratory finale.

The birthday date, wishes, captions, photos, and music can all be adjusted before sharing Ichha's page.

---

## 🎮 Live Preview & Unlock Password

Use the preview query on your locally hosted or deployed site to open the celebration immediately:

| Access Method | Link / Details | Action |
|---|---|---|
| **🚀 Instant Preview** | Add `?preview=1` to your site URL | Opens the celebration without waiting for the configured birthday. |
| **🌐 Birthday Countdown** | Open the site without a query string | Shows the countdown using the date configured in `script.js`. |
| **🔑 Secret Unlock Password** | `birthday` *(all lowercase)* | Click the lock button on the countdown screen & enter this password to unlock! |

---

## 🌟 Key Interactive Features

1. **⏳ Live IST Countdown & Password Gate**
   - Real-time countdown timer locked until the exact birthday date.
   - Built-in instant preview bypass: append `?preview=1` or enter password `birthday`.
2. **🌌 6 Multiverse Character Universes**
   - **Universe 01 — Office Hours, Ichha Style 💻**: A supplied workday video and office candids.
   - **Universe 02 — The Candid Files 🎬**: Unplanned snapshots and behind-the-scenes laughs.
   - **Universe 03 — Saree-Day Spotlight 💜**: Ichha's festive looks and personal portrait.
   - **Universe 04 — The Little Throwback 📼**: Earlier chapters from the photo archive.
   - **Universe 05 — A Little Saree-Day Spin 💃**: The supplied saree-day video.
   - **Universe 06 — Ichha, Full Spotlight 👑**: A birthday portrait and personal wishes.
3. **🌳 Blooming Memory Tree & Polaroid Gallery**
   - Tap the heart tree to reveal all 27 supplied photos in sets of eight, with a zoomable lightbox.
4. **🎩 The Magic Wish Hat**
   - Interactive pullable ribbon: drag the ribbon upwards to unveil 6 heartfelt birthday wishes one by one with sparkler effects.
5. **🎂 Sliceable 3-Tier Cake with Candle Blowout**
   - Click or tap the birthday cake to slice through layers, extinguish the candle flame, and trigger realistic fireworks + confetti blast.
6. **🏹 Grand Finale: Crossbow Archery & Secret Envelope**
   - Pull back the crossbow arrow and fire at the royal wax heart to unseal the secret letter and royal birthday card!
7. **🎵 Smart Background Audio Engine**
   - Seamless background music with auto-pause when universe video showcases are playing.

---

## 🚀 How to Customize & Deploy (Step-by-Step)

You can update Ichha's birthday date, photos, favorite song, and wishes in a few steps:

### Step 1: Download or Clone the Code

Click the green **`< > Code`** button above and select **Download ZIP** (or run):
```bash
git clone https://github.com/Stark345/interactive-birthday-webpage.git
cd interactive-birthday-webpage
```

---

### Step 2: Personalize with Your Photos, Music & Text

#### A. Configure Birthday Details (`script.js`)
Open `script.js` in any text editor (VS Code, Notepad, etc.) and edit the `CONFIG` block at the top:

```javascript
const CONFIG = {
   birthdayMonth: 11,          // November
   birthdayDay:   28,          // Ichha's birthday
  timeZone:      "Asia/Kolkata", // Your timezone
  passcode:      "birthday",  // Change or keep your secret unlock password!
   friendName:    "Ichha",     // Birthday person's name

   // 27 photos in the scrapbook album
  gallery: [
      { caption: "The mirror caught us", stamp: "#Us", tilt: -2.5, img: "assets/images/ichha-memory-01.jpg", icon: "📸" },
      { caption: "Office hours, Ichha style", stamp: "#Workday", tilt: 3.2, img: "assets/images/ichha-memory-02.jpg", icon: "💻" },
      // ... continue through ichha-memory-27.jpg
  ],

  // 6 Magic Hat Wishes
  balloons: [
    { msg: "Stay wonderfully authentic and uniquely you, always!", icon: "🌈", cls: "b1" },
    // ... customize your 6 personal wishes
  ]
};
```

The countdown is set to November 28 for Ichha. For an immediate preview, add `?preview=1` to the URL.

#### B. Birthday Photos and Videos
- The 27 gallery photos are in `assets/images/ichha-memory-01.jpg` through `ichha-memory-27.jpg`.
- The finale portrait is `assets/images/ichha-portrait.jpg`.
- The office and saree-day clips are `assets/videos/ichha-workday.mp4` and `assets/videos/ichha-saree.mp4`.
- Gallery captions can be edited in the `CONFIG.gallery` array in `script.js`.
- **Music (`assets/audio/`)**:
   - Replace `song.mp3` with Ichha's favorite celebration song.
- **Videos (`assets/videos/`)**:
   - The office and saree-day clips are already connected to their matching pages.

---

### Step 3: Deploy for FREE in 60 Seconds

#### Option 1: Netlify Drag & Drop (Easiest - No Coding Required!)
1. Go to [Netlify Drop](https://app.netlify.com/drop) (sign in or create a free account).
2. Simply **drag and drop** your project folder into the upload box on Netlify.
3. Your site is live instantly! You will get a link like `https://your-name.netlify.app`.
4. *(Optional)* Go to **Site Configuration > Change site name** to give it a custom name (e.g., `birthday-wishes-for-ichha.netlify.app`).

#### Option 2: Deploy with GitHub Pages
1. Push your customized project to a new repository on your GitHub account.
2. In your GitHub repo, go to **Settings > Pages**.
3. Under **Branch**, select `main` and `/ (root)`, then click **Save**.
4. Your site will be published at `https://<your-username>.github.io/<repo-name>/`.

#### Option 3: Deploy with Vercel
1. Create a new GitHub repository under your account. This workspace still points to the original template repository, so do not import that upstream repository for Ichha's site.
2. Push this customized project, including `assets/images/` and `assets/videos/`, to your new repository.
3. In [Vercel](https://vercel.com/), choose **Add New Project** and import your new repository.
4. Choose **Other** as the framework preset. Leave the build and output directory overrides empty; this is a static HTML site.
5. Click **Deploy**, then share the generated `https://<project>.vercel.app/?preview=1` link to open the celebration immediately.

The deployed page and its photo/video asset URLs will be accessible online. A private GitHub repository does not make the deployed site or its media private.

---

## 📂 Project Structure

```
interactive-birthday-webpage/
├── index.html              # Main application page
├── script.js               # Central configuration, physics engine & interactions
├── style.css               # Responsive styling, animations & 3D transforms
├── assets/
│   ├── audio/
│   │   └── song.mp3
│   ├── images/
│   │   ├── ichha-portrait.jpg
│   │   └── ichha-memory-[01-27].jpg
│   └── videos/
│       ├── ichha-workday.mp4
│       └── ichha-saree.mp4
├── .gitignore              # Keeps your private media safe
├── LICENSE                 # MIT License
└── README.md               # Documentation & setup guide
```

---

## 🛡️ Privacy & Safety

- Built to ensure sensitive media is kept secure.
- Video and personal photo folders have gitignore protections so private media is never exposed publicly without intent.

---

## 📜 License

Distributed under the [MIT License](LICENSE). Feel free to use, modify, and share this celebration template to bring joy to your friends and loved ones!

Crafted with 💖 and creative coding by [S Jaichandran](https://github.com/Stark345).
