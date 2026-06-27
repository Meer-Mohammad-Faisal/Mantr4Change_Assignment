# PBL Program Intelligence & Grant Reporting Assistant

A data-driven dashboard for monitoring Project-Based Learning (PBL) implementation across schools. The application helps program managers review monthly performance, generate grant reports, identify risk areas, and recommend actions based on program data.

---

## Features

- 📊 Program Review Dashboard
- 📈 Monthly Review Summary
- 📄 Grant Reporting Assistant
- ✅ Recommended Actions
- 🎯 KPI Cards
- 📉 Attendance & Participation Analysis
- 📍 District & Block Filtering
- ⚠️ Risk Classification
- 📂 CSV → JSON Data Conversion Script
- 📱 Responsive UI
- 🌙 Light/Dark Theme Support

---

## Tech Stack

### Frontend

- React 19
- TypeScript
- Vite
- TanStack Router
- TanStack Query
- Tailwind CSS v4
- shadcn/ui
- Lucide React

### Backend

- TanStack Start
- Nitro Server

### Utilities

- React Hook Form
- Zod
- Sonner
- clsx
- tailwind-merge

---

## Project Structure

```
Assignment-Ace/
│
├── public/
│   └── data/
│       ├── schools.json
│       ├── grant_finance.json
│       ├── grant_performance.json
│       └── evidence.json
│
├── scripts/
│   └── convert_csv_to_json.py
│
├── src/
│   ├── components/
│   │   ├── AppShell.tsx
│   │   ├── FilterBar.tsx
│   │   ├── KpiCard.tsx
│   │   ├── RiskBadge.tsx
│   │   └── ui/
│   │
│   ├── hooks/
│   │   └── use-mobile.tsx
│   │
│   ├── lib/
│   │   ├── data.ts
│   │   ├── filters.tsx
│   │   ├── narrative.ts
│   │   ├── utils.ts
│   │   ├── error-page.ts
│   │   ├── error-capture.ts
│   │   └── lovable-error-reporting.ts
│   │
│   ├── routes/
│   │   ├── __root.tsx
│   │   ├── index.tsx
│   │   ├── summary.tsx
│   │   ├── grants.tsx
│   │   └── actions.tsx
│   │
│   ├── router.tsx
│   ├── routeTree.gen.ts
│   ├── server.ts
│   ├── start.ts
│   └── styles.css
│
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

---

## Installation

Clone the repository

```bash
git clone <repository-url>
```

Install dependencies

```bash
npm install
```

or

```bash
bun install
```

---

## Development

```bash
npm run dev
```

or

```bash
bun run dev
```

---

## Production Build

```bash
npm run build
```

Preview production build

```bash
npm run preview
```

---

## Data Source

The application reads data from

```
public/data/
```

including

- schools.json
- grant_finance.json
- grant_performance.json
- evidence.json

These files are generated using

```
scripts/convert_csv_to_json.py
```

---

## Dashboard Modules

### Program Review

Displays

- Overall Program Score
- KPIs
- Attendance
- Participation
- Risk Status
- District Performance

---

### Monthly Review Summary

Automatically generates

- Key Achievements
- Risks
- Priorities
- Discussion Points

---

### Grant Reporting

Creates narrative reports suitable for donor reporting using available program metrics.

---

### Recommended Actions

Suggests

- Mentor Visits
- Evidence Submission Follow-ups
- Attendance Improvements
- District Priorities

---

## Risk Categories

| Score | Status |
|--------|--------|
| ≥ 75% | On Track |
| ≥ 60% | Behind |
| ≥ 35% | At Risk |
| < 35% | Critical |

---

## Main Libraries

- TanStack Router
- TanStack Query
- TailwindCSS
- shadcn/ui
- React Hook Form
- Zod
- Sonner
- Lucide Icons

---

## Notes

This project was developed as a dashboard for analyzing Project-Based Learning (PBL) implementation using normalized JSON datasets generated from CSV files.

The dashboard provides an overview of participation, attendance, evidence submission, district-wise performance, grant reporting, and actionable recommendations for program managers.

---

## License

This project is intended for educational and assessment purposes.
