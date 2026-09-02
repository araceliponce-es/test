Your repository starts as:

my-portfolio/
├── .github/
│   └── workflows/
│       └── portfolio.yml
├── bears.yml
├── custom.css
└── extra.css

The action builds it into:

my-portfolio/
├── .github/
├── bears.yml
├── custom.css
├── extra.css
└── dist/
    ├── index.html
    ├── output.css
    ├── custom.css
    └── extra.css

Then on .github/workflows/anything.yml:

path: ./dist

means only the distribution folder gets sent to GitHub Pages:

dist/
├── index.html
├── output.css
├── custom.css
└── extra.css
