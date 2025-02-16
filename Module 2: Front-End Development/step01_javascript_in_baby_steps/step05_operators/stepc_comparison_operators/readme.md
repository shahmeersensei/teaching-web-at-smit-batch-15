# **Comparison Operators in JavaScript**  
Comparison operators **compare two values** and return a **Boolean (true or false)**.

| **Operator** | **Description** | **Example** |
|-------------|----------------|------------|
| `==`  | Equal to (value check only) | `5 == "5"` → `true` |
| `===` | Strict equal (value + type check) | `5 === "5"` → `false` |
| `!=`  | Not equal (value check only) | `5 != 4` → `true` |
| `!==` | Strict not equal (value + type check) | `5 !== "5"` → `true` |
| `>`   | Greater than | `10 > 5` → `true` |
| `<`   | Less than | `3 < 7` → `true` |
| `>=`  | Greater than or equal to | `10 >= 10` → `true` |
| `<=`  | Less than or equal to | `8 <= 9` → `true` |

---

## **1. Equal (`==`) vs. Strict Equal (`===`)**
**Difference:**  
- `==` **checks only value**, type ignore karta hai.  
- `===` **value aur type dono check karta hai**.

### **Example: Bhai Ka Qarz**
```javascript
let bhaiKaQarz = 500;
let dostSeMangayHoyePaisa = "500"; // String format

console.log(bhaiKaQarz == dostSeMangayHoyePaisa);  // true (value same hai)
console.log(bhaiKaQarz === dostSeMangayHoyePaisa); // false (type different hai)
```
💡 **Output:**  
```
true
false
```

---

## **2. Not Equal (`!=`) vs. Strict Not Equal (`!==`)**
**Difference:**  
- `!=` **value check karta hai** (agar value alag ho to `true`).  
- `!==` **value aur type dono check karta hai** (agar koi bhi alag ho to `true`).  

### **Example: Chai Ka Bill**
```javascript
let chaiKaBill = 50;
let dostKiSoch = "50"; // Yeh string hai

console.log(chaiKaBill != dostKiSoch);  // false (value same hai)
console.log(chaiKaBill !== dostKiSoch); // true (type alag hai)
```
💡 **Output:**  
```
false
true
```

---

## **3. Greater Than (`>`) and Less Than (`<`)**
- **`>`**: Koi value doosri se badi hai ya nahi.  
- **`<`**: Koi value doosri se chhoti hai ya nahi.  

### **Example: Aam Ke Rate**
```javascript
let aamKaRate = 150; // per kg price
let merePaasPaisa = 120; 

console.log(merePaasPaisa > aamKaRate); // false (120 bada nahi 150 se)
console.log(merePaasPaisa < aamKaRate); // true (120 chhota hai 150 se)
```
💡 **Output:**  
```
false
true
```

---

## **4. Greater Than or Equal (`>=`) and Less Than or Equal (`<=`)**
- **`>=`**: Koi value **barabar ya badi** ho to `true`.  
- **`<=`**: Koi value **barabar ya chhoti** ho to `true`.  

### **Example: Test Passing Marks**
```javascript
let passingMarks = 40;
let aliKeMarks = 40;

console.log(aliKeMarks >= passingMarks); // true (Ali pass ho gaya)
console.log(aliKeMarks <= passingMarks); // true (Ali ka score equal hai)
```
💡 **Output:**  
```
true
true
```

---

## **💡 Quick Practice Task for You!**
1. Ek variable `mughalBiryaniPrice` (400 rupees) aur `merePaasPaisa` (350 rupees) banao.
2. Check karo **kya paisay biryani se zyada hain? (`>`)**  
3. Check karo **kya paisay biryani ke barabar hain? (`==`)**  
4. Check karo **kya paisay kam hain? (`<`)**  
5. Check karo **kya paisay biryani se kam ya barabar hain? (`<=`)**  

Jaldi likho aur batao **biryani milay gi ya nahi?** 😃