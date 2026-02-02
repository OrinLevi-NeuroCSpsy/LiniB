# העתקות לינאריות

## הגדרה

<div class="definition-box" markdown>

**הגדרה:** יהיו \( V, W \) מרחבים וקטוריים מעל אותו שדה \( F \).

פונקציה \( T: V \to W \) היא **העתקה לינארית** אם לכל \( u, v \in V \) ולכל \( \alpha \in F \):

1. **אדיטיביות:** \( T(u + v) = T(u) + T(v) \)
2. **הומוגניות:** \( T(\alpha v) = \alpha T(v) \)

</div>

<div class="formula-box" markdown>

**שקילות:** \( T \) לינארית אם"ם לכל \( u, v \in V \) ולכל \( \alpha, \beta \in F \):
\[ T(\alpha u + \beta v) = \alpha T(u) + \beta T(v) \]

</div>

---

## תכונות בסיסיות

<div class="theorem-box" markdown>

**משפט:** אם \( T: V \to W \) העתקה לינארית, אז:

1. \( T(0_V) = 0_W \)
2. \( T(-v) = -T(v) \)
3. \( T(\alpha_1 v_1 + \cdots + \alpha_n v_n) = \alpha_1 T(v_1) + \cdots + \alpha_n T(v_n) \)

</div>

---

## גרעין ותמונה

<div class="definition-box" markdown>

**גרעין (Kernel):**
\[ \ker(T) = \{ v \in V : T(v) = 0 \} \]

**תמונה (Image):**
\[ \text{Im}(T) = \{ T(v) : v \in V \} = \{ w \in W : \exists v \in V, T(v) = w \} \]

</div>

<div class="theorem-box" markdown>

**משפט:**
- \( \ker(T) \) הוא תת-מרחב של \( V \)
- \( \text{Im}(T) \) הוא תת-מרחב של \( W \)

</div>

---

## משפט המימדים

<div class="formula-box" markdown>

**משפט המימדים (Rank-Nullity):**
\[ \dim(V) = \dim(\ker(T)) + \dim(\text{Im}(T)) \]

או בסימון אחר:
\[ \dim(V) = \text{nullity}(T) + \text{rank}(T) \]

</div>

---

## חד-חד-ערכיות ועל

<div class="theorem-box" markdown>

**משפט:** יהי \( T: V \to W \) העתקה לינארית.

| תכונה | תנאי שקול |
|-------|-----------|
| \( T \) חח"ע | \( \ker(T) = \{0\} \) |
| \( T \) על | \( \text{Im}(T) = W \) |
| \( T \) הפיכה | \( T \) חח"ע ועל |

</div>

<div class="theorem-box" markdown>

**משפט:** אם \( \dim(V) = \dim(W) = n \), אז שקול:
- \( T \) חח"ע
- \( T \) על
- \( T \) הפיכה

</div>

---

## מטריצה מייצגת

<div class="definition-box" markdown>

**הגדרה:** יהי \( T: V \to W \) העתקה לינארית, \( B = \{v_1, \ldots, v_n\} \) בסיס של \( V \), ו-\( C = \{w_1, \ldots, w_m\} \) בסיס של \( W \).

**המטריצה המייצגת** \( [T]_B^C \) מוגדרת כך: העמודה ה-\( j \) היא וקטור הקואורדינטות של \( T(v_j) \) לפי הבסיס \( C \).

</div>

<div class="formula-box" markdown>

**נוסחת הקשר:**
\[ [T(v)]_C = [T]_B^C \cdot [v]_B \]

</div>

---

## הרכבת העתקות

<div class="theorem-box" markdown>

**משפט:** אם \( T: V \to W \) ו-\( S: W \to U \) העתקות לינאריות, אז \( S \circ T: V \to U \) גם העתקה לינארית, ומתקיים:
\[ [S \circ T]_B^D = [S]_C^D \cdot [T]_B^C \]

</div>
