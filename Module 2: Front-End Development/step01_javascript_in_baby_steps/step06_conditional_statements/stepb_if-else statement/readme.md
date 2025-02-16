### **Conditional Statements in JavaScript**  

Conditional statements ka kaam **decision making** hota hai. Ye **check** karte hain ke koi **condition true hai ya false**, phir uske hisaab se code execute hota hai.  

Samajhne ke liye ek simple **desi example** lete hain:  

## **2️⃣ if-else Statement**  
Agar **condition true hai to ek kaam hoga**, agar false hai to **doosra kaam hoga**.

### **Syntax:**
```js
if (condition) {
    // Ye tab chalega jab condition true hogi
} else {
    // Ye tab chalega jab condition false hogi
}
```

### **Example:**  
_Agar bijli hai, fan chalay ga. Warna garmi me paseena aaye ga!_ 😓

```js
let bijliHai = false;

if (bijliHai) {
    console.log("Fan chalu hai! 🌬️");
} else {
    console.log("Bijli nahi hai, garmi bardasht karo! 😓");
}
```

### **Explanation:**  
✅ Agar **bijliHai = true** hoti to `"Fan chalu hai! 🌬️"` print hota.  
❌ Yahan **false** hai, is liye `"Bijli nahi hai, garmi bardasht karo! 😓"` print hoga.

---

## **🎯 Practice Task for You:**
1. Tumhare pass ek variable `marks` hai.  
   - Agar marks **80 ya zyada** hain to print karo `"A Grade"`.  
   - Agar **60 se zyada hain** to print karo `"B Grade"`.  
   - Agar **40 se zyada hain** to print karo `"C Grade"`.  
   - Warna print karo `"Fail"`.  

👉 **Iska JavaScript code likho aur mujhe bhejo!** 🚀