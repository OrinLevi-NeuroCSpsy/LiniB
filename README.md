# אלגברה לינארית — סיכום

סיכום מקיף לקורסים אלגברה לינארית 1ב ו-2ב (למדמ״ח) באוניברסיטת תל אביב.

[![Deploy to GitHub Pages](https://github.com/OrinLevi-NeuroCSpsy/LinearAlgebra/actions/workflows/deploy.yml/badge.svg)](https://github.com/OrinLevi-NeuroCSpsy/LinearAlgebra/actions/workflows/deploy.yml)

**[📖 צפה באתר](https://orinlevi-neurocspsy.github.io/LinearAlgebra/)**

## מבנה הפרויקט

```
lini1B_notes/
├── docs/
│   ├── index.md              # עמוד הבית
│   ├── lini1b/               # לינארית 1ב
│   │   ├── notes/            # סיכומים לפי נושא
│   │   │   ├── linear_systems.md
│   │   │   ├── vector_spaces.md
│   │   │   ├── linear_dependence.md
│   │   │   ├── row_column_spaces.md
│   │   │   ├── linear_transformations.md
│   │   │   ├── similar_matrices.md
│   │   │   ├── determinants.md
│   │   │   └── cramers_rule.md
│   │   └── practice/         # שאלות תרגול
│   ├── lini2b/               # לינארית 2ב
│   │   ├── notes/            # סיכומים לפי נושא
│   │   │   ├── eigenvalues.md
│   │   │   └── inner_product.md
│   │   └── practice/         # שאלות תרגול
│   ├── assets/               # תמונות ו-PDF
│   ├── stylesheets/          # עיצוב
│   └── javascripts/          # MathJax
├── mkdocs.yml                # הגדרות האתר
└── README.md
```

## נושאי הקורסים

### לינארית 1ב

| נושא | תיאור |
|------|--------|
| מערכות משוואות | דירוג, מטריצות אלמנטריות |
| מרחבים וקטוריים | הגדרות, תתי-מרחבים, סכום ישר |
| תלות לינארית | בסיס ומימד |
| מרחבי שורות ועמודות | דרגה, פסילה |
| העתקות לינאריות | גרעין, תמונה, מטריצה מייצגת |
| דטרמיננטות | מינור, מטריצה מצורפת, לפלס |
| כלל קרמר | פתרון מערכות |

### לינארית 2ב

| נושא | תיאור |
|------|--------|
| ערכים עצמיים | לכסון מטריצות |
| מכפלה פנימית | אורתוגונליות, גרם-שמידט |

## תרגול

- שאלות ממבחנים (2021-2025)
- שאלות משיעורי בית
- שאלות מתרגולים
- טריקים וטכניקות

## אתר הסיכום

האתר נבנה עם [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) ומתארח ב-GitHub Pages.

### הרצה מקומית

```bash
pip install mkdocs-material
mkdocs serve
```

האתר יהיה זמין בכתובת `http://localhost:8000`

## מחבר

אורין לוי
