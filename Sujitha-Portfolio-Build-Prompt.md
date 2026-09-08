# Master Prompt: Data Analyst Portfolio Website for Sujitha Suresh

Copy everything below into a new chat with Claude (or another coding-capable AI) to generate the full site in one pass.

---

## PROMPT START

You are a senior frontend developer, UI/UX designer, and technical recruiter rolled into one. Build a **premium, modern, subtly animated data-analyst portfolio website** — the visual quality should be comparable to a top-tier Dribbble landing page (dark UI, glassmorphism, confident whitespace, restrained motion), but the content strategy must be optimized for **passing real Data Analyst interview screenings**, not for looking flashy.

### Candidate details
- **Name:** Sujitha Suresh
- **Title:** Aspiring Data Analyst | SQL · Power BI · Python · Excel
- **Location:** India
- **Profile photo:** I will supply `profile.jpg` — use it as the hero/about portrait (professional headshot, plain background). Do not generate or substitute a different photo.
- **LinkedIn:** https://www.linkedin.com/in/sujitha-suresh
- **GitHub:** `YOUR_GITHUB_URL` (placeholder — I'll fill in)
- **Resume:** `const resumeURL = "YOUR_RESUME_URL";` (placeholder — I'll fill in)

### What the site must communicate in the first 5 seconds
"She is a Data Analyst who works with SQL, Excel, Python and Power BI, and has actually built projects." Professional, technical, modern, interview-ready — never childish, template-y, or overloaded with neon/gaming aesthetics.

---

## 1. Tech stack
- HTML5, CSS3 (with CSS custom properties for all colors/spacing), vanilla JavaScript
- Optional, only where they genuinely add value: GSAP, Lucide icons, AOS/Intersection Observer for scroll reveals, Chart.js for real chart widgets
- No heavy frameworks unless justified
- Fully responsive (mobile, tablet, desktop), fast-loading, SEO-friendly, accessible (WCAG basics — alt text, focus states, contrast, keyboard nav), GitHub Pages–deployable
- File structure: `index.html`, `css/style.css`, `js/script.js`, `assets/images/`, `assets/projects/`, `assets/icons/` — no giant single-file dump, clean semantic HTML, commented JS with reusable functions

## 2. Visual direction
Dark, premium, "modern data analyst + BI + tech" mood — not a gaming site.
- Deep navy/black background, glassmorphism cards, soft gradients, subtle glow accents
- Accent palette via CSS variables: cyan/blue + purple accent + green for positive analytics indicators, white/off-white text
- Subtle background grid + light floating particles, animated data points/line charts used sparingly as texture, not distraction
- Clean typography (a strong sans-serif pairing), generous spacing, minimal but impressive — think Dribbble-grade landing page polish
- Motion budget: tasteful entrance/scroll-reveal animations, hover lift + glow on cards, magnetic hover on primary buttons, animated counters, skill bars, and a self-drawing timeline — nothing that hurts load performance or feels gimmicky

## 3. Signature visual concept (use throughout the site)
A recurring "pipeline" motif: **RAW DATA → CLEANING → SQL/PYTHON ANALYSIS → POWER BI → INSIGHTS → BUSINESS DECISIONS**, expressed as:
- An animated data-stream visual in the hero (particles flowing left to right through pipeline stages, ending in the line "DATA → INSIGHTS → DECISIONS")
- A dedicated animated "Analytics Workflow" section using the same stage names, each with its associated tools listed underneath, animating in on scroll

## 4. Page sections (in nav order)
**Sticky nav:** Home · About · Skills · Workflow · Projects · Dashboards · Certifications · Experience · Resume · Contact — background changes on scroll, mobile hamburger menu.

**Hero**
- H1: "Hi, I'm Sujitha Suresh"
- Subheading: "Data Analyst | SQL | Power BI | Python | Excel"
- Supporting line: "I transform raw data into meaningful insights, interactive dashboards, and business-ready decisions."
- Typing animation cycling: Data Analyst / SQL Developer / Power BI Analyst / Python Data Analyst / Business Intelligence Enthusiast / Data Visualization Enthusiast
- CTAs: "View My Projects" and "Download Resume"; secondary icon links to GitHub, LinkedIn, Email
- Floating glass dashboard card with animated counters, e.g. Total Sales ₹45.93L · Total Orders 10K+ · Average Sales ₹XXXX (mark placeholder numbers clearly if not real)
- "Scroll to explore" micro-animation

**About**
- Entry-level-appropriate copy: hands-on experience with Excel, SQL, Power BI, Python; enjoys cleaning/transforming/analyzing/visualizing data to uncover business insights; focus on turning raw datasets into dashboards and recommendations. No exaggerated claims.
- Animated portrait area using the supplied headshot
- Skill-focus cards: Data Cleaning, Data Analysis, Data Visualization, Business Intelligence, Dashboard Development, SQL Analytics

**Skills** (interactive, grouped, with honest proficiency labels — Advanced / Strong / Intermediate / Working Knowledge, never "Expert")
- **Data Analytics:** Excel, Advanced Excel, Data Cleaning, Data Transformation, Data Validation, Pivot Tables, Pivot Charts, Power Query, Data Analysis
- **SQL:** Advanced SQL, SELECT, WHERE, GROUP BY, HAVING, JOINs, Subqueries, CTEs, CASE statements, Window Functions (ROW_NUMBER, RANK, DENSE_RANK), Aggregations, Indexes, Stored Procedures, Triggers, Transactions/ACID, Isolation Levels, Query Optimization, EXPLAIN
- **Power BI:** Power BI, Power Query, Data Modeling, DAX, KPI Development, Interactive Dashboards, Slicers, Drill-through, Data Visualization, Business Intelligence
- **Python:** Python, Pandas, NumPy, Matplotlib, Seaborn, Data Cleaning, Data Manipulation, EDA, Data Visualization
- **Tools:** MySQL, Excel, Power BI, Git, GitHub, VS Code, Jupyter Notebook
- Animated bars or circular indicators on scroll

**Analytics Workflow** — animated pipeline per the signature concept above, each stage with tools listed (e.g., Raw Data → Excel/CSV; Cleaning → Python/Pandas/Power Query; Analysis → SQL/Python; Visualization → Power BI/Matplotlib/Seaborn; Insights → Business Recommendations)

**Projects** — the strongest section. Animated grid; each card shows project name, business problem, tools, key analysis, key insights, preview, GitHub button, Live Demo button if available. Clicking a card opens an animated detail modal with: Project Overview, Business Problem, Dataset, Tools, Data Cleaning, Analysis, Visualization, Key Insights, Business Recommendations, GitHub, Live Dashboard. Use real screenshots where I provide them, clearly labeled placeholders otherwise — never fabricate a screenshot.

1. **Retail Sales Analytics** — Python, Pandas, NumPy, Excel, MySQL, Power BI. Workflow: Excel data → Python cleaning → MySQL → SQL analysis → Power BI dashboard. KPIs: Total Sales, Average Sales, Regional Sales, Product Performance, Monthly Sales Trend.
2. **E-Commerce Analytics** — Excel, Python, SQL, Power BI. KPIs: Total Sales, Total Profit, Total Orders, Total Customers, AOV. Analysis: category sales, top 10 products, sales by country, payment method, order status, monthly trend, product ranking.
3. **Sales Performance Dashboard** — Excel, Power BI, SQL. KPI cards, sales by region/product, monthly trend, category analysis, interactive slicers.
4. **Netflix Content Analytics Dashboard** — Power BI, Excel. Movies vs TV shows, content by country, release trends, genres, ratings, content growth.
5. **Airbnb Analytics** — Excel, Power BI, SQL. Listings, price, availability, neighbourhood, room type, reviews, revenue metrics.
6. **Car Sales Analytics** — Excel, SQL, Power BI. Sales, vehicle categories, brands, models, price trends, regional performance.
7. **Customer Churn Analysis** — Python, Pandas, SQL, Power BI. Churn rate, customer segments, contract type, tenure, revenue patterns, high-risk segments.
8. **Titanic Classification** — Python, Pandas, NumPy, Matplotlib, Seaborn, ML. Present as a secondary/exploratory ML project, not a core analyst project.

**Power BI Dashboard Gallery** — large visual cards per dashboard (preview image, title, KPIs, tools, "View Dashboard," "GitHub"), hover animation, click-to-enlarge lightbox.

**SQL Analytics** — interactive code cards demonstrating JOINs, GROUP BY, CASE, CTEs, window functions (RANK, ROW_NUMBER, DENSE_RANK), subqueries, aggregations, query optimization. Include a real example, e.g.:
```sql
SELECT region, SUM(sales) AS total_sales
FROM sales
GROUP BY region
ORDER BY total_sales DESC;
```
Tagline: "SQL is one of my core analytical skills."

**Python Data Analytics** — animated flow Python → Pandas → NumPy → Data Cleaning → EDA → Matplotlib → Seaborn → Insights, with real snippet examples (`read_csv`, `info()`, `describe()`, `isnull()`, `fillna()`, `groupby()`, `merge()`, `sort_values()`, `value_counts()`).

**Excel Analytics** — Advanced Excel, Pivot Tables/Charts, Power Query, Data Cleaning, Data Validation, Lookup functions, Conditional Formatting, Dashboard development — shown via an animated spreadsheet-style component.

**Certifications & Learning** — cards for completed/relevant items only (e.g. Python Programming, Advanced Google Analytics, Meta Data Analyst Professional Certificate, NPTEL, AWS Academy, Wipro TalentNext, Infosys Springboard, VOIS Python Data Visualization, Power BI/Excel training). Each: name, platform, year, "View Certificate" button — use a placeholder if no link exists. Never fabricate certificate IDs.

**Experience / Training** — vertical animated timeline (role, organization, duration, skills, what was worked on) covering verified items only (e.g. Data Science Intern, Python Development Intern, RPA Developer Virtual Internship, Python/Data Analytics Training, VOIS Python Data Visualization). Do not invent responsibilities.

**Resume CTA** — Heading "Want to know more about my journey?"; text "Download my resume to explore my technical skills, projects, education and certifications."; "Download Resume" (uses `download` attribute) and "View Resume" (`target="_blank"`) buttons wired to the `resumeURL` config variable — no fake URL.

**GitHub & LinkedIn** — prominent icon buttons with hover animation, linking to the real LinkedIn URL above and the GitHub placeholder.

**Contact ("Let's Connect")** — "I'm open to Data Analyst opportunities, internships, and projects where I can use data to solve real business problems." Email, LinkedIn, GitHub links; a contact form UI (Name, Email, Message) that either uses `mailto:` or clearly states backend integration is required — never fake a "message sent" confirmation without a real backend.

**"How I Approach Data Problems"** — 5 steps: 1) Understand the business problem, 2) Collect and inspect data, 3) Clean and transform data, 4) Analyze and visualize, 5) Communicate insights and recommendations. Line: "I focus not only on creating dashboards, but on understanding what the data means for the business."

**Recruiter View** — a toggle button that reveals a compact summary card: Candidate name, Role, Core Skills (SQL | Power BI | Python | Excel), Strong Areas, Project list, and quick links to Resume/LinkedIn/GitHub — designed to be screen-shared or skimmed in under 20 seconds during an interview.

**Footer** — Name, title, tagline "Turning data into insights.", LinkedIn/GitHub/Email links, © 2026 Sujitha Suresh.

## 5. Animation rules
- Load: logo fade-in, nav slide-in, hero text reveal, typing effect, floating dashboard card, animated counters
- Scroll: section reveals, staggered card entrances, skill bars filling, self-drawing timeline, workflow pipeline connecting
- Hover: card lift + soft glow + border animation, icon micro-motion, magnetic buttons
- Smooth scrolling throughout; keep total animation weight light enough that performance stays fast

## 6. SEO & metadata
- `<title>Sujitha Suresh | Data Analyst Portfolio</title>`
- Meta description: "Data Analyst portfolio of Sujitha Suresh showcasing SQL, Power BI, Excel, Python, data visualization, dashboards and analytics projects."
- Open Graph tags, favicon

## 7. Hard content rules — never violate these
- Never invent job experience, companies, project results, salary figures, certificate IDs, GitHub URLs, dashboard URLs, client names, or business metrics.
- Where real data isn't provided, use clearly labeled placeholders (`YOUR_GITHUB_URL`, `YOUR_RESUME_URL`, `YOUR_PROJECT_IMAGE`) — never silently fabricate.
- Keep skill-level language honest and entry-level-appropriate.
- All personal info (name, links, resume URL, placeholders) should live in one clearly marked config section for easy editing later.

## 8. Deliverable
Provide the complete project: folder structure, `index.html`, `style.css`, `script.js`, the assets folder structure, and short instructions for (1) adding project images, (2) adding the resume, (3) adding certificate links, (4) deploying to GitHub Pages. Before calling it done, mentally verify: all nav links work, mobile menu works, resume/GitHub/LinkedIn links work, project buttons work, animations run smoothly, layout is responsive with no horizontal scroll, no broken images, and no obvious accessibility gaps.

## PROMPT END

---

### How to use this
1. Paste the prompt block above into a fresh conversation.
2. Attach `profile.jpg` and, if you have them, your resume PDF and any real dashboard screenshots.
3. Fill in the `YOUR_GITHUB_URL` / `YOUR_RESUME_URL` placeholders once you have final links — search-and-replace is easy since they're isolated in one config spot.
