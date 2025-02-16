### **Conditional Statements in JavaScript**  

Conditional statements ka kaam **decision making** hota hai. Ye **check** karte hain ke koi **condition true hai ya false**, phir uske hisaab se code execute hota hai.  

Samajhne ke liye ek simple **desi example** lete hain:  


## **3️⃣ if-else if-else Statement**  
Agar ek se zyada **conditions** check karni ho to `else if` use hota hai.

### **Syntax:**
```js
if (condition1) {
    // Ye tab chalega jab condition1 true hogi
} else if (condition2) {
    // Ye tab chalega jab condition2 true hogi
} else {
    // Agar koi condition true na ho to ye chalega
}
```

### **Example:**  
_Agar **500 rupay hain** to **Biryani** kha lo. Agar **200 rupay hain** to **Chai Paratha** khao. Agar **kuch nahi** to **paani pe ke so jao!**_  

```js
let paisay = 100;

if (paisay >= 500) {
    console.log("Biryani kha lo! 🍛");
} else if (paisay >= 200) {
    console.log("Chai aur Paratha kha lo! ☕🍞");
} else {
    console.log("Paani pe ke so jao! 😴");
}
```

### **Explanation:**  
✅ Agar **paisay = 500** hote to `"Biryani kha lo! 🍛"` print hota.  
✅ Agar **paisay = 200** hote to `"Chai aur Paratha kha lo! ☕🍞"` print hota.  
❌ **100** hai, jo kisi condition ko match nahi karta, is liye **paani pe ke so jao** print hoga.

---


## **🎯 Practice Task for You:**
1. Tumhare pass ek variable `marks` hai.  
   - Agar marks **80 ya zyada** hain to print karo `"A Grade"`.  
   - Agar **60 se zyada hain** to print karo `"B Grade"`.  
   - Agar **40 se zyada hain** to print karo `"C Grade"`.  
   - Warna print karo `"Fail"`.  

👉 **Iska JavaScript code likho aur mujhe bhejo!** 🚀