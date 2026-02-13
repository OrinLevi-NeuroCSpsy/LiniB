# מטריצות דומות ושינוי בסיס

## מטריצת מעבר

<div class="definition-box" markdown>

**הגדרה:** יהיו \( B = \{v_1, \ldots, v_n\} \) ו-\( C = \{u_1, \ldots, u_n\} \) שני בסיסים של \( V \).

**מטריצת המעבר** \( P_{C \leftarrow B} \) היא המטריצה שעמודותיה הן וקטורי הקואורדינטות של איברי \( B \) לפי \( C \):
\[ [P_{C \leftarrow B}]_j = [v_j]_C \]

</div>

---

## נוסחת שינוי בסיס

<div class="formula-box" markdown>

**נוסחת שינוי בסיס:**
\[ [v]_C = P_{C \leftarrow B} \cdot [v]_B \]

</div>

---

## תכונות מטריצת מעבר

<div class="theorem-box" markdown>

**משפט:**
1. \( P_{C \leftarrow B} \) הפיכה, ו-\( P_{C \leftarrow B}^{-1} = P_{B \leftarrow C} \)
2. \( P_{D \leftarrow B} = P_{D \leftarrow C} \cdot P_{C \leftarrow B} \)

</div>

---

## מטריצות דומות

<div class="definition-box" markdown>

**הגדרה:** שתי מטריצות \( A, B \in M_n(F) \) נקראות **דומות** אם קיימת מטריצה הפיכה \( P \) כך ש:
\[ B = P^{-1}AP \]

</div>

---

## שימור תחת דמיון

<div class="theorem-box" markdown>

**משפט:** אם \( A \) ו-\( B \) דומות, אז:

1. \( \det(A) = \det(B) \)
2. \( \text{tr}(A) = \text{tr}(B) \)
3. \( \text{rank}(A) = \text{rank}(B) \)
4. להן אותו פולינום אופייני
5. להן אותם ערכים עצמיים

</div>

---

## קשר בין מטריצות מייצגות

<div class="formula-box" markdown>

**משפט:** אם \( T: V \to V \) ו-\( B, C \) בסיסים של \( V \), אז:
\[ [T]_C = P_{C \leftarrow B}^{-1} \cdot [T]_B \cdot P_{C \leftarrow B} \]

**מסקנה:** מטריצות מייצגות של אותה העתקה הן דומות!

</div>
