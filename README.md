# 🐕 Osaka — Interactive 3D Web Experience

A **high‑end interactive web experience** inspired by Dogstudio’s design philosophy, blending **React, Three.js, GSAP, and WebGL** to create a cinematic, scroll‑driven 3D environment.

This project focuses on **emotional storytelling, motion, and material transitions**, delivering a premium creative‑developer portfolio piece.

---

## ✨ Features

* 🎥 **Scroll‑driven 3D animation** using GSAP + ScrollTrigger
* 🐶 **Animated 3D Dog model** (GLTF) with skeletal animation
* 🎨 **Dynamic Matcap material transitions** on hover
* 🖼️ **Image‑driven background transitions** synced with UI
* ⚡ **GPU‑optimized rendering** with custom shader logic
* 🧠 **Custom `onBeforeCompile` shader manipulation**
* 📱 **Responsive layout** with modern typography

---

## 🛠 Tech Stack

### Frontend

* **React**
* **@react-three/fiber**
* **@react-three/drei**
* **Three.js**

### Animation

* **GSAP**
* **GSAP ScrollTrigger**

### 3D & Graphics

* **GLTF models**
* **Matcap materials**
* **Normal maps**
* **Custom fragment shader blending**

### Styling

* **SCSS / CSS nesting**
* **Custom web fonts**

---

## 📂 Project Structure

```bash
src/
├── components/
│   └── Dog.jsx        # 3D model, shaders & animations
├── App.jsx            # Main layout & Canvas
├── App.css            # Global & section styles
public/
├── models/            # GLTF / DRACO models
├── matcap/            # Matcap textures
├── fonts/             # Custom typography
├── images/            # Hover background images
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/osaka.git
cd osaka
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the Development Server

```bash
npm run dev
```

The app will run on:

```
http://localhost:5173
```

---

## 🎮 Interaction Guide

* **Scroll** → Drives the 3D dog’s position & rotation
* **Hover on project titles** →

  * Background image fades in
  * Dog material smoothly transitions using shader blending
* **Leave titles section** → Reverts to default material

---

## 🧩 Shader Logic (Matcap Transition)

* Two matcap textures are blended using a **custom uniform (`uProgress`)**
* Transition is calculated in the **fragment shader**
* GSAP animates the uniform for buttery‑smooth material morphing

> This avoids material re‑creation and keeps GPU performance optimal.

---

## 📸 Preview

> Add screenshots / screen recordings here for maximum impact.

---

## 🧠 Learnings & Takeaways

* Advanced **Three.js material customization**
* Integrating **GSAP with WebGL shaders**
* Performance‑friendly **scroll‑based storytelling**
* Building **award‑style portfolio experiences**

---

## 📌 Inspiration

Inspired by:

* **Dogstudio®**
* **Awwwards‑level interactive websites**

This project is built for **learning & portfolio purposes**.

---

## 👨‍💻 Author

**Chetan Kumawat**
Creative Frontend / WebGL Developer


---

## 📜 License

This project is licensed for **personal & educational use**.

---

⭐ If you like this project, don’t forget to **star the repository**!
