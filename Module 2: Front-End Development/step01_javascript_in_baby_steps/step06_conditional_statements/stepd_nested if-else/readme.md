### **Conditional Statements in JavaScript**  

Conditional statements ka kaam **decision making** hota hai. Ye **check** karte hain ke koi **condition true hai ya false**, phir uske hisaab se code execute hota hai.  

Samajhne ke liye ek simple **desi example** lete hain:  

## **4️⃣ Nested if-else (if ke andar if)**  
Agar ek **if ke andar doosri condition** check karni ho to **nested if-else** use hota hai.

### **Syntax:**
```js
if (condition1) {
    if (condition2) {
        // Ye tab chalega jab dono conditions true hongi
    } else {
        // Jab sirf pehli condition true ho
    }
} else {
    // Jab pehli condition bhi false ho
}
```

### **Example:**  
_Agar tum **10th class pass** ho aur **admission fees** bhi hai to tum admission le sakte ho._  

```js
let passKiya = true;
let feesHai = false;

if (passKiya) {
    if (feesHai) {
        console.log("Admission ho gaya! 🎓");
    } else {
        console.log("Pehle fees jama karao! 💰");
    }
} else {
    console.log("Pehle 10th pass karo! 📚");
}
```

### **Explanation:**  
✅ Agar **passKiya = true** aur **feesHai = true** hota to `"Admission ho gaya!"` print hota.  
✅ Agar **feesHai = false** hota to `"Pehle fees jama karao!"` print hoga.  
❌ Agar **passKiya = false** hota to `"Pehle 10th pass karo!"` print hota.

---

## **🎯 Practice Task for You:**
1. Tumhare pass ek variable `marks` hai.  
   - Agar marks **80 ya zyada** hain to print karo `"A Grade"`.  
   - Agar **60 se zyada hain** to print karo `"B Grade"`.  
   - Agar **40 se zyada hain** to print karo `"C Grade"`.  
   - Warna print karo `"Fail"`.  

👉 **Iska JavaScript code likho aur mujhe bhejo!** 🚀