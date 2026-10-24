# Salone Trails

A responsive five-page travel website that helps visitors discover beaches, wildlife, history and mountains in Sierra Leone, and plan a trip with local guides. Built with HTML and CSS only (no JavaScript).

## 1. Project overview

Salone Trails is a travel website that helps visitors discover beaches, wildlife, history and mountains in Sierra Leone, and plan a trip with local guides. The site was designed from wireframes for five pages (Home, About, Services, Explore and Contact) and then developed into a realistic, responsive website.

## 2. Pages

| Page | File | Purpose |
|---|---|---|
| Home | `index.html` | Hero banner with "Plan your trip" and "Explore places" buttons, a feature strip (local guides, safe transport, great stays, fast support), four category cards and a call to action |
| About | `about.html` | Introduction to Sierra Leone and four travel-fact tiles (Nov to Apr, Visa, English, Leone) |
| Services | `services.html` | Four service cards (Guided Tours, Stay, Transport, Culture) and a three-step "How it works" section |
| Explore | `explore.html` | Six destinations with category filters, bookmarks and a "View saved trip" button |
| Contact | `contact.html` | Inquiry form (name, email, date, message) beside WhatsApp, phone and email links |

### Screenshots

**Home**

![Home page](screenshots/home.jpg)

**About**

![About page](screenshots/about.jpg)

**Services**

![Services page](screenshots/services.jpg)

**Explore**

![Explore page](screenshots/explore.jpg)

**Contact**

![Contact page](screenshots/contact.jpg)

## 3. Technologies used

- **HTML5** for the structure and content of every page
- **CSS3** for layout, colours, hover effects and responsive design (Flexbox, Grid, media queries, CSS variables)
- **Font Awesome 6.5.1** for icons (loaded from a CDN)
- **Google Fonts (Poppins)** for typography (loaded from a CDN)

No JavaScript is used anywhere in the project, as required.

> An internet connection is needed to load the icons and the font. If they are offline, the site still works, but icons will not appear and a default font is used.

## 4. How the interactive parts work without JavaScript

| Feature | Technique |
|---|---|
| Mobile menu button | A hidden checkbox plus the CSS sibling selector (`:checked ~ nav`) |
| About page travel-fact tiles | Radio buttons and labels, with CSS showing the text of the selected tile |
| Explore category filters | Radio buttons with the CSS `:has()` selector, which hides cards that do not match |
| Bookmarks and saved trip | Checkboxes styled as bookmark icons, with the saved list shown through CSS |
| Contact form checks | Built-in HTML rules: `required`, `type="email"`, `minlength` |
| Hover effects and animations | CSS `:hover` and `transition` |

## 5. Design decisions

- **Wireframes first.** The five pages follow the layout order of the original wireframes: header with logo and menu, hero with a "Plan your trip" button, four category cards, the About image beside text and four fact tiles, four service cards, the Explore search and filter area, and the Contact form beside WhatsApp, phone and email links.
- **Colour palette.** Green `#1eb53a` (inspired by the Sierra Leone flag), a dark green-black `#0e1b14`, white and a soft sand `#f6f1e7`. All colours are stored as CSS variables in `:root`, so the theme can be changed in one place.
- **Typography.** Poppins, in weights 400 to 700.
- **Photography.** Real photos replace the grey placeholder boxes in the wireframes. A dark gradient is laid over photos so white text stays readable.
- **Consistent layout.** Every page shares the same header (logo, menu and green Contact button), the same dark footer with WhatsApp, email and phone icons, and a green call-to-action band where it fits.
- **Responsive layout.** Media queries at 900 px, 800 px and 640 px change the grids from four columns to two and then one, and the menu collapses into a button on phones.
- **Accessibility.** Descriptive `alt` or `aria-label` text, semantic tags (`header`, `nav`, `main`, `section`, `footer`), visible focus outlines and sufficient text contrast.

## 6. Folder structure

```
salone-trails/
├── index.html
├── about.html
├── services.html
├── explore.html
├── contact.html
├── README.md
├── css/
│   └── style.css
├── screenshots/
│   └── home.jpg  about.jpg  services.jpg  explore.jpg  contact.jpg
└── images/
    ├── hero.jpg  beach.jpg  wildlife.jpg  history.jpg  mountain.jpg
    ├── about.jpg  contact.jpg
    └── tokeh.jpg  loma.jpg  tacugama.jpg  river2.jpg  banana.jpg  bunce.jpg
```

## 7. How to run the project

**Option A: open directly**
1. Open the `salone-trails` folder.
2. Double-click `index.html`. It opens in your browser.

**Option B: VS Code with Live Server**
1. Open the folder in VS Code (File > Open Folder).
2. Install the **Live Server** extension.
3. Right-click `index.html` and choose **Open with Live Server**.

## 8. Testing

- Checked every menu and footer link on all five pages.
- Tested the phone layout using Chrome DevTools (`F12`, then `Ctrl + Shift + M`).
- Tested the contact form with an empty form, an invalid email and a valid entry.
- Tested the Explore filters and bookmarks.
- Confirmed all file names are lowercase so links and images work on web servers.

## 9. Known limitations

- **Search box does not work.** The Explore page shows a "Search places" box to match the wireframe, but searching text needs JavaScript. Visitors use the category filters (All, Beaches, Wildlife, History, Mountain) instead.
- **Bookmarks are not remembered.** Saved places are cleared when the page is reloaded, because remembering them needs JavaScript or a server.
- **Form delivery.** The inquiry form opens the visitor's email app. It does not send messages from a server.
- **Contact details.** Check that the phone number and email address shown on the Contact page are the ones you want to publish.

## 10. Future improvements

- Add a backend or a form service to receive inquiries directly.
- Add a working search feature and permanent saved trips (this would need JavaScript).
- Add more destinations and a booking calendar.
- Add a French or Krio language option.

## 11. Credits

- Photographs: [Unsplash](https://unsplash.com) and [Pexels](https://www.pexels.com). [Add the photographer names for each image you used.]
- Icons: [Font Awesome](https://fontawesome.com) (free licence)
- Font: [Poppins](https://fonts.google.com/specimen/Poppins) on Google Fonts (Open Font Licence)
- Wireframes: designed by the student for this assignment.
