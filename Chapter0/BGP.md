
# 🌐 BGP (Border Gateway Protocol)

## 📌 What is BGP?

BGP is the **routing protocol of the internet**.

* It decides:
  👉 *“Which path should data take across networks?”*
* It works between **Autonomous Systems (AS)**

---

## 🧠 Key Concept: Autonomous System (AS)

* An **AS** = a large network controlled by one organization
  Examples:

  * ISPs (Airtel, Jio)
  * Google network
  * Amazon AWS

Each AS has:

* A unique **ASN (Autonomous System Number)**

---

## 🔄 How BGP Works

### 🔍 Basic Idea:

* Networks (AS) **announce routes**
* Other networks decide **best path**

---

### 🧾 Example Flow

1. You request a website (say google.com)

2. Your ISP (AS1) asks:

   * “Which path leads to Google’s network (AS2)?”

3. Multiple routes exist:

   * AS1 → AS3 → AS2
   * AS1 → AS4 → AS5 → AS2

4. BGP selects **best path based on policies**, NOT just shortest path

---

## ⚙️ BGP Decision Factors

BGP does NOT simply choose shortest path. It considers:

* Path length (AS hops)
* Local preference
* Routing policies
* Network agreements (business decisions)

👉 Important:
**BGP is policy-based, not purely technical**

---

## 🔁 BGP Message Types

* **OPEN** → establish connection
* **UPDATE** → share routes
* **KEEPALIVE** → maintain connection
* **NOTIFICATION** → errors

---

## 🚨 Real-World Issue

### BGP Hijacking

* A malicious AS announces fake routes
* Traffic gets redirected

👉 Example:

* Traffic meant for Google goes to attacker

---


