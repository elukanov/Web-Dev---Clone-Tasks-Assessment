# Clone Task 2: Responsive Layouts (watch.it)

Movie streaming page built with React function components (Vite), using Flexbox, Grid and media queries.

## Run the project

1. Install Node.js (LTS) from https://nodejs.org
2. Copy the images from the provided `assets` folder into `public/assets/`
3. Update titles, descriptions and poster filenames in `src/data/movies.js`
4. In a terminal inside this folder:

```
npm install
npm run dev
```

5. Open the address shown in the terminal (usually http://localhost:5173)

## Breakpoints

| Device  | Width        | Layout |
| ------- | ------------ | ------ |
| Mobile  | 360-720px    | One column, no nav, Search button beside logo |
| Tablet  | 720px and up | Nav appears, 2-column card grid, 32px large spacing |
| Desktop | 1024px and up | Featured card, two cards side by side, three wide cards, 48px large spacing |

Large spacing is a CSS variable (`--space-large`: 16px / 32px / 48px); small spacing is always 16px.

## Structure

```
src/
├── App.jsx               header + content container
├── index.css             all styles (variables and media queries)
├── data/movies.js        movie content and genres
└── components/
    ├── Header.jsx        logo, genre nav, Search button
    └── MovieCard.jsx     poster, text, Watch now button
```

## Specification checklist

- Colours from the watch.it palette (#070410, #231651, #4DCCBD, #EEF36A, #FFFFFF)
- Content container max width 900px
- Fonts: "Teko" for headings and buttons, "Lato" for other text
- Logo 2em on mobile, 3em on tablet and desktop; cards 1.5em; buttons 2em
- Header: large spacing between nav options, small spacing elsewhere
- Cards and buttons use small spacing; buttons use a 16px border radius

## Testing

Use browser dev tools to check 360px, 719px, 720px, 1023px and 1024px, plus 768px and 1280px.
