# **Increment & Decrement Operators in JavaScript**  
Increment (`++`) and Decrement (`--`) **values ko barhane ya kam karne ke liye** use hote hain.

| **Operator** | **Name** | **Description** |
|-------------|---------|----------------|
| `++` | Increment | Ek value ko `+1` se barhata hai. |
| `--` | Decrement | Ek value ko `-1` se kam karta hai. |

## **Types of Increment & Decrement**
1. **Post-Increment (`x++`)** → **Pehle value use hoti hai, phir increase hoti hai.**  
2. **Pre-Increment (`++x`)** → **Pehle value increase hoti hai, phir use hoti hai.**  
3. **Post-Decrement (`x--`)** → **Pehle value use hoti hai, phir decrease hoti hai.**  
4. **Pre-Decrement (`--x`)** → **Pehle value decrease hoti hai, phir use hoti hai.**  

---

## **1. Post-Increment (`x++`)**  
**Pehle value print hoti hai, phir `+1` hota hai.**

### **Example: Chai ki Pyali ☕**
Ahmed ne **chai ki 1 pyali pi**, magar counter **baad me update** hoga.

```javascript
let chai = 1;
console.log(chai++);  // Pehle print karega: 1
console.log(chai);    // Ab value badh chuki hai: 2
```

💡 **Output:**  
```
1
2
```

---

## **2. Pre-Increment (`++x`)**  
**Pehle value `+1` hoti hai, phir print hoti hai.**

### **Example: Golgappay Competition 🥤**
Ali ek saath 5 golgappay khata hai, **counter pehle update** hoga.

```javascript
let golgappay = 5;
console.log(++golgappay);  // Pehle badhega, phir print hoga: 6
```

💡 **Output:**  
```
6
```

---

## **3. Post-Decrement (`x--`)**  
**Pehle value print hoti hai, phir `-1` hota hai.**

### **Example: Petrol Tank ⛽**
Car ka **petrol level 10 hai**, lekin ek trip ke baad **baad me kam hoga**.

```javascript
let petrol = 10;
console.log(petrol--);  // Pehle print karega: 10
console.log(petrol);    // Ab value kam ho chuki hai: 9
```

💡 **Output:**  
```
10
9
```

---

## **4. Pre-Decrement (`--x`)**  
**Pehle value `-1` hoti hai, phir print hoti hai.**

### **Example: Ice Cream 🍦**
Bachay ke haath me 3 ice creams hain, **ek girti hai, pehle kam hoga phir dikhayega.**

```javascript
let iceCreams = 3;
console.log(--iceCreams);  // Pehle giregi, phir print hoga: 2
```

💡 **Output:**  
```
2
```

---

## **🎯 Practice Task for You!**
1. Ek variable `mangoes = 7` rakho.
2. Use **post-increment (`x++`)** aur dekho result.
3. Use **pre-decrement (`--x`)** aur dekho result.
4. Batao **post-increment aur pre-increment me kya farq hai?** 😃