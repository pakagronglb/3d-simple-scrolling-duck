# 🦆 3D Simple Duck Animations with Scrolling 



https://github.com/user-attachments/assets/cde30f9f-2b8a-4e00-8bf6-01137f06f0bc



[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Three.js](https://img.shields.io/badge/Three.js-black?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
[![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)](https://greensock.com/gsap/)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=for-the-badge&logo=framer&logoColor=white)](https://www.framer.com/motion/)
[![React Spring](https://img.shields.io/badge/React_Spring-1fd1f9?style=for-the-badge&logo=react&logoColor=white)](https://react-spring.dev/)

A simple guide to implementing various animation techniques in 3D web development using React Three Fiber. This guide covers:

## 👾 Animation Techniques

- **Lerp (Linear Interpolation)**
  - Interpolates between two values for smooth animations
  - Control animation speed with interpolation factor
  - Example usage with useFrame:
  ```javascript
  const value = THREE.MathUtils.lerp(start, end, t);
  ```

- **Float Animations**
  - Using Drei's Float component for natural floating effects
  - Customizable parameters:
    ```javascript
    <Float floatIntensity={2} speed={3} rotationIntensity={1}>
      <Duck />
    </Float>
    ```
  
- **GSAP Animations**
  - Timeline management
  - Color transitions
  - Scroll-based animations
  - Example:
    ```javascript
    gsap.timeline()
      .to(target, { duration: 1, color: "#ffc544" })
      .to(target, { duration: 1, color: "#7c4e9f" });
    ```
  
- **Spring-Based Animations**
  - Framer Motion implementation with motion components
  - Physics-based natural movements
  - Variants support for structured animations
  - Global spring configurations:
    ```javascript
    <MotionConfig transition={{ 
      type: "spring", 
      mass: 5, 
      stiffness: 500, 
      damping: 42 
    }}>
    ```

## 🔑 Key Features

- 🎨 Multiple animation approaches
- 🔄 Smooth transitions
- 📜 Scroll-based animations
- 🎯 Interactive examples
- 🔧 Practical implementations
- 🌊 Physics-based movements
- 🎭 Animation variants support

## 💻 Technologies Used

- React Three Fiber
- Three.js
- GSAP
- Framer Motion
- React Spring

## 🙏🏻 Credit

This guide is based on the excellent course material from [Wawa Sensei](https://wawasensei.dev/). Check out their comprehensive courses and tutorials on 3D web development!

Note: The 3D model animations are covered in the models chapter.

**Lerp**
Lerp is a mathematical function that interpolates between two values. It is useful to animate a value from one point to another.

**Copy**
``const value = THREE.MathUtils.lerp(start, end, t);``
The first parameter is the start value, the second parameter is the end value and the third parameter is the interpolation factor between 0 and 1.
The closer the interpolation factor is to 0, the slower the animation will be. The closer the interpolation factor is to 1, the faster the animation will reach the end or target value.

