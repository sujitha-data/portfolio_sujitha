# MASTER PROMPT — Sujitha Suresh Data Analyst Portfolio

Copy everything below into your AI code tool (Claude Code, Cursor, v0, etc.) as one message.

---

You are a senior frontend developer, UI/UX designer, and animation specialist. Build a premium, highly animated, interview-ready portfolio website for a data analyst. This is not a generic student portfolio — it must read as a polished junior/entry-level Data Analyst portfolio that a recruiter would trust.

## 1. CANDIDATE INFO
- Name: Sujitha Suresh
- Title: Aspiring Data Analyst | SQL | Power BI | Python | Excel
- Location: India
- Headshot / hero photo: `assets/images/profile-hero.jpg` (full-body, studio, black suit — use for hero section)
- Portrait: `assets/images/profile-portrait.jpg` (close-up headshot — use for About section)
> I'll supply both image files — reference them by these filenames, don't invent alt images.

## 2. TECH STACK
- HTML5, CSS3 (custom properties for theming), vanilla JavaScript
- Optional if genuinely useful: GSAP, Lucide Icons, Intersection Observer / AOS, Chart.js
- No unnecessary frameworks. No React/build tooling — must run as static files on GitHub Pages.
- Must be: fully responsive (mobile/tablet/desktop), fast-loading, SEO-friendly, accessible (WCAG AA — semantic HTML, alt text, keyboard nav, focus states), no console errors, no horizontal scroll, no broken/placeholder-looking images.

## 3. FILE STRUCTURE
```
index.html
style.css
script.js
assets/
  images/          (profile photos, project screenshots — use placeholders where I haven't supplied real ones)
  icons/
  resume/          (resume PDF goes here)
favicon.ico
```
Keep code split across these files (not one giant file), semantic HTML, commented, reusable JS functions, CSS variables for all colors/spacing so I can restyle later.

## 4. VISUAL DIRECTION
Premium dark data/tech-analytics aesthetic — closer to a modern BI product landing page than a "creative portfolio." Reference feel: clean dark hero, generous whitespace, confident typography, one striking hero visual, restrained motion — not a gaming/neon site, not template-generic.

- Deep navy/black background, glassmorphism cards, soft gradients, subtle glow accents
- Accent palette (as CSS variables): cyan/blue + purple accents, green for positive metrics, white/light-gray text
- Subtle background grid + a few floating data particles — restrained, not busy
- Professional sans-serif typography, clear hierarchy, generous spacing
- Data-visualization-inspired UI motifs (mini charts, KPI cards, animated counters) used as design elements throughout, not just in one section

## 5. SIGNATURE VISUAL CONCEPT (use throughout the site)
A recurring "data pipeline" motif: **RAW DATA → PYTHON → SQL → POWER BI → INSIGHTS → DECISIONS**. Use it as the hero's animated centerpiece and echo it in the Workflow section.

## 6. PAGE SECTIONS (in order, sticky nav with smooth scroll)

**Nav:** Home / About / Skills / Workflow / Projects / Dashboards / Certifications / Experience / Resume / Contact. Hamburger on mobile. Nav background changes on scroll.

**Hero**
- H1: "Hi, I'm Sujitha Suresh"
- Subhead: "Data Analyst | SQL | Power BI | Python | Excel"
- Support line: "I transform raw data into meaningful insights, interactive dashboards, and business-ready decisions."
- Animated typing text cycling: Data Analyst / SQL Developer / Power BI Analyst / Python Data Analyst / Business Intelligence Enthusiast / Data Visualization Enthusiast
- CTAs: [View My Projects] [Download Resume]; secondary links: GitHub, LinkedIn, Email
- Floating dashboard card with animated counters (e.g. Total Sales, Total Orders, Avg Sales — use placeholder figures clearly marked as sample data)
- The data-pipeline animation described in section 5
- "Scroll to explore" indicator

**About**
- Entry-level-appropriate copy: hands-on experience with Excel, SQL, Power BI, Python; enjoys cleaning/transforming/analyzing/visualizing data to uncover business insights; focus on turning raw datasets into dashboards and recommendations. Do not overstate seniority.
- Animated profile image area using the portrait photo
- Skill-focus cards: Data Cleaning, Data Analysis, Data Visualization, Business Intelligence, Dashboard Development, SQL Analytics

**Skills** (interactive, animated bars/rings — use honest levels: Advanced / Strong / Intermediate / Working Knowledge, never "Expert")
- Data Analytics: Excel, Advanced Excel, Data Cleaning, Transformation, Validation, Pivot Tables/Charts, Power Query, Data Analysis
- SQL: SELECT, WHERE, GROUP BY, HAVING, JOINs, Subqueries, CTEs, CASE, Window Functions (ROW_NUMBER, RANK, DENSE_RANK), Aggregations, Indexes, Stored Procedures, Triggers, Transactions/ACID, Isolation Levels, Query Optimization, EXPLAIN
- Power BI: Power Query, Data Modeling, DAX, KPI Development, Interactive Dashboards, Slicers, Drill-through, Data Visualization, BI
- Python: Pandas, NumPy, Matplotlib, Seaborn, Data Cleaning, Manipulation, EDA, Visualization
- Tools: MySQL, Excel, Power BI, Git, GitHub, VS Code, Jupyter Notebook

**Analytics Workflow** — animated pipeline, each stage reveals on scroll, tools listed under each stage:
Raw Data (Excel/CSV) → Data Cleaning (Python/Pandas/Power Query) → SQL Analysis → Python Analysis → Power BI → Insights → Business Decisions

**Projects** — premium animated grid; each card shows project name, business problem, tools, key analysis, key insights, preview, GitHub button, live demo button if available. Clicking opens an animated modal with: Overview, Business Problem, Dataset, Tools, Data Cleaning, Analysis, Visualization, Key Insights, Business Recommendations, GitHub link, Live Dashboard link. Use image placeholders (clearly marked, e.g. `YOUR_PROJECT_IMAGE`) where I haven't supplied screenshots — never fabricate a screenshot.

Projects to include:
1. **Retail Sales Analytics** — Python/Pandas/NumPy/Excel/MySQL/Power BI. Pipeline: Excel → Python cleaning → MySQL → SQL analysis → Power BI. KPIs: Total Sales, Avg Sales, Regional Sales, Product Performance, Monthly Trend.
2. **E-Commerce Analytics** — Excel/Python/SQL/Power BI. KPIs: Total Sales, Profit, Orders, Customers, AOV. Analysis: category, top 10 products, country, payment method, order status, monthly trend, product ranking.
3. **Sales Performance Dashboard** — Excel/Power BI/SQL. KPI cards, region/product sales, monthly trend, category analysis, interactive slicers.
4. **Netflix Content Analytics** — Power BI/Excel. Movies vs TV, content by country, release trends, genres, ratings, growth.
5. **Airbnb Analytics** — Excel/Power BI/SQL. Listings, price, availability, neighbourhood, room type, reviews, revenue metrics.
6. **Car Sales Analytics** — Excel/SQL/Power BI. Sales, categories, brands, models, price trends, regional performance.
7. **Customer Churn Analysis** — Python/Pandas/SQL/Power BI. Churn rate, segments, contract type, tenure, revenue patterns, high-risk segments.
8. **Titanic Classification** — Python/Pandas/NumPy/Matplotlib/Seaborn/ML. Present as a secondary ML/analytical project, not a core BI project.

**Power BI Dashboard Gallery** — dedicated section, large hover-animated cards (preview, title, KPIs, tools, View Dashboard, GitHub), lightbox on click.

**SQL Analytics** — interactive animated code snippet cards covering JOIN, GROUP BY, CASE, CTE, window functions (RANK/ROW_NUMBER/DENSE_RANK), subqueries, aggregations, query optimization. Include one real example, e.g.:
```sql
SELECT region, SUM(sales) AS total_sales
FROM sales
GROUP BY region
ORDER BY total_sales DESC;
```
Tagline: "SQL is one of my core analytical skills."

**Python Data Analytics** — animated flow Python → Pandas → NumPy → Cleaning → EDA → Matplotlib → Seaborn → Insights, with snippet examples: `read_csv`, `info()`, `describe()`, `isnull()`, `fillna()`, `groupby()`, `merge()`, `sort_values()`, `value_counts()`.

**Excel Analytics** — animated spreadsheet-style component covering Advanced Excel, Pivot Tables/Charts, Power Query, Data Cleaning, Data Validation, Lookup functions, Conditional Formatting, Dashboard development.

**Certifications & Learning** — cards with certificate name, platform, year, "View Certificate" button (placeholder link if not supplied — never fabricate an ID or URL). Candidates to list (only include ones I confirm): Python Programming, Advanced Google Analytics, Meta Data Analyst Professional Certificate, NPTEL, AWS Academy, Wipro TalentNext, Infosys Springboard, VOIS Python Data Visualization, Power BI/Excel training.

**Experience / Training** — vertical animated timeline; each item: role, organization, duration, skills, what was worked on. Only use info I confirm — do not invent responsibilities.

**How I Approach Data Problems** — 5 steps: Understand the business problem → Collect and inspect data → Clean and transform data → Analyze and visualize → Communicate insights and recommendations. Line: "I focus not only on creating dashboards, but on understanding what the data means for the business."

**Resume CTA** — Heading "Want to know more about my journey?"; buttons "Download Resume" (download attr) and "View Resume" (target="_blank"). Use a config variable: `const resumeURL = "YOUR_RESUME_URL";` — no fake URL.

**Recruiter View toggle** — a button that shows a compact summary card: name, role, core skills, strong areas, project list, and links to resume/LinkedIn/GitHub.

**Contact / "Let's Connect"** — line: "I'm open to Data Analyst opportunities, internships, and projects where I can use data to solve real business problems." Include email, LinkedIn, GitHub, and a contact form UI. No fake backend — either use `mailto:` or clearly note backend integration is required.

**Footer** — name, title, tagline "Turning data into insights.", LinkedIn/GitHub/Email links, © 2026 Sujitha Suresh.

## 7. LINKS
- LinkedIn: https://www.linkedin.com/in/sujitha-suresh
- GitHub: `YOUR_GITHUB_URL` (placeholder — I'll supply)
- Resume: `YOUR_RESUME_URL` (placeholder — I'll supply, place file in `assets/resume/`)

## 8. ANIMATION SPEC
- Load: logo fade-in, nav slide-in, hero text reveal, typing effect, floating dashboard card, number counters, particle drift
- Scroll: section reveals, staggered card entrances, animated skill bars, self-drawing timeline, workflow pipeline connecting
- Hover: cards lift + soft glow, buttons have a subtle magnetic effect, icons micro-animate
- Keep it smooth and tasteful — no animation that hurts load performance or causes layout shift

## 9. SEO / META
- Title: "Sujitha Suresh | Data Analyst Portfolio"
- Meta description: "Data Analyst portfolio of Sujitha Suresh showcasing SQL, Power BI, Excel, Python, data visualization, dashboards and analytics projects."
- Open Graph tags, favicon

## 10. HARD RULES — DO NOT FABRICATE
Never invent: job history, employers, project results/metrics, salary, certificate IDs, GitHub/dashboard URLs, client names, or business outcomes. Anywhere real data isn't supplied, use a clearly labeled placeholder (`YOUR_GITHUB_URL`, `YOUR_RESUME_URL`, `YOUR_PROJECT_IMAGE`) rather than a plausible-looking fake. All personal info/config values should live in one easy-to-edit block at the top of `script.js`.

## 11. DELIVERABLE
Full working site (index.html, style.css, script.js, assets structure) plus:
1. Instructions for adding project screenshots
2. Instructions for adding the resume PDF
3. Instructions for adding certificate links
4. Instructions for deploying to GitHub Pages

Before calling it done, verify: all nav links work, mobile menu works, resume/GitHub/LinkedIn links work, project modals open/close correctly, animations don't jank, layout is responsive at mobile/tablet/desktop widths, no console errors, no horizontal scroll.
