### **Conditional Statements in JavaScript**  

Conditional statements ka kaam **decision making** hota hai. Ye **check** karte hain ke koi **condition true hai ya false**, phir uske hisaab se code execute hota hai.  

Samajhne ke liye ek simple **desi example** lete hain:  

## **5️⃣ switch Statement**  
Jab ek **value ko multiple cases** ke saath check karna ho to `switch` use hota hai.

### **Syntax:**
```js
switch (value) {
    case condition1:
        // Ye tab chalega jab condition1 true hogi
        break;
    case condition2:
        // Ye tab chalega jab condition2 true hogi
        break;
    default:
        // Agar koi condition match na kare to ye chalega
}
```

### **Example:**  
_Agar tum Pizza order karo to Pizza milega, Burger order karo to Burger milega, warna Bhooka raho!_  

```js
let order = "Burger";

switch (order) {
    case "Pizza":
        console.log("Pizza aa gaya! 🍕");
        break;
    case "Burger":
        console.log("Burger aa gaya! 🍔");
        break;
    case "Biryani":
        console.log("Biryani aa gayi! 🍛");
        break;
    default:
        console.log("Kuch nahi mila, Bhooka raho! 😭");
}
```

### **Explanation:**  
✅ **order = "Burger"**, to `"Burger aa gaya! 🍔"` print hoga.  
❌ Agar `"Samosa"` hota jo kisi case me nahi hai, to `"Kuch nahi mila, Bhooka raho! 😭"` print hota.

---


## **🎯 Practice Task for You:**
1. Tumhare pass ek variable `marks` hai.  
   - Agar marks **80 ya zyada** hain to print karo `"A Grade"`.  
   - Agar **60 se zyada hain** to print karo `"B Grade"`.  
   - Agar **40 se zyada hain** to print karo `"C Grade"`.  
   - Warna print karo `"Fail"`.  

👉 **Iska JavaScript code likho aur mujhe bhejo!** 🚀