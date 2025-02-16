# **📌 Variables, Naming Rules & Scoping in JavaScript**  
Aaj hum **variables ke naming rules aur scoping** ka concept **desi examples** ke saath seekhenge. 🚀  

---

## **🟢 Variable Naming Rules (Naam Rakhnay Ke Qanoon)**
Jab bhi variable ka naam rakho, **yahi chaar qanoon yaad rakhna:**  

1️⃣ **Sirf alphabets, numbers, `_` (underscore) aur `$` (dollar sign) use kar sakte hain.**  
2️⃣ **Naam kabhi bhi number se start nahi hona chahiye.**  
3️⃣ **Spaces allowed nahi hain.**  
4️⃣ **JavaScript ke reserved keywords use nahi kar sakte (e.g., `let`, `var`, `if`).**  

### **🎯 Example: Galat vs Sahi Naming**
```javascript
// ❌ Galat (Wrong)
let 2cars = "Toyota";  // ❌ Number se start nahi ho sakta
let my car = "Civic";   // ❌ Spaces allowed nahi
let let = "something";  // ❌ Reserved word use nahi kar sakte

// ✅ Sahi (Correct)
let myCar = "Civic";   
let _price = 50000;     
let $discount = 10;      
```

---

## **🟢 Scoping (Variable Kahan Tak Kaam Karega?)**  
Scoping ka matlab hai **variable kis area mein accessible hai**.  

### **🔹 1. Global Scope (Poore Program Mein Available)**
Agar hum **`var` ya `let`** se variable **function ke bahar** declare karein, toh wo **poore program mein accessible hota hai**.

**💡 Example:**  
```javascript
let harisKaWallet = 50; // Global Variable

function checkMoney() {
    console.log("Haris ke wallet mein: " + harisKaWallet + " rupees"); 
}

checkMoney();  
console.log("Bahar bhi use kar sakte hain: " + harisKaWallet);  
```
📢 **Output:**  
```
Haris ke wallet mein: 50 rupees  
Bahar bhi use kar sakte hain: 50 rupees
```

✅ **Poore program mein accessible hai!**  

---

### **🔹 2. Function Scope (Sirf Function Ke Andar Kaam Karega)**
Agar hum **function ke andar `var` se variable declare karein**, toh wo sirf **usi function mein accessible hota hai**.

**💡 Example:**  
```javascript
function chaiBanana() {
    var sugar = 2;  // Function Scope
    console.log("Chai mein " + sugar + " chamach cheeni hai");
}

chaiBanana(); 
console.log(sugar); // ❌ Error! Ye function ke bahar access nahi ho sakta
```
📢 **Output:**  
```
Chai mein 2 chamach cheeni hai  
ReferenceError: sugar is not defined
```

❌ **Bahar access nahi ho sakta kyunki `sugar` function ke andar hi defined hai.**  

---

### **🔹 3. Block Scope (`let` & `const` Wale)**
Agar hum **`let` ya `const`** use karein kisi `{}` block ke andar, toh wo sirf **usi block ke andar kaam karega**.

**💡 Example: Chotu Ki Ice Cream 🍦**  
```javascript
if (true) {
    let chotuKiIceCream = "Vanilla";
    console.log("Chotu ki ice cream: " + chotuKiIceCream);
}

console.log(chotuKiIceCream); // ❌ Error! Bahar access nahi kar sakte
```
📢 **Output:**  
```
Chotu ki ice cream: Vanilla  
ReferenceError: chotuKiIceCream is not defined
```

🔹 **`let` aur `const` block scope mein rehte hain.**  
🔹 **Sirf `{}` ke andar accessible hote hain.**  

---

### **🔹 4. Lexical Scope (Nested Function Scope)**
Agar ek function doosre function ke andar ho, toh **andar wala function bahar wale function ke variables use kar sakta hai**.

**💡 Example: Abbu Ki Salary 💸**
```javascript
function abbuKiSalary() {
    let salary = 50000; // Parent Scope
    
    function betaKaPocketMoney() {
        let pocketMoney = 500; // Child Scope
        console.log("Beta ka pocket money: " + pocketMoney);
        console.log("Abbu ki salary: " + salary); // Beta Abbu ki salary dekh sakta hai
    }

    betaKaPocketMoney();
    console.log("Abbu beta ka pocket money nahi dekh sakte: " + pocketMoney); // ❌ Error!
}

abbuKiSalary();
```
📢 **Output:**  
```
Beta ka pocket money: 500  
Abbu ki salary: 50000  
ReferenceError: pocketMoney is not defined
```
✅ **Child function Parent function ke variables ko use kar sakta hai!**  
❌ **Parent function Child function ke variables ko use nahi kar sakta.**  

---

## **📌 Quick Recap**
| Scope Type        | Accessible Kahan?                         | Example |
|------------------|---------------------------------|---------|
| **Global Scope**  | Poore program mein accessible  | `let name = "Ali";` |
| **Function Scope** | Sirf function ke andar        | `var sugar = 2;` |
| **Block Scope**   | Sirf `{}` block ke andar       | `let chai = "Karak";` |
| **Lexical Scope** | Child function Parent ke variables use kar sakta hai | Nested functions |

---

## **🎯 Practice Challenge**
Aap ek function likhiye **`mobileRecharge()`** jo ek **global variable `balance`** ko check kare.  
- Agar balance **500 rupay se kam ho**, toh **"Recharge karna padega!"** print kare.  
- Warna **"Balance sahi hai!"** print kare.  

Aapka answer kuch is tarah hona chahiye:  

```javascript
let balance = 300;  // Global variable

function mobileRecharge() {
    if (balance < 500) {
        console.log("Recharge karna padega!");
    } else {
        console.log("Balance sahi hai!");
    }
}

mobileRecharge();
```

📢 **Output:**  
```
Recharge karna padega!
```

---

### **🔥 Aapka Agla Step**
Agar aapko **variables aur scoping** ka concept samajh aa gaya hai, toh **practice karke batayein!**  
👀 **Koi aur desi example chahiye? Batao!** 🚀

### **🔥 Practice Time – Desi Examples ke Saath 🚀**  
Aap neeche diye gaye **practice challenges** solve karein. Har ek example **desi life se related hai**, jo aapko **variables aur scoping** ka concept samajhne mein madad dega.  

---

## **📌 Challenge 1: Ammi ka Shopping Budget 🛍️**
👩‍👦 **Scenario:** Ammi ne **shopping ke liye 1000 rupay diye hain**, lekin **aap har shopping item ke baad balance check karna chahte hain.**  

📢 **Task:** Ek function likhiye **`shopping()`** jo ek item ki price subtract kare aur updated balance show kare.  

🔹 **Rules:**  
- **Global variable** `budget = 1000` rakhein.  
- Function `shopping(price)` ko **item ki price deni hai**, jo **budget se minus ho jayegi.**  
- Har shopping ke baad **"Bachay huay paisay:"** print kare.  

📌 **Hint:** `budget = budget - price;`

### **✅ Example Output:**
```javascript
let budget = 1000; // Global variable

function shopping(price) {
    budget = budget - price; // Shopping karne ke baad balance update
    console.log("Bachay huay paisay: " + budget);
}

shopping(200);  // Pehli shopping
shopping(300);  // Dusri shopping
shopping(150);  // Teesri shopping
```
📢 **Output:**  
```
Bachay huay paisay: 800
Bachay huay paisay: 500
Bachay huay paisay: 350
```
💡 **Samajh Aaya?** Aap ke budget mein se har baar paisay minus ho rahe hain!

---

## **📌 Challenge 2: Chai Ka Masla ☕**
👦 **Scenario:** Ali apne dosto ko **chai pilana chahta hai**, lekin chai ka **saman check karna zaroori hai!**  
Agar **doodh aur chai patti available hai**, tabhi **"Chai tayar ho gayi!"** print hoga. Warna **"Saman kam hai, chai nahi ban sakti!"**  

📢 **Task:**  
- Do **block-scoped variables** (`let` use karna hai).  
- Ek function **`makeChai()`** likhna hai jo check kare **doodh aur chai patti** available hain ya nahi.  

### **✅ Example Output:**
```javascript
function makeChai() {
    let doodhHai = true;  // Block Scope Variable
    let chaiPattiHai = false; // Block Scope Variable

    if (doodhHai && chaiPattiHai) {
        console.log("Chai tayar ho gayi! ☕");
    } else {
        console.log("Saman kam hai, chai nahi ban sakti!");
    }
}

makeChai();
```
📢 **Output:**  
```
Saman kam hai, chai nahi ban sakti!
```
💡 **Kyun?** Kyunki `chaiPattiHai = false;` hai!  

🔹 Aap `chaiPattiHai = true;` kar ke dubara run karein!  

---

## **📌 Challenge 3: Petrol Bharao Ya Nahi? ⛽**
🚗 **Scenario:**  
Ali ka petrol ka tank sirf **10 liters petrol** store kar sakta hai.  
Agar petrol ka **level 2 liters se kam ho**, toh **"Warning! Petrol kam hai!"** print karna hai.  
Agar petrol **full ho jaye (10 liters)**, toh **"Tank full, aur petrol nahi dal sakte!"** kehna hai.  

📢 **Task:**  
- Ek **global variable** `petrolLevel = 5` rakhein.  
- Ek function **`fillPetrol(amount)`** likhein jo petrol **add kare**.  
- **Conditions** likhein:  
  - Agar **petrol 2 se kam ho** → `"Warning! Petrol kam hai!"`  
  - Agar **10 liters se zyada ho jaye** → `"Tank full, aur petrol nahi dal sakte!"`  

### **✅ Example Output:**
```javascript
let petrolLevel = 5;  // Global Variable

function fillPetrol(amount) {
    petrolLevel = petrolLevel + amount;

    if (petrolLevel < 2) {
        console.log("Warning! Petrol kam hai! ⛽");
    } else if (petrolLevel > 10) {
        console.log("Tank full, aur petrol nahi dal sakte!");
    } else {
        console.log("Petrol level: " + petrolLevel + " liters");
    }
}

fillPetrol(1);  // 5+1 = 6
fillPetrol(3);  // 6+3 = 9
fillPetrol(2);  // 9+2 = 11 (Tank full hoga!)
```
📢 **Output:**  
```
Petrol level: 6 liters
Petrol level: 9 liters
Tank full, aur petrol nahi dal sakte!
```
💡 **Samajh aaya?** Jab petrol **10 liters se zyada ho gaya, toh humne warning de di!**  

---

## **📌 Challenge 4: Mehmaan Aaye Toh Pani Pilao 🚰**
👳‍♂️ **Scenario:**  
Ghar mehmaan aaye hain, aur hum check karna chahte hain ke **pani ka glass available hai ya nahi**.  
Agar glass available hai, toh **"Mehmaan ko pani de diya!"** print karein.  
Agar nahi, toh **"Glass nahi hai, pehle glass le aao!"** print ho.  

📢 **Task:**  
- Ek function **`serveWater()`** likhna hai jo check kare ke **glass available hai ya nahi.**  
- Agar **glass true hai** → `"Mehmaan ko pani de diya!"`  
- Agar **false hai** → `"Glass nahi hai, pehle glass le aao!"`  

### **✅ Example Output:**
```javascript
function serveWater() {
    let glassAvailable = false; // Block Scope Variable

    if (glassAvailable) {
        console.log("Mehmaan ko pani de diya! 🥤");
    } else {
        console.log("Glass nahi hai, pehle glass le aao!");
    }
}

serveWater();
```
📢 **Output:**  
```
Glass nahi hai, pehle glass le aao!
```
🔹 **Agar aap `glassAvailable = true;` kar dein, toh kya output aayega?** 🧐  

---

## **🎯 Bonus Challenge: Apna Example Banao!**
Aap ek **apna khud ka desi example** likho jo **variables aur scoping** ko use kare.  
Agar kisi example mein **problem aa rahi hai**, toh mujhe bhej do, **main review kar ke bataunga!** 🚀  

📌 **👀 Example Idea:**  
- **Ghar ke bill ka budget check karna** 💡  
- **Bhai ka mobile balance check karna** 📱  
- **Dost se udhaar lena aur wapas karna** 💸  

👨‍💻 **Practice zaroor karo!** Jitna likhoge, utna samajh aayega! 🚀🔥