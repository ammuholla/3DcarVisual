# 3DcarVisual4
The goal of this project was to create an interactive 3D web application that showcases a car model and allows a user to dynamically change its materials, lighting, and camera perspective. This demonstrates key principles of real-time 3D rendering in a web browser, including:
•	Model Loading: Efficiently loading a complex 3D model with textures.

•	Dynamic Material Application: Allowing users to change the appearance of different parts of the car (body, rims, glass) on the fly.

•	Lighting Control: Simulating different lighting environments, from a showroom to a dark night scene, to observe how materials react.

•	Interactive Controls: Providing a user-friendly interface for manual adjustments (dropdown menus) and a voice-activated chatbot for a more natural, conversational experience.

•	Physics and Animation: Implementing basic car physics and a camera that can follow the car's movement to create a more immersive and engaging experience.

The core challenge was to build a robust and performant application that could handle these features without sacrificing a smooth frame rate, all while running entirely within a web browser.

IMPLEMENTATION DETAILS:
•	Scene Initialization: The main.js script sets up the Three.js scene, camera, and renderer. It also loads a skybox to create realistic reflections.

•	Model Identification: The initCar() function loads the model and identifies different parts (body, rims, glass) so they can be individually customized.

•	Customization Logic: Materials and lighting presets are pre-defined, and functions like updateMaterials() and updateLighting() apply the user's choices. This logic can also be extended to include Augmented Reality (AR), which is used to detect and anchor the 3D car model to a real-world surface via the follow up camera. This allows the virtual lighting and reflections to respond to the real-world environment. The existing voice and UI controls would be adapted for the AR environment, allowing users to tap the screen or use a voice command like "place car" to set the model on a surface.

•	Interactive Controls: User input comes from both dropdown menus and a voice-activated chatbot. The handleCommand() function parses voice commands to trigger actions.

•	Animation Loop: The update() function runs continuously to manage car physics, animate the camera, and render the scene for a real-time visual experience.

