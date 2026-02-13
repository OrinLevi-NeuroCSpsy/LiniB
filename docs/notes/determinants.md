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

\( A \) הפיכה \( \iff \det(A) \neq 0 \)

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

---

## מינור וקופקטור

<div class="definition-box" markdown>

**מינור \( M_{ij} \):** הדטרמיננטה של המטריצה המתקבלת ממחיקת שורה \( i \) ועמודה \( j \) מ-\( A \).

**קופקטור (משלים אלגברי) \( C_{ij} \):**
\[ C_{ij} = (-1)^{i+j} M_{ij} \]

</div>

<div class="warning-box" markdown>

**שימו לב לסימן!**

\[
\begin{pmatrix} + & - & + & \cdots \\ - & + & - & \cdots \\ + & - & + & \cdots \\ \vdots & \vdots & \vdots & \ddots \end{pmatrix}
\]

הסימן נקבע לפי \( (-1)^{i+j} \).

</div>

---

## פיתוח לפלס (Laplace Expansion)

<div class="theorem-box" markdown>

**פיתוח לפי שורה \( i \):**
\[ \det(A) = \sum_{j=1}^{n} a_{ij} C_{ij} = \sum_{j=1}^{n} (-1)^{i+j} a_{ij} M_{ij} \]

**פיתוח לפי עמודה \( j \):**
\[ \det(A) = \sum_{i=1}^{n} a_{ij} C_{ij} = \sum_{i=1}^{n} (-1)^{i+j} a_{ij} M_{ij} \]

</div>

<div class="example-box" markdown>

**טיפ:** תמיד פתחו לפי השורה/עמודה עם הכי הרבה אפסים - זה מקטין את כמות החישובים!

</div>

---

## המטריצה המצורפת (Adjugate Matrix)

<div class="definition-box" markdown>

**מטריצה מצורפת \( \text{adj}(A) \):**

המטריצה שאיבריה הם הקופקטורים, **עם שחלוף**:
\[ (\text{adj}(A))_{ij} = C_{ji} \]

**שימו לב:** האינדקסים מתחלפים!

</div>

<div class="theorem-box" markdown>

**זהות חשובה:**
\[ A \cdot \text{adj}(A) = \text{adj}(A) \cdot A = \det(A) \cdot I \]

**מסקנה - נוסחה להופכי:**
\[ A^{-1} = \frac{1}{\det(A)} \cdot \text{adj}(A) \]

</div>

<div class="example-box" markdown>

**למטריצה \( 2 \times 2 \):**
\[ A = \begin{pmatrix} a & b \\ c & d \end{pmatrix} \implies \text{adj}(A) = \begin{pmatrix} d & -b \\ -c & a \end{pmatrix} \]

ולכן:
\[ A^{-1} = \frac{1}{ad-bc} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix} \]

</div>

---

## מטריצת בלוקים

<div class="theorem-box" markdown>

**דטרמיננטה של מטריצת בלוקים משולשת:**

\[ \det\begin{pmatrix} B & C \\ 0 & D \end{pmatrix} = \det(B) \cdot \det(D) \]

\[ \det\begin{pmatrix} B & 0 \\ C & D \end{pmatrix} = \det(B) \cdot \det(D) \]

</div>

<div class="warning-box" markdown>

**זהירות:** זה עובד רק כשיש בלוק אפסים! אם שני הבלוקים "מלאים", אי אפשר להפריד את הדטרמיננטה.

</div>

---

## השפעת פעולות שורה על הדטרמיננטה

<div class="theorem-box" markdown>

| פעולה | השפעה על \( \det \) |
|-------|---------------------|
| \( R_i \leftrightarrow R_j \) (החלפת שורות) | כפל ב-\( (-1) \) |
| \( R_i \to \alpha R_i \) (כפל שורה בסקלר) | כפל ב-\( \alpha \) |
| \( R_i \to R_i + \alpha R_j \) (הוספת כפולה) | **ללא שינוי** |

**אותו דבר עבור פעולות עמודה!**

</div>

<div class="theorem-box" markdown>

**אדישות לשחלוף:**
\[ \det(A^T) = \det(A) \]

לכן כל תכונה שנכונה לשורות, נכונה גם לעמודות.
