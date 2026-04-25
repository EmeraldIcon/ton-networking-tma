# TON Social Networking Ecosystem (Telegram Mini App)

### **Project Overview**
This project is a high-velocity Telegram Mini App (TMA) designed for professional networking and lead generation. Built to live within the Telegram interface, it leverages the **TON (The Open Network)** blockchain for decentralized interactions and a pure PHP backend for maximum server-side efficiency.

> **Note:** This is an architectural overview. The core backend logic and database schemas are proprietary.

---

### **Technical Architecture**
* **Frontend:** Telegram Web App (TWA) standard with lightweight JavaScript for UI responsiveness.
* **Backend:** **Pure PHP (8.x)** - Chosen for rapid execution, low memory footprint, and high-performance Server-Side Rendering (SSR).
* **Web3 Integration:** **Wallet Connect v2** for secure TON wallet linking and transaction signing.
* **Payment Rails:** Dual-provider setup using **Stripe** (International) and localized TON-based payments.
* **Real-Time Communication:** **Agora SDK** for high-fidelity audio/video calling within the Telegram window.

---

### **Engineering Highlights**

#### **1. The "Pure PHP" Advantage**
In an era of heavy Node/React overhead, I architected this system using Pure PHP to ensure the Mini App loads instantly on any mobile device, regardless of network conditions in emerging markets. This allows for near-zero TTI (Time to Interactive).

#### **2. Multi-Currency Payment Engine**
Developed a hybrid payment gateway that detects user location and preference:
* **Fiat:** Handled via Stripe Webhooks for subscription-based features.
* **Crypto:** Integrated Wallet Connect to allow users to interact with TON assets directly.

#### **3. Real-Time Networking**
Integrated **Agora RTC** to move professional networking from text to voice. Managed RTC token generation on the PHP backend to ensure secure, authorized access to private call rooms.

---

### **System Workflow**
1. **Auth:** User enters via Telegram Bot -> HMAC-SHA256 verification of `initData`.
2. **Profile:** PHP generates the user profile dashboard via SSR.
3. **Connect:** Wallet Connect initializes a session for on-chain identity.
4. **Interact:** Users initiate Agora-powered calls for instant networking.

---

### **Contact & Access**
For technical review or partnership inquiries regarding the EmeraldIcon ecosystem, reach out via [LinkedIn](YOUR_LINKEDIN_URL).
