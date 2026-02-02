# דטרמיננטות

## הגדרה

<div class="definition-box" markdown>

**הגדרה רקורסיבית:** הדטרמיננטה של מטריצה \( A \in M_n(F) \) מוגדרת:

**בסיס:** \( n = 1 \): \( \det([a]) = a \)

**צעד:** \( n > 1 \): פיתוח לפי שורה/עמודה:
\[ \det(A) = \sum_{j=1}^{n} (-1)^{i+j} a_{ij} \det(A_{ij}) \]

כאשר \( A_{ij} \) היא המטריצה המתקבלת ממחיקת שורה \( i \) ועמודה \( j \).

</div>

---

## דטרמיננטות של מטריצות קטנות

<div class="formula-box" markdown>

**מטריצה \( 2 \times 2 \):**
\[ \det\begin{pmatrix} a & b \\ c & d \end{pmatrix} = ad - bc \]

</div>

<div class="formula-box" markdown>

**מטריצה \( 3 \times 3 \) (כלל סרוס):**
\[ \det\begin{pmatrix} a & b & c \\ d & e & f \\ g & h & i \end{pmatrix} = aei + bfg + cdh - ceg - bdi - afh \]

</div>

---

## תכונות הדטרמיננטה

<div class="theorem-box" markdown>

**תכונות בסיסיות:**

| תכונה | תוצאה על הדטרמיננטה |
|-------|---------------------|
| החלפת שתי שורות | כפל ב-\( (-1) \) |
| כפל שורה בסקלר \( \alpha \) | כפל ב-\( \alpha \) |
| הוספת כפולה של שורה לאחרת | **לא משתנה** |
| שתי שורות זהות | \( \det = 0 \) |
| שורת אפסים | \( \det = 0 \) |

</div>

---

## משפטים חשובים

<div class="theorem-box" markdown>

**משפט (כפליות):**
\[ \det(AB) = \det(A) \cdot \det(B) \]

</div>

<div class="theorem-box" markdown>

**משפט (שחלוף):**
\[ \det(A^T) = \det(A) \]

</div>

<div class="theorem-box" markdown>

**משפט (הפיכות):**
\[ A \text{ הפיכה} \iff \det(A) \neq 0 \]

ואם \( A \) הפיכה:
\[ \det(A^{-1}) = \frac{1}{\det(A)} \]

</div>

---

## דטרמיננטה של מטריצות מיוחדות

<div class="example-box" markdown>

| סוג מטריצה | דטרמיננטה |
|-----------|-----------|
| מטריצה משולשת | מכפלת האלכסון |
| מטריצה אלכסונית | מכפלת האלכסון |
| מטריצת היחידה | 1 |
| מטריצה סינגולרית | 0 |
| \( \alpha A \) | \( \alpha^n \det(A) \) |

</div>

---

## חישוב הדטרמיננטה

<div class="warning-box" markdown>

**שיטות חישוב:**

1. **פיתוח לפי שורה/עמודה** - בחר שורה/עמודה עם הרבה אפסים
2. **דירוג לצורה משולשת** - זכור לעקוב אחר הסימן
3. **כלל סרוס** - רק למטריצות \( 3 \times 3 \)

</div>

---

## המשוואה האופיינית

<div class="definition-box" markdown>

**הפולינום האופייני:**
\[ p_A(\lambda) = \det(A - \lambda I) \]

זהו פולינום ממעלה \( n \) ב-\( \lambda \).

</div>

<div class="formula-box" markdown>

**משוואת הערכים העצמיים:**
\[ \det(A - \lambda I) = 0 \]

הפתרונות הם הערכים העצמיים של \( A \).

</div>
