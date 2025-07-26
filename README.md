
# DEVELOPMENT PROCESS

Enjoy the tour of my portfolio website re-developed with NextJS 😉

The website is developed using NextJS and this is the design of the project structure.
The structure might be changing depending on what has to be added to the portfolio at a given point in time

portfolio website/
│
├── public/                          
│   ├── images/
│   └── icons/
│
├── src/                            
│   ├── app/                        
│   │   ├── layout.tsx              # Root layout
│   │   ├── page.tsx                # Homepage
│   │
│   │   ├── github-projects/        # GitHub Projects page
│   │   │   ├── page.tsx
│   │   │   └── [id]/page.tsx       # Dynamic project detail page to highlight more about the project
│   │
│   │   ├── published-books/        # Published Books page to show the books that I have published before
│   │   │   ├── page.tsx
│   │   │   └── [slug]/page.tsx     # Book detail page to show more info about the book
│   │
│   │   ├── blogs/                  # Blog articles more about my blogs 
│   │   │   ├── page.tsx
│   │   │   └── [slug]/page.tsx     # Blog detail page
│   │
│   │   ├── social-media/           # Social Media platforms page to show my social media pages and links to them
│   │   │   └── page.tsx
│   │
│   │   ├── shop/                   # Shop/Product listings listing all my publications 
│   │   │   ├── page.tsx
│   │   │   └── [slug]/page.tsx     # Product details page 
│   │
│   │   ├── skills/                 # Skills page hifhlighing my skills 
│   │   │   └── page.tsx
│
│   ├── components/                 # The are the Reusable components I use throughout the project to avoid repetitions.
│   │   ├── Navbar.tsx
│   │   ├── Footer.tsx
│   │   ├── ProjectCard.tsx
│   │   ├── BookCard.tsx
│   │   ├── BlogCard.tsx
│   │   └── ProductCard.tsx
│
│   ├── styles/                     # CSS/SCSS/Modules
│   │   ├── globals.css
│   │   └── components/
│
│   ├── lib/                        # Utilities (API calls, helpers)
│   │   ├── fetchGithub.ts
│   │   ├── fetchBooks.ts
│   │   ├── fetchBlogs.ts
│   │   └── fetchProducts.ts
│
│   ├── constants/                  # Reusable constants
│   │   └── siteData.ts
│
│   └── types/                      # TypeScript interfaces
│       ├── project.d.ts
│       ├── book.d.ts
│       ├── blog.d.ts
│       └── product.d.ts
│
├── .env.local                      # Environment variables to store the secret keys that I might use in this project.
├── next.config.js
├── package.json
├── tsconfig.json
└── README.md                       # Well, this is the file you are reading right now 😉. 
# my-portfolio-website
