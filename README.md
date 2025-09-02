# Materials for the course "GenAI-Powered Data Analysis with Python" for O'Reilly by Dr. Chester Ismay

# Course content

The major files in this repository are
- `slides.pdf`: PDF version of the slides used in this course to motivate the code.
- `economies.csv`: Data for code walkthroughs, one as Comma-Separated Values and the other as a Microsoft Excel file
- `populations.csv`: Data for student exercises.
- `exercises.ipynb`: A Jupyter Notebook with pseudocode/instructions provide to be filled in for code walkthroughs and student exercises
- `exercises_solutions.ipynb`: A Jupyter Notebook with answers to the code walkthroughs and exercises. An HTML version of these solutions is available at https://ismay-oreilly-aidap.netlify.app/exercises_solutions.html and is the recommended way to view solutions.

## Recommended instructions on getting set up with Python and Jupyter Notebook

If you aren't able to do this on your machine, you may want to check out [Google Colab](https://colab.research.google.com/). 
It's a free service that allows you to run Jupyter notebooks in the cloud. 
Alternatively, I've set up some temporary notebooks on Binder [here](https://mybinder.org/v2/gh/ismayc/oreilly-genai-powered-data-analysis-with-python/HEAD?urlpath=%2Fdoc%2Ftree%2Fexercises.ipynb) that you can work with online as well.

### Step 1: Install Python
- **Option 1: Anaconda Installation**:
  - **Download Anaconda**: Go to the [official Anaconda website](https://www.anaconda.com/products/distribution) and download the latest version of Anaconda for your operating system (Windows, macOS, or Linux). Anaconda conveniently installs Python, Jupyter Notebook, and many other commonly used packages for data science and machine learning.
- **Option 2: Python Installation**:
  - **Download Python**: Alternatively, you can download Python directly from the [official Python website](https://www.python.org/downloads/) and install the latest version for your operating system.

### Step 2: Launch Jupyter Notebook
- **Launch Jupyter Notebook**:
  - **Anaconda**: After installing Anaconda, open Anaconda Navigator from your Start Menu (Windows) or using the Anaconda Navigator application (macOS/Linux). In Anaconda Navigator, find Jupyter Notebook in the list of available applications and click on the "Launch" button. This will open Jupyter Notebook in your default web browser.
  - **Python Installation**: Open your command prompt (Windows) or terminal (macOS/Linux), and install Jupyter using pip:
    ```bash
    pip install notebook
    ```
    After installation, you can launch Jupyter Notebook by running:
    ```bash
    jupyter notebook
    ```

### Step 3: Install Required Libraries
- **Open Anaconda Prompt (Windows) or Terminal (macOS/Linux)** (if using Anaconda), or **open your command prompt (Windows) or terminal (macOS/Linux)** (if using Python installation).
- **Install Required Libraries using conda (Anaconda)**:
  ```bash
  conda install pandas matplotlib seaborn plotly
  ```
- **Install Required Libraries using pip** (if not using Anaconda):
  ```bash
  pip install pandas matplotlib seaborn plotly
  ```

### Step 4: Verify Installation
- **Create a new notebook**: In the Jupyter Notebook interface, click on "New" and select "Python 3" to open a new notebook.
- **Test the installation of the libraries**:
  - Import the libraries in the first cell of your notebook:
    ```python
    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns
    import plotly.express as px
    import plotly.graph_objects as go
    from plotly.subplots import make_subplots
    
    # For plotly to load directly in Jupyter notebook
    import plotly.offline as pyo
    pyo.init_notebook_mode(connected=True)
    ```
    
  - Run the cell (`Shift + Enter`). If no errors appear, the libraries are installed correctly.

## Tips for Using ChatGPT Effectively During the Course

This course emphasizes how GenAI can support learning, exploration, and problem solving. Here are a few ways to use ChatGPT while working through the materials:

### General Prompts

* **Clarify Concepts**: Ask *"Explain this code step by step"* or *"What does `groupby()` mean in plain English?"*
* **Alternative Approaches**: Try *"Show me a shorter way to write this in pandas"* or *"Is there a more efficient method for this task?"*
* **Debugging Help**: Paste error messages and ask *"Why am I getting this error and how can I fix it?"*

### Data Wrangling with Pandas

* When cleaning data, ask *"How can I fill in these missing values?"* or *"Why am I seeing NaNs after merging?"*
* When summarizing data, try variations like *"Explain what `agg()` does with an analogy"* or *"Give me three examples of grouping this dataset differently."*

### Visualization

* Use prompts like *"Which type of plot is best for comparing distributions?"* or *"Rewrite this seaborn code to add better labels."*
* For Plotly, ask *"How can I add interactivity for executives?"* or *"Suggest three ways to make this chart easier to interpret."*

### Storytelling with Data

* After generating insights, ask *"Turn this into a 3-sentence story for a stakeholder"* or *"Give me two alternative angles to present this insight."*
* Use *"Reword this finding for a newsletter audience"* to practice adapting your narrative for different readers.

### Reflection and Practice

* End each exercise by asking ChatGPT for **three new questions** you could ask of your dataset.
* Practice **prompt engineering** by rewriting the same request in different ways (short, step-by-step, analogy-based) and comparing responses.

---

## Example Prompt Templates

You can copy and adapt these while working through the exercises:

* *"Explain what this code is doing as if I’m new to Python."*
* *"Fix this error: [paste error message]."*
* *"Write three different visualizations of this dataset: one in Matplotlib, one in Seaborn, and one in Plotly."*
* *"Suggest improvements to make this chart more audience-friendly."*
* *"Summarize my dataset in three sentences and suggest next questions to explore."*

## Resources and References

Here are some helpful links for both technical topics and GenAI guidance:

### Python and Libraries

* [Python Documentation](https://docs.python.org/3/)
* [Pandas Documentation](https://pandas.pydata.org/docs/)
* [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
* [Seaborn Documentation](https://seaborn.pydata.org/)
* [Plotly Express Documentation](https://plotly.com/python/plotly-express/)

### Jupyter and Setup

* [Jupyter Notebook Documentation](https://jupyter-notebook.readthedocs.io/en/stable/)
* [Google Colab Guide](https://colab.research.google.com/notebooks/intro.ipynb)
* [Binder Quickstart](https://mybinder.org/)

### GenAI and Prompting

* [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
* [ChatGPT for Data Science Tutorials](https://towardsdatascience.com/) *(searchable collection of articles)*
* Suggested practice: keep a "Prompt Log" notebook where you track which prompts worked best for you.
