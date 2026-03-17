# 🌐 DNS Resolution — Short Structured Notes

---

## 📌 1. What is DNS?

> DNS (Domain Name System) translates **domain names → IP addresses**

Example:

```id="dns1"
google.com → 142.250.x.x
```

---

## 📌 2. Why DNS is Needed

* Humans remember names (google.com)
* Computers use IP addresses
* DNS acts like a **phonebook of the Internet**

---

## 📌 3. DNS Resolution Flow (Step-by-Step)

```id="dnsflow"
User → Browser Cache → OS Cache → ISP Resolver → Root → TLD → Authoritative Server
```

---

## 📌 4. Step-by-Step Explanation

### 1. Browser Cache

* First check in browser cache
* If found → return IP

---

### 2. OS Cache

* If not in browser → check system cache

---

### 3. ISP DNS Resolver

* Query goes to ISP’s DNS server (resolver)
* It also checks its cache

---

### 4. Root Server

* There are **13 logical root server systems worldwide**
* Managed by global organizations

✔️ Root server DOES NOT give IP
✔️ It tells:

> “Go ask this TLD server”

---

### 5. TLD Server (Top-Level Domain)

* Handles domains like:

  * `.com`
  * `.org`
  * `.net`

✔️ TLD also DOES NOT give final IP
✔️ It says:

> “Ask this authoritative server”

---

### 6. Authoritative Name Server

* Final source of truth ✅
* Stores actual IP of domain

✔️ Returns:

```id="dns2"
google.com → 142.250.x.x
```

---

### 7. Response Back

* Resolver gets IP
* Sends it back to your device
* Stores it in cache

---

## 📌 5. Caching (Very Important)

* Happens at multiple levels:

  * Browser
  * OS
  * ISP resolver

✔️ Makes future requests faster
✔️ Reduces load on servers

---

## 📌 7. Complete Flow Summary

```id="dnsfinal"
1. Check local cache
2. Ask ISP resolver
3. Resolver → Root server
4. Root → TLD server
5. TLD → Authoritative server
6. Authoritative → IP address
7. Cache + return to user
```

---

## 🧠 Mental Model

* DNS = Phonebook 📖
* Root = Directory of categories
* TLD = Category section (.com)
* Authoritative = Exact contact details

---
