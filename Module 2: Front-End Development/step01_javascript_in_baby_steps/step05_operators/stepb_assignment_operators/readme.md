## **2. Assignment Operators in JavaScript**  
Assignment operators are used to **assign values to variables**. They can also be used to modify values in a **shortcut** way.

| **Operator** | **Description** | **Example** |
|-------------|----------------|------------|
| `=` | Assigns a value | `a = 10` |
| `+=` | Adds and assigns | `a += 5` (Same as `a = a + 5`) |
| `-=` | Subtracts and assigns | `a -= 3` (Same as `a = a - 3`) |
| `*=` | Multiplies and assigns | `a *= 2` (Same as `a = a * 2`) |
| `/=` | Divides and assigns | `a /= 2` (Same as `a = a / 2`) |
| `%=` | Modulus and assigns | `a %= 4` (Same as `a = a % 4`) |

---

## **1. Simple Assignment (`=`)**
**Value assign karna**  
Aik variable ko koi bhi value dena.

### **Example: Aman Ki Jeb Ka Hisab**
```javascript
let amanKiJeb = 1000; // Aman ke paas 1000 rupay hain
console.log("Aman ke paas rupay: " + amanKiJeb);
```
💡 **Output:** `Aman ke paas rupay: 1000`

---

## **2. Addition and Assignment (`+=`)**
**Mazid paisay jama karna**  
Aik value ko doosri value se jama karke update karna.

### **Example: Aman Ne Pocket Money Save Ki**
```javascript
let jeb = 500; // Aman ke paas 500 rupay hain
jeb += 200; // Aman ne 200 aur save kar liye

console.log("Aman ke paas ab total: " + jeb + " rupay");
```
💡 **Output:** `Aman ke paas ab total: 700 rupay`

---

## **3. Subtraction and Assignment (`-=`)**
**Kuch paisay kharch karna**  
Aik value ko doosri value se minus karke update karna.

### **Example: Aman Ne Dosto Ko Chai Pilai**
```javascript
let jeb = 700; // Aman ke paas 700 rupay hain
jeb -= 150; // Chai pe 150 rupay kharch hue

console.log("Aman ke paas ab bacha hua paisa: " + jeb + " rupay");
```
💡 **Output:** `Aman ke paas ab bacha hua paisa: 550 rupay`

---

## **4. Multiplication and Assignment (`*=`)**
**Amount barhakar update karna**  
Aik variable ki value ko kisi number se multiply karna.

### **Example: Aman Ne Apna Paisa Double Kiya**
```javascript
let jeb = 500; // Aman ke paas 500 rupay hain
jeb *= 2; // Paisa double ho gaya

console.log("Aman ke paas ab total: " + jeb + " rupay");
```
💡 **Output:** `Aman ke paas ab total: 1000 rupay`

---

## **5. Division and Assignment (`/=`)**
**Paisay kis ratio se divide karna**  
Aik value ko kisi number se divide karke update karna.

### **Example: 5 Doston Ne Barabar Paisay Diye**
```javascript
let totalBill = 1000; // Hotel ka total bill 1000 rupay
totalBill /= 5; // 5 doston mein barabar baat diya

console.log("Har dost ka hissa: " + totalBill + " rupay");
```
💡 **Output:** `Har dost ka hissa: 200 rupay`

---

## **6. Modulus and Assignment (`%=`)**
**Baaki paisay dekhna**  
Ek value ko doosri se divide karke jo remainder bache use store karna.

### **Example: Mithai Ka Distribution**
```javascript
let totalMithai = 25; // Total 25 laddu hain
totalMithai %= 6; // 6 doston mein baantne ke baad kitne bache?

console.log("Baqi laddu: " + totalMithai);
```
💡 **Output:** `Baqi laddu: 1`

---

## **💡 Quick Practice Task for You!**
**Challenge:**  
1. Ek variable **`pocketMoney`** banayein (1000 rupees).  
2. **200 rupees** ka recharge karein (**-=**).  
3. **500 rupees** ka double karein (***=**).  
4. **300 rupees** 3 doston mein barabar divide karein (**/=**).  
5. Bache hue paisay console.log karein.  

Jaldi likho aur batao **kitna paisa bacha?** 😃