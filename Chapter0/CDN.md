
# 🚀 CDN (Content Delivery Network)

## 📌 What is CDN?

A CDN is a **distributed network of servers** that deliver content **closer to users**.

👉 Goal:

* Reduce latency
* Improve speed
* Handle traffic efficiently

---

## 🧠 Problem Without CDN

User in India requests a server in USA:

* High latency ⏳
* Slow loading 🐢
* Heavy load on origin server

---

## ⚡ Solution: CDN

* Copies content to **multiple global servers (edge servers)**
* User gets data from **nearest server**

---

## 🌍 How CDN Works

### 🔄 Step-by-step

1. User enters website URL
2. DNS resolves domain → CDN instead of origin server
3. CDN finds **nearest edge server**
4. Edge server:

   * If content cached → returns immediately ✅
   * If not → fetches from origin, caches it, then returns

---

## 🧾 Types of Content CDN Handles

* Static:

  * Images
  * CSS
  * JavaScript

* Dynamic (modern CDNs):

  * APIs
  * Videos
  * Streaming

---

## ⚙️ CDN Components

### 1. Edge Servers

* Located globally
* Serve cached content

### 2. Origin Server

* Main server where original content lives

### 3. Cache

* Stores copies of content

---

## 🔑 CDN Caching Concept

* Frequently accessed data stored temporarily
* Reduces:

  * Server load
  * Network distance

---

## 🔐 CDN + Security

CDNs also provide:

* DDoS protection
* TLS termination (handles HTTPS)
* Web Application Firewall (WAF)

---

## 🧠 CDN Example Flow

User (India) → CDN (Mumbai server)
Instead of → Origin (USA)

👉 Result:

* Faster load time ⚡
* Lower latency 📉

---







