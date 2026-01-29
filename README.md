# AR T-Shirts

**Bring your T-shirts to life with Augmented Reality!**  

This project allows you to create T-shirts with unique printed designs that trigger automatic Augmented Reality (AR) effects when scanned with a single QR code. Each T-shirt has its own AR content—animations, 2D sprites, or 3D models—activated automatically when the camera detects the printed design. Users don’t need to select anything; the experience starts as soon as the camera recognizes the T-shirt.

---

## **Features**

- **Multiple T-shirt designs**: Each shirt has a unique AR target and effect.
- **Automatic detection**: The AR effect starts automatically when the T-shirt is detected.
- **Single QR code**: All T-shirts use the same QR link to access the AR experience.
- **Supports 2D and 3D content**: Frame-by-frame sprite animations or GLB/GLTF 3D models.
- **Scalable**: Add new T-shirts simply by adding a new marker and assets folder.

---

## **How It Works**

1. Print your T-shirt design as a **marker**.  
2. Users scan the QR code that points to this repository’s **GitHub Pages URL**.  
3. The web app uses **MindAR + Three.js** to detect the marker.  
4. The corresponding AR effect is automatically activated (sprite animation, 3D model, or other effects).  

---

## **Project Structure**

ar-tshirts/
├─ index.html <-- main AR webpage
├─ style.css <-- global styles
├─ main.js <-- AR logic: detects markers and triggers effects
├─ assets/
│ ├─ markers/ <-- MindAR marker files for each T-shirt
│ │ ├─ tshirt1.mind
│ │ ├─ tshirt2.mind
│ │ └─ tshirt3.mind
│ ├─ models/ <-- sprites or 3D models for each T-shirt
│ │ ├─ tshirt1/
│ │ │ ├─ frame_0.png
│ │ │ ├─ frame_1.png
│ │ │ └─ ...
│ │ ├─ tshirt2/
│ │ │ ├─ animation.glb
│ │ │ └─ ...
│ │ └─ tshirt3/
└─ README.md

---

## **Adding a New T-Shirt**

1. Create a new marker using MindAR's [Image Target Generator](https://hiukim.github.io/mind-ar-js-doc/tools/target-image-generator.html).  
2. Save the `.mind` file in `assets/markers/`.  
3. Create a new folder in `assets/models/` with your sprites or 3D model.  
4. Add a new entry in `main.js` with the marker path and effect type.  
5. Commit and push changes to GitHub.  

The new T-shirt will be automatically recognized when scanned with the same QR code.

---

## **Requirements**

- Mobile device with a camera and WebGL support.  
- Modern browser (Chrome, Safari, Firefox).  
- Internet connection to access GitHub Pages.  

---

## **Demo**

Once deployed on GitHub Pages, scan the same QR code printed on any T-shirt to see the AR effects live.

---

## **Technologies Used**

- [MindAR.js](https://hiukim.github.io/mind-ar-js-doc/) for marker-based AR.  
- [Three.js](https://threejs.org/) for rendering 2D/3D content.  
- [GitHub Pages](https://pages.github.com/) for hosting the web app.

---

## **License**

MIT License
