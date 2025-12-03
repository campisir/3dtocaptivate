# Repository Contents

This repository provides a basic setup for working with 3D models using Three.js. The `three-js` folder contains essential JavaScript libraries and utilities for rendering and interacting with 3D content. You will use the files in the `three-js` folder every time you work with this project.

The files `example.mtl`, `example.obj`, and any example `.png` images are provided strictly for demonstration purposes. **You should use your own `.mtl`, `.obj`, and texture files** for your actual projects. The example files are only meant to help you get started and understand how to structure your own assets.

---
  
How to include a 3D model in an Adobe Captivate project
------------------------------------------------------

What you need
- .mtl file
- .obj file
- Base color PNG (albedo)
- Normal map PNG

Step-by-step

1. Create a copy of index.html
   - Duplicate the example index.html so you don't overwrite the original.
   - Rename the copy to a unique filename (for example: my-model-viewer.html).

![GIF placeholder for Step 1](assets/gifs/step-1.gif)

2. Edit the HTML to point to your model files
   - Open your copied HTML and replace the example filenames:
     - Change "Item 1 3d finished.mtl" → your-file.mtl
     - Change "Item 1 3d finished.obj" → your-file.obj
   - Save the file under the unique name you chose.

![GIF placeholder for Step 2](assets/gifs/step-2.gif)

3. Add a link from Captivate to the HTML file
   - In Captivate, create a button where you want users to open the model.
   - Link the button to the HTML file.

![GIF placeholder for Step 3](assets/gifs/step-3.gif)

4. Publish your Captivate project
   - Complete and publish the Captivate project as you normally would.
 
 ![GIF placeholder for Step 4](assets/gifs/step-4.gif)

5. Copy three-js and your model files into the published project
   - After publishing, open the output folder.
   - Copy the three-js folder (runtime/scripts, shaders, etc.) into the published output folder.
   - Copy your .mtl, .obj, base color PNG, and normal PNG into the same folder (or a subfolder) referenced by your HTML.
  
  ![GIF placeholder for Step 5](assets/gifs/step-5.gif)

6. Test on a local server
   - Start a simple local server (e.g., Python: python -m http.server) in the published output folder and open the Captivate output in a browser.
   - Click the button in your Captivate content to open the HTML viewer — the model should render.

![GIF placeholder for Step 6](assets/gifs/step-6.gif)
---

**Note:** You can add as many 3D models to your Captivate project as you want, as long as all the associated files (such as `.obj`, `.mtl`, and texture images) have unique filenames. This ensures there are no conflicts when loading multiple models. You only need to add the `three-js` folder once.

