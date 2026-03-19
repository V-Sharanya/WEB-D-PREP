## 🔹 What is a Protocol?

A **protocol** is a standardized set of rules that defines how data is:

* formatted
* transmitted
* received
* acknowledged

between devices in a network.

👉 In simpler terms:
**Protocol = rules that allow two systems to communicate reliably**

---

# 📌 Overview

HTTP and HTTPS are **application-layer protocols** used for communication between a **client (browser)** and a **server (website)**.

* **HTTP** → Not secure (plain text)
* **HTTPS** → Secure (encrypted using TLS)

---

# 🔹 1. What is HTTP?

**HTTP (HyperText Transfer Protocol)** is a protocol that defines how data is exchanged over the web.

👉 It follows a **request-response model**

## 🔁 Flow:

```text
Client (Browser) → HTTP Request → Server  
Server → HTTP Response → Client
```

---

## 🔹 Key Characteristics

* Stateless
* Runs on TCP
* Default port: **80**
* Data sent in **plain text**

---

## 🔹 Example HTTP Request

```http
GET /index.html HTTP/1.1
Host: example.com
```
---

## 🔴 Major Flaw of HTTP

* Data is sent in **plain text**
* No encryption ❌
* Vulnerable to:

  * **Man-in-the-middle attacks**
  * Data theft (passwords, cookies, etc.)

👉 Anyone intercepting packets can read the data.

---

## 🔹 HTTPS (HyperText Transfer Protocol Secure)

* HTTPS = **HTTP + Encryption**
* It uses **TLS (Transport Layer Security)**
  (SSL is outdated but still used as a term informally)

---


* Both **client and server** can encrypt/decrypt using a **shared session key**
* This key is established during the TLS handshake

---



## 🔹 Key Features

* Encryption ✅

* Data integrity ✅

* Authentication ✅

* Default port: **443**

---

# 🔐 3. How HTTPS Works

## 🔹 Step-by-Step

### 1. Client Hello

* Browser sends supported encryption algorithms

### 2. Server Hello

* Server responds with:

  * SSL/TLS certificate
  * Public key

### 3. Certificate Verification

* Browser verifies:

  * Certificate authority (CA)
  * Domain validity

### 4. Key Exchange

* Session key generated securely

### 5. Secure Communication

* Data encrypted using symmetric key

---

## 🔑 Encryption Breakdown

| Type       | Usage         |
| ---------- | ------------- |
| Asymmetric | Key exchange  |
| Symmetric  | Data transfer |

---



# 🔁 6. Full Request Lifecycle

```text
1. Enter URL
2. DNS lookup → IP
3. TCP connection established
4. TLS handshake (HTTPS only)
5. HTTP request sent
6. Server processes request
7. HTTP response returned
8. Browser renders page
```

---

# 📦 7. HTTP Methods

| Method | Purpose       |
| ------ | ------------- |
| GET    | Retrieve data |
| POST   | Send data     |
| PUT    | Update data   |
| DELETE | Remove data   |

---

# 📊 8. HTTP Status Codes

| Code | Meaning      |
| ---- | ------------ |
| 200  | OK           |
| 301  | Redirect     |
| 400  | Bad Request  |
| 401  | Unauthorized |
| 404  | Not Found    |
| 500  | Server Error |

---

# 🍪 9. Stateless Nature & Solutions

## 🔹 Problem

HTTP is stateless:

* Each request is independent

## 🔹 Solutions

* Cookies
* Sessions
* Tokens (JWT)

---

# ⚡ 10. HTTP vs HTTPS

| Feature    | HTTP                   | HTTPS           |
| ---------- | ---------------------- | --------------- |
| Security   | ❌ No                   | ✅ Yes           |
| Encryption | ❌                      | ✅ TLS           |
| Port       | 80                     | 443             |
| Speed      | Faster (no encryption) | Slight overhead |
| Usage      | Rare today             | Standard        |

---

