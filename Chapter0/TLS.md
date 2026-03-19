# 🔐 TLS (Transport Layer Security) 

## 📌 What is TLS?

TLS (Transport Layer Security) is a **cryptographic protocol** used to secure communication over a network.

* It is the **successor of SSL**
* Used in **HTTPS, email (SMTP), FTP, etc.**
* Provides:

  * **Authentication**
  * **Confidentiality (Encryption)**
  * **Integrity**

---

## ⚠️ Real-World Context

* The **Equifax breach (2017)** exposed ~147 million users
* Root cause: failure to patch a vulnerability
* Lesson: **TLS alone is not enough** — security also depends on system updates, configs, and practices

---

## 🎯 Goals of TLS

1. **Authentication** → Verify server identity
2. **Encryption** → Keep data confidential
3. **Integrity** → Ensure data is not altered

---

## 🔄 TLS Working Overview

TLS works in **two main phases**:

### 1️⃣ Handshake Phase

### 2️⃣ Data Transfer (Encryption) Phase

---

# 🤝 1. Handshake Phase (Most Important)

### 🔍 Purpose:

* Authenticate server (and optionally client)
* Establish shared keys securely

---

### 🧠 Step-by-Step Flow (Simplified)

1. **Client Hello**

   * Sends:

     * Supported TLS versions
     * Cipher suites
     * Random number

2. **Server Hello**

   * Chooses:

     * TLS version
     * Cipher suite
   * Sends:

     * Server random number
     * SSL/TLS certificate

3. **Certificate Verification**

   * Client verifies:

     * Certificate is issued by a trusted **CA**
     * Domain name matches
     * Certificate is not expired

4. **Key Exchange**

   * Client generates a **pre-master secret**
   * Encrypts it using **server’s public key**
   * Sends it to server

5. **Server Decrypts**

   * Uses **private key** to decrypt pre-master secret

6. **Session Key Creation**

   * Both compute:

     * **Master secret**
     * Then derive **session keys**

---


* Public key is used **only during handshake**
* Actual data encryption uses **symmetric session key**

---

## 🔑 Key Concepts in Handshake

### 🧾 TLS Certificate

Contains:

* Domain name
* Organization details
* Public key
* Issuer (CA)
* Digital signature

---

### 🏢 Certificate Authority (CA)

* Trusted third-party (e.g., DigiCert, Let’s Encrypt)
* Digitally signs certificate
* Allows browser to verify authenticity

---

### 🔐 Asymmetric Encryption (Used in Handshake)

* Public key → encrypt
* Private key → decrypt

Used for:

* Secure key exchange

---

# 🔒 2. Encryption Phase (Data Transfer Phase)

Once handshake is complete:

### ✅ Symmetric Encryption is used

* Same key for encryption & decryption
* Much faster than asymmetric encryption

---

### 🔁 Data Flow

1. Client encrypts data using session key
2. Sends to server
3. Server decrypts using same key

---

## ⚡ Why Hybrid Approach?

| Method     | Use           | Reason              |
| ---------- | ------------- | ------------------- |
| Asymmetric | Handshake     | Secure key exchange |
| Symmetric  | Data transfer | Fast and efficient  |

---

# 🧾 Data Integrity in TLS

### ✔️ Achieved using:

* **MAC (Message Authentication Code)** OR
* AEAD modes (like AES-GCM in modern TLS)

### 🔍 Purpose:

* Detect tampering
* Ensure message is unchanged

---

# 🔁 Session & Session Resumption

### 📌 Session

* A communication between client and server
* May persist across multiple connections

---

### ⚡ Session Resumption

* Skips full handshake
* Uses previous session data
* Improves performance

---

# 🔗 How TLS Enables HTTPS

### Flow:

1. You type:
   `https://example.com`

2. Browser:

   * Connects using TLS
   * Verifies certificate

3. If valid:

   * Secure channel established
   * 🔒 Padlock appears

---

### ✔️ Important:

* **HTTP + TLS = HTTPS**

---

### 🔸 Perfect Forward Secrecy (PFS)

* Uses ephemeral keys (Diffie-Hellman)
* Even if private key is leaked later → past data stays secure

---

### 🔸 Cipher Suite

Defines:

* Key exchange algorithm
* Encryption algorithm
* Hashing algorithm

Example:

```
TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256
```

---

### 🔸 Modern TLS Versions

* TLS 1.0, 1.1 → Deprecated ❌
* TLS 1.2 → Widely used ✔️
* TLS 1.3 → Faster & more secure 🚀

---


