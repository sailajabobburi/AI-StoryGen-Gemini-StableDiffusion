## **Approach**

### **Story Generation:**

- Use the power of Gemini to generate engaging children's stories based on randomly selected themes (e.g., friendship, bravery, adventure) and settings (e.g., forest, village, ocean).
- Utilize natural language processing (NLP) techniques to craft simple, imaginative narratives that are suitable for young readers.
- Divide each story into five distinct parts, ensuring a well-structured plot with a clear challenge and resolution, along with an underlying moral or lesson.

### **Protagonist Description:**

- Use Gemini to create a detailed description of the protagonist, including their physical traits (e.g., size, clothing, distinctive features) and personality traits (e.g., bravery, kindness).
- Ensure the protagonist’s description remains consistent throughout the story for visual coherence.

### **Image Generation:**

- Implement Stable Diffusion and image-to-image techniques to generate high-quality, visually engaging images for each scene of the story.
- First, generate the protagonist’s image based on the description provided by Gemini.
- For each of the five story parts, create corresponding visual prompts for Stable Diffusion, ensuring that the illustrations reflect the protagonist's actions, emotions, and environment.

### **Implementation and Workflow**

1. **Input Handling:**

  Automatically generate the story content using Gemini based on randomly chosen themes and settings.
  Collect detailed descriptions for the protagonist and corresponding scene prompts that will guide the image generation.

2. **Model Integration:**

  Integrate Stable Diffusion for generating both the protagonist and scene images.
  Fine-tune the prompts for image generation to ensure they are clear, concise, and visually aligned with the story’s narrative.

3. **Image Synthesis:**

  Use the protagonist’s description to generate the first image using Stable Diffusion.
  For subsequent scenes, employ image-to-image generation to maintain visual consistency by referencing the protagonist’s image, enhancing continuity across the story.

4. **Final Output:**

  Present a fully illustrated, 5-part children's story complete with high-quality images for each scene, ready to be showcased as a picture book.

  ---
# Execution Instructions

# Python version 3.10

To create a virtual environment and install requirements in Python 3.10 on different operating systems, follow the instructions below:

### For Windows:

Open the Command Prompt by pressing Win + R, typing "cmd", and pressing Enter.

Change the directory to the desired location for your project:


`cd C:\path\to\project`

Create a new virtual environment using the venv module:


`python -m venv myenv`

Activate the virtual environment:

`myenv\Scripts\activate`


Install the project requirements using pip:

`pip install -r requirements.txt`

### For Linux/Mac:
Open a terminal.

Change the directory to the desired location for your project:

`cd /path/to/project`

Create a new virtual environment using the venv module:

`python3.10 -m venv myenv`


Activate the virtual environment:

`source myenv/bin/activate`

Install the project requirements using pip:

`pip install -r requirements.txt`

These instructions assume you have Python 3.10 installed and added to your system's PATH variable.

## Execution Instructions if Multiple Python Versions Installed

If you have multiple Python versions installed on your system, you can use the Python Launcher to create a virtual environment with Python 3.10. Specify the version using the -p or --python flag. Follow the instructions below:

For Windows:
Open the Command Prompt by pressing Win + R, typing "cmd", and pressing Enter.

Change the directory to the desired location for your project:

`cd C:\path\to\project`

Create a new virtual environment using the Python Launcher:

`py -3.10 -m venv myenv`

Note: Replace myenv with your desired virtual environment name.

Activate the virtual environment:

`
myenv\Scripts\activate
`

Install the project requirements using pip:

`pip install -r requirements.txt`


### For Linux/Mac:
Open a terminal.

Change the directory to the desired location for your project:

`cd /path/to/project
`
Create a new virtual environment using the Python Launcher:


`python3.10 -m venv myenv`


Note: Replace myenv with your desired virtual environment name.

Activate the virtual environment:

`source myenv/bin/activate`

Install the project requirements using pip:

`pip install -r requirements.txt`


By specifying the version using py -3.10 or python3.10, you can ensure that the virtual environment is created using Python 3.10 specifically, even if you have other Python versions installed.

## Installations

The notebook will require GPU, we recommend using Google Colab for this purpose. You can simply upload these notebooks in your google drive and then it can be opened with Colaboratory.

If you have higher GPU RAM access you can try implementing the same with larger stable diffusion models to get even better reults. We have used comparatively simple models so that it can implemented on Google Colab free of cost.
