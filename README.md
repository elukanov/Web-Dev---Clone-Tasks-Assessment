# Clone Task 1: Layout in React

Blog page for the Erased Tapes Records music label, built with React function components (Vite).

## Run the project

1. Install Node.js (LTS) from https://nodejs.org
2. Copy the images from the provided `assets` folder into `public/assets/`
3. Update the image filenames in `src/data/content.js` (and the logo in `src/components/Header.jsx`)
4. In a terminal inside this folder:

```
npm install
npm run dev
```

5. Open the address shown in the terminal (usually http://localhost:5173)

## Structure

```
src/
├── App.jsx               page layout
├── index.css             all styles (variables at the top)
├── data/content.js       text, links and image paths
└── components/
    ├── Header.jsx        logo + navigation
    ├── NavLinks.jsx      reused in header and footer
    ├── Article.jsx       title, intro, three-column text
    ├── Gallery.jsx       CSS Grid album layout
    ├── Author.jsx        bio, photo, social icons
    ├── SocialLinks.jsx   reused in author section and footer
    ├── Comments.jsx
    └── Footer.jsx
```

## Specification checklist

- Page background `#e9e9e9`, content white, footer `#14181d`
- Logo and author photo 200px wide; social icons 50px wide
- Standard spacing 50px; 10px between social icons
- Headings in "Protest Guerrilla" at 3rem (title larger); other text in "Josefin Sans"; first paragraph larger
- Layout: Flexbox (header, author, social icons, footer), CSS Grid (album gallery), CSS columns (article text)

## Design decisions (not in the spec)

- Content column capped at 900px and centred
- Body text uses a 1.6 line height; intro and comments limited to 60ch for readability
- Comments section uses the page grey, as drawn in the wireframe
- Links have visible focus styles; all images have alt text
