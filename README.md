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

