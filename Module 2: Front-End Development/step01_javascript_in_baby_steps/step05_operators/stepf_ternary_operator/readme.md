# **Ternary Operator (`? :`) in JavaScript**  
Ternary operator **ek short-hand if-else statement** hai jo **ek hi line me condition check** karne ke liye use hota hai.  

### **Syntax:**
```javascript
condition ? expression_if_true : expression_if_false;
```
Agar **condition true** ho to **first value return** hogi, warna **second value return** hogi.

---

## **🎯 Real-Life Example: Chai vs Coffee ☕**
Agar **chai garam hai** to **"Mazaydar Chai!"** warna **"Chai thandi hai! ☹️"**.

```javascript
let chaiGaram = true;
let message = chaiGaram ? "Mazaydar Chai! 😍" : "Chai thandi hai! ☹️";
console.log(message);
```

💡 **Output (Agar chai garam hai)**  
```
Mazaydar Chai! 😍
```
💡 **Output (Agar chai thandi hoti)**  
```
Chai thandi hai! ☹️
```

---

## **🛒 Example: Shopping Discount 🛍️**
Agar **500 rupay se zyada ka shopping** ki to **discount milega**, warna **nahi milega**.

```javascript
let totalBill = 600;
let discount = totalBill > 500 ? "Aapko discount mila! 🎉" : "Koi discount nahi! 😢";
console.log(discount);
```

💡 **Output (Agar 600 ka bill hai)**  
```
Aapko discount mila! 🎉
```
💡 **Output (Agar 400 ka bill hota)**  
```
Koi discount nahi! 😢
```

---

## **🕺 Example: Dance Party Age Check 🎶**
Agar **18 ya us se zyada age hai** to **party join kar sakte ho**, warna **entry nahi milegi**.

```javascript
let age = 17;
let entry = age >= 18 ? "Welcome to the party! 🎉" : "Sorry, underage ho! 😢";
console.log(entry);
```

💡 **Output (Agar 17 saal ka banda hai)**  
```
Sorry, underage ho! 😢
```

---

## **⏳ Nested Ternary Operator 🏆**
Agar **60 ya us se upar marks** hain to **"Pass"**, agar **40-59 ke darmiyan hain** to **"Average"**, warna **"Fail"**.

```javascript
let marks = 50;
let result = marks >= 60 ? "Pass 🏆" : marks >= 40 ? "Average 🤔" : "Fail ❌";
console.log(result);
```

💡 **Output (Agar marks 50 hain)**  
```
Average 🤔
```

---

## **🎯 Practice Task for You!**
1. Ek variable `temperature = 35` rakho.  
2. Check karo **agar 30 se zyada hai** to `"Bahut garmi hai! 🔥"` warna `"Mausam normal hai. 😊"`  
3. Ek variable `wallet = 100` rakho. Check karo **agar 150 rupay se kam hai** to `"Pizza nahi khareed sakte! 😢"` warna `"Pizza khareed lo! 🍕"`  

🔥 **Apna code likho aur check karo!** 😃