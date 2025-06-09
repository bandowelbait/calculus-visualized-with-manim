# calculus-visualized-with-manim
Calculus Made Easy 
📘 Why We Integrate and Differentiate

This project uses Manim (Mathematical Animation Engine) to visually explain differentiation and integration—two foundational concepts in calculus. It includes multiple animated scenes that show infinitesimal change, area under a curve, and instantaneous rate of change in an intuitive, visual way.

🎥 Ideal for educators, students, or creators looking to build conceptual understanding through animations.
🔧 Requirements
Python 3.8 or later
Manim Community Edition
Jupyter Notebook (for .ipynb file execution)
📁 Project Structure
📦Why-We-Integrate-and-Differentiate
 ┣ 📜 Why we integrate and differentiate [Organized].ipynb
 ┣ 📜 README.md
 ┗ 📂 media/
    ┗ (optional) Rendered videos/images will go here
▶️ How to Run the Notebook
Launch Jupyter:
jupyter notebook
Open Why we integrate and differentiate [Organized].ipynb.
Run each code cell using Shift + Enter:
Each scene is a subclass of Scene in Manim.
These cells do not execute the animations in the notebook directly, but define them for CLI rendering.
🎬 How to Render an Animation

Once a scene is defined in the notebook, you can render it from the terminal.

For example, to render the InfinitesimalChange animation:

manim -pql "Why we integrate and differentiate [Organized].ipynb" InfinitesimalChange
Or, if you've moved the scene to a Python file (recommended for large-scale rendering):

manim -pql your_file.py InfinitesimalChange
-p → Preview after rendering
-ql → Quick render (for speed); use -qm or -qh for medium/high quality
------------------------------------------------------------------------
🖼️ How to Render & Save a Thumbnail

To render and save a static thumbnail image:

Modify a scene (e.g. InfinitesimalChange) to include:
self.add(your_final_mobjects_here)
self.wait()
Render with the -s flag to export an image instead of a video:
manim -p -s -ql your_file.py InfinitesimalChange
The image will be saved by default in:

media/images/your_file/480p15/InfinitesimalChange.png
You can change output folder or resolution in the render command if needed.
