# **Logical Operators in JavaScript**  
Logical operators **combine multiple conditions** and return a **Boolean (true or false)**.

| **Operator** | **Name** | **Description** |
|-------------|---------|----------------|
| `&&` | AND | Dono conditions `true` honi chahiye warna `false`. |
| `||` | OR | Koi ek condition `true` ho to result `true`. |
| `!` | NOT | Value ka **ulta** (negation) return karta hai. |

---

## **1. AND (`&&`) Operator**
**Sirf tab `true` hoga jab dono conditions `true` hongi.**  
Agar koi ek `false` ho to result `false` hoga.

### **Example: Cinema Ticket ka Scene** 🎟️
Ali aur Usman dono ka ticket hona zaroori hai tabhi andar ja sakte hain.

```javascript
let aliKaTicket = true;
let usmanKaTicket = false;

console.log(aliKaTicket && usmanKaTicket); // false (kyunki Usman ka ticket nahi hai)
```
💡 **Output:**  
```
false
```

---

## **2. OR (`||`) Operator**
**Agar ek bhi condition `true` ho to result `true` hoga.**  
Sirf tab `false` hoga jab dono `false` hon.

### **Example: Cricket Match Dekhna** 🏏  
Agar ghar pe **TV** chal raha hai ya **mobile** pe live stream hai, to match dekha ja sakta hai.

```javascript
let gharKaTVChalRahaHai = false;
let mobilePeLiveStreamHai = true;

console.log(gharKaTVChalRahaHai || mobilePeLiveStreamHai); // true (kyunki mobile pe stream hai)
```
💡 **Output:**  
```
true
```

---

## **3. NOT (`!`) Operator**
**`!` kisi bhi value ka ulta kar deta hai.**  
- `true` ko `false` banata hai  
- `false` ko `true` banata hai

### **Example: Burger Khana Allowed Hai? 🍔**
Burger sirf tab nahi milega agar **diet mode** on hai.

```javascript
let dietModeOn = true;

console.log(!dietModeOn); // false (kyunki diet mode on hai, burger nahi milega)
```
💡 **Output:**  
```
false
```

---

## **💡 Practice Task for You!**
1. Ek variable `baarishHoRahiHai` (true) aur `chhatriHai` (false) banao.
2. **Check karo** kya **baarish aur chhatri dono hain? (`&&`)**
3. **Check karo** kya **kam az kam ek condition sahi hai? (`||`)**
4. **Check karo** kya **baarish ho rahi hai ya nahi? (`!`)**

Jaldi likho aur batao **baarish me bheegne wale ho ya nahi?** ☔😃