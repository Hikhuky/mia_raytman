# 🌟 Modern Bio Link (Linktree Alternative)

A minimalist, high-performance, and fully responsive personal Bio Link website built with vanilla HTML5, CSS3, and modern JavaScript.

---

## 🚀 Quick Setup & Customization

All personal details, avatar, links, and social accounts are configured inside the `userData` object located in `<script>` at the bottom of [`index.html`](file:///Users/hikhu/.gemini/antigravity/scratch/biolink/index.html).

### 1. Change Profile Info
Edit this block:
```javascript
const userData = {
  profile: {
    name: "Your Name",
    handle: "@yourhandle",
    bio: "Your short bio or elevator pitch goes here.",
    avatar: "https://your-domain.com/photo.jpg",
    verified: true,      // true | false (shows blue checkmark)
    activeStatus: true   // true | false (shows green active dot)
  },
  // ...
};
```

### 2. Add or Edit Links
Add as many items as you want to the `links` array:
```javascript
links: [
  {
    title: "🚀 My New Project",
    url: "https://example.com",
    icon: "rocket",       // rocket | book | podcast | coffee | briefcase | globe
    featured: true        // true highlights the link with a subtle gradient badge
  },
  {
    title: "☕ Buy Me a Coffee",
    url: "https://buymeacoffee.com",
    icon: "coffee",
    featured: false
  }
]
```

### 3. Change Themes in CSS (`:root`)
Change 3-4 hex variables inside `<style>` at line ~20:
```css
:root {
  --primary-color: #6366f1;       /* Main accent */
  --page-bg: #0b0f19;             /* Background base */
  --card-bg: rgba(255, 255, 255, 0.04);
  --btn-bg: rgba(255, 255, 255, 0.06);
}
```

### 4. Deploying to the Web (Free)
1. **GitHub Pages**: Push this file as `index.html` to a GitHub repository, go to Settings -> Pages, and enable GitHub Pages.
2. **Netlify Drop**: Simply drag-and-drop this folder onto [app.netlify.com/drop](https://app.netlify.com/drop).
3. **Vercel / Cloudflare Pages**: Deploy with zero build step needed.
