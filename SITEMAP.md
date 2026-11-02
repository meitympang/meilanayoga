# Meilana Yoga website: site map and setup

Domain: meilanayoga.co.uk
Email: meilanayoga@icloud.com
Instagram: @meilana_yoga (https://www.instagram.com/meilana_yoga/)
Booking: Bookwhen (https://bookwhen.com/meilanayoga)

Open `index.html` in a browser to look around. Every page shares the same header, footer and styles.

## Site map

```
Home (index.html)
├── Classes & timetable (classes.html)       weekly classes, prices, booking info
├── Styles (styles/index.html)                comparison of the three styles
│   ├── Beginners Hatha Yoga (styles/hatha.html)
│   ├── Energising Vinyasa Yoga (styles/vinyasa.html)
│   └── Restorative Yoga (styles/restorative.html)
├── Events & workshops (events.html)          workshops, seasonal, beach yoga, retreats
├── 1:1 sessions (private.html)               private and small-group sessions, packs
├── Workplace yoga (workplace.html)           corporate offer, links to the PDF brochure
├── About Mei (about.html)                     story, training, approach
├── Blog (blog/index.html)
│   ├── Welcome to Meilana Yoga (blog/welcome-to-meilana.html)
│   ├── Hatha or vinyasa: which is for you? (blog/hatha-vs-vinyasa.html)
│   └── Five desk stretches you can do right now (blog/desk-yoga.html)
└── Contact (contact.html)                    email, Instagram, Bookwhen
```

Folders:
- `assets/css/style.css` holds all the styles (brand pink, Cormorant Garamond and Montserrat)
- `assets/js/main.js` runs the mobile menu
- `assets/img/` is for your photos (empty for now)
- `assets/downloads/` holds the workplace brochure PDF

## Suggested prices (please check)

| What | Price |
| --- | --- |
| First class (new students) | £5 |
| Drop-in class | £10 (restorative 75 min £12, online £8, concessions £8) |
| 5-class pass, valid 8 weeks | £45 |
| 10-class pass, valid 16 weeks | £85 |
| 1:1 session, 60 min | £55 at home, £45 online |
| 1:1 packs | 3 for £150, 6 for £285 (online £120 / £225) |
| Small group private (2 to 4 people) | £70 (online £60) |
| Workshops (2 to 3 hours) | from £25, examples at £30 |
| Candlelit / seasonal | from £15, example at £18 |
| Beach yoga | £10 |
| Day retreat with lunch | from £45 for a half day, example full day £85 |

Local research found Woodbridge-area drop-ins at £8 to £9, Ipswich at £8 to £15, and 1:1 sessions at £40 to £70.

## Things to replace before going live

Search the files for `[` and `Example` to find them all.

1. **Timetable** (classes.html): the days, times and venues are examples. Replace each `[Venue, ...]`.
2. **Class size**: "capped at [12]" on classes.html.
3. **Events** (events.html): the four events, dates and venues are examples.
4. **Bookwhen link**: done. Every Book button uses https://bookwhen.com/meilanayoga. Add your classes, events and passes there so the buttons land on real listings.
5. **Photos**: done. Resized copies of 15 photos from the Yoga folder are in `assets/img/`, with clear names (for example `hatha-crescent-lunge.jpg`). To swap one, save a new photo over it with the same name, or add a new image like this:
   `<img src="assets/img/hero-teaching.jpg" alt="Mei teaching a hatha class" style="border-radius:16px">`
   (pages inside `styles/` or `blog/` need `../assets/img/...`)
6. **Registration**: the footer and About page say "Yoga Alliance registered". Change this if you're registered with BWY instead.
7. **Phone number**: it only appears on the Workplace page. Remove it if you'd rather not have it public.

Photos still worth taking: a desk yoga session in a real office (for the Workplace page) and a Felixstowe or Woodbridge beach class of your own.

## Setting up Bookwhen

- Create classes as a "course" with drop-in tickets, so people can book single classes or the whole term.
- Set up passes for the 5-class and 10-class options, and a £5 "first class" ticket limited to one per person.
- Add events as one-off listings, and 1:1 sessions as bookable appointments.
- Use the same email and Instagram in your Bookwhen profile.

## Putting it online

The simplest free route is Netlify Drop (https://app.netlify.com/drop). Drag the whole `website` folder onto the page and it goes live straight away. Then connect meilanayoga.co.uk in Netlify's domain settings. GitHub Pages or any web host also works, because the site is plain HTML.

## Editing

Each page is a normal HTML file. Open one in a text editor (TextEdit in plain-text mode, or VS Code) to change wording. The header and footer are repeated on every page, so a change to the menu or footer needs making on each page. Ask Claude to do that for you in one go.

New blog post: copy one of the files in `blog/`, change the text, and add a card for it on `blog/index.html`.
