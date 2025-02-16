# **`typeof` Operator in JavaScript**  
`typeof` ek **built-in operator** hai jo kisi bhi **variable ya value ka data type return** karta hai. Yeh **debugging** aur **data validation** ke liye kaafi useful hota hai.  

---

## **📌 Syntax:**  
```javascript
typeof variable_or_value;
```

---

## **🎯 Real-Life Example: Aadhaar Card Check**  
Jaise aadmi ka **Naam (String), Umar (Number), Passport Hai Ya Nahi (Boolean)** hota hai, waise hi **JavaScript me har value ka type hota hai**.

```javascript
let name = "Haris";
let age = 25;
let hasPassport = true;

console.log(typeof name);       // "string"
console.log(typeof age);        // "number"
console.log(typeof hasPassport);// "boolean"
```

💡 **Output:**  
```
string
number
boolean
```

---

## **🔢 `typeof` Different Data Types Ko Check Karta Hai**  
JavaScript me different **data types** hain, aur `typeof` unko identify karne me help karta hai.

| **Value**           | **typeof Output** |
|---------------------|----------------|
| `"Hello"`          | `"string"`     |
| `100`              | `"number"`     |
| `true / false`     | `"boolean"`    |
| `{}` (object)      | `"object"`     |
| `null`             | `"object"` (bug in JS 😅) |
| `undefined`        | `"undefined"`  |
| `function() {}`    | `"function"`   |

---

## **🍕 Example: Pizza Order System 🛒**  
Maan lo ek **pizza order system** hai, jisme **user ka name (string), order ka price (number), aur delivery confirm hai ya nahi (boolean)** check karna hai.

```javascript
let customerName = "Ali Khan";
let orderPrice = 1200;
let isDelivered = false;

console.log(typeof customerName); // "string"
console.log(typeof orderPrice);   // "number"
console.log(typeof isDelivered);  // "boolean"
```

💡 **Output:**  
```
string
number
boolean
```

---

## **🚀 Example: Null & Undefined**  
`null` aur `undefined` dono alag-alag hote hain, aur `typeof` se ye clear hota hai.

```javascript
let x = null;
let y;

console.log(typeof x); // "object" (JavaScript ka ek bug!)
console.log(typeof y); // "undefined"
```

💡 **Output:**  
```
object
undefined
```

💡 **Note:** `"object"` ek **JavaScript ka old bug hai** jo ab bhi exist karta hai.

---

## **🛠️ Example: Function and Object Check**  
Agar **function ya object hai** to `typeof` use kar ke check kar sakte hain.

```javascript
let person = { name: "Haris", age: 28 };
let greet = function () {
  return "Hello World!";
};

console.log(typeof person); // "object"
console.log(typeof greet);  // "function"
```

💡 **Output:**  
```
object
function
```

---

## **🎯 Practice Tasks for You!**
1. Ek **variable `price = "500"` rakho** aur `typeof` se check karo kya type hai.  
2. Ek **function create karo** aur uska `typeof` print karo.  
3. **Ek empty array (`[]`) ka `typeof` check karo** aur dekho JavaScript kya return karti hai.  
4. **Agar `typeof variable === "number"` ho** to `"Yeh ek number hai"` print karo, warna `"Yeh koi number nahi hai"` print karo.  

🔥 **Try karo aur practice improve karo!** 😃