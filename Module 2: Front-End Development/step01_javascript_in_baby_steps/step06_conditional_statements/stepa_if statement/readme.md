### **Conditional Statements in JavaScript**  

Conditional statements ka kaam **decision making** hota hai. Ye **check** karte hain ke koi **condition true hai ya false**, phir uske hisaab se code execute hota hai.  

Samajhne ke liye ek simple **desi example** lete hain:  

📌 **Example:**  
_Agar tumhare pass **500 rupay** hain, to tum **Biryani** kha sakte ho. Warna **Chai Paratha** pe guzara karna parega!_ ☕🍛  

---

## **1️⃣ if Statement**  
Agar **condition true** hai to andar wala code chalega, warna **skip** ho jayega.

### **Syntax:**
```js
if (condition) {
    // Yeh block tabhi chalega jab condition true hogi
}
```

### **Example:**  
_Agar dukan ka darwaza khula hai, to andar chalay jao!_  

```js
let darwazaKhulaHai = true;

if (darwazaKhulaHai) {
    console.log("Andar chalay jao! 🏠");
}
```

### **Explanation:**  
✅ **darwazaKhulaHai = true**, is liye andar jane ka message print hoga.  
❌ Agar `darwazaKhulaHai = false;` hota to kuch bhi print nahi hota.

---


## **📌 Summary:**
| Statement | Usage | Example |
|-----------|--------|---------|
| **if** | Jab ek simple condition ho | _Agar bijli hai to fan chalu hai_ |
| **if-else** | Jab ek condition fail ho to doosra kaam ho | _Agar paisay hain to chai pee lo, warna paani piyo_ |
| **if-else if-else** | Jab multiple conditions ho | _500 rupay = Biryani, 200 rupay = Chai, 0 = Paani_ |
| **Nested if-else** | Jab ek condition ke andar doosri check karni ho | _Agar pass ho aur fees bhi ho to admission milega_ |
| **switch** | Jab ek value ko multiple cases ke saath check karna ho | _Pizza/Burger/Biryani ka order_ |

---

## **🎯 Practice Task for You:**
1. Tumhare pass ek variable `marks` hai.  
   - Agar marks **80 ya zyada** hain to print karo `"A Grade"`.  
   - Agar **60 se zyada hain** to print karo `"B Grade"`.  
   - Agar **40 se zyada hain** to print karo `"C Grade"`.  
   - Warna print karo `"Fail"`.  

👉 **Iska JavaScript code likho aur mujhe bhejo!** 🚀