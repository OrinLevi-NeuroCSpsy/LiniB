# כלל קרמר

## המשפט

<div class="theorem-box" markdown>

**כלל קרמר:** תהי \( Ax = b \) מערכת משוואות כאשר \( A \in M_n(F) \) **הפיכה**.

אזי הפתרון היחיד הוא:
\[ x_i = \frac{\det(A_i)}{\det(A)} \]

כאשר \( A_i \) היא המטריצה המתקבלת מ-\( A \) ע"י החלפת העמודה ה-\( i \) בוקטור \( b \).

</div>

---

## דוגמה

<div class="example-box" markdown>

**מערכת 2×2:**

עבור המערכת:
\[ \begin{pmatrix} a & b \\ c & d \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} e \\ f \end{pmatrix} \]

הפתרון:
\[ x = \frac{\det\begin{pmatrix} e & b \\ f & d \end{pmatrix}}{\det(A)} = \frac{ed - bf}{ad - bc} \]

\[ y = \frac{\det\begin{pmatrix} a & e \\ c & f \end{pmatrix}}{\det(A)} = \frac{af - ec}{ad - bc} \]

</div>

---

## דוגמה מספרית

<div class="example-box" markdown>

פתור את המערכת:
\[ \begin{cases} 2x + 3y = 8 \\ x - y = 1 \end{cases} \]

**פתרון:**

\[ A = \begin{pmatrix} 2 & 3 \\ 1 & -1 \end{pmatrix}, \quad b = \begin{pmatrix} 8 \\ 1 \end{pmatrix} \]

\[ \det(A) = 2 \cdot (-1) - 3 \cdot 1 = -5 \]

\[ x = \frac{\det\begin{pmatrix} 8 & 3 \\ 1 & -1 \end{pmatrix}}{-5} = \frac{-8-3}{-5} = \frac{-11}{-5} = \frac{11}{5} \]

\[ y = \frac{\det\begin{pmatrix} 2 & 8 \\ 1 & 1 \end{pmatrix}}{-5} = \frac{2-8}{-5} = \frac{-6}{-5} = \frac{6}{5} \]

</div>

---

## מתי להשתמש בכלל קרמר?

<div class="warning-box" markdown>

**יתרונות:**
- נוסחה סגורה - לא צריך דירוג
- שימושי להוכחות תיאורטיות
- קל למצוא משתנה אחד ספציפי

**חסרונות:**
- דורש חישוב של \( n+1 \) דטרמיננטות
- לא יעיל חישובית עבור מטריצות גדולות
- עובד רק כאשר \( A \) הפיכה (פתרון יחיד)

</div>
