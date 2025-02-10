# Overview of Project
In this project, we explored and compared how different open-source generative AI models compose poetry based on user-provided themes and prompts. Our goal is to assess how effectively these models produce poems that align with the intended themes, emotions and settings while maintaining creativity and coherence. We ensured that the poems sound natural and adhere to poetic conventions. By evaluating each model’s performance, we aimed to identify which models excel at generating poetry and highlight areas where improvements are needed.


# Dependencies
Ensure the following dependencies are installed:

```markdown
pandas==1.5.3
nltk==3.7
torch==1.12.0
transformers==4.27.0
pronouncing==0.2.0
sentence-transformers==2.2.2
scikit-learn==1.2.2
textstat==0.7.2
seaborn==0.12.2
matplotlib==3.7.1
```

# Install dependencies
```markdown
pip install -r requirements.txt
```
- Run the ipynb files under scripts folder for all 6 models mentioned below:  
  - Code Ninja 7B Q4	
  - Gemma 2 2B Q4	
  - Llama 3.2 3B Instruct Q8	
  - Mistral 7B INSTRUCT Q4	
  - Openchat-3.5 7B		
  - QWEN2 7B Instruct Q4

- Run the **`Common-Metrics.ipynb`** file to generate a comparison of the key metrics for all six models.

# Folder Structure:
- scripts Folder:  
Contains six Python files, each dedicated to calculating metrics for a specific model. Additionally, it includes a comparison script that aggregates the metrics of all six models, performs a comparative analysis, and generates visualizations.  

- images Folder:  
Stores the images generated from key metrics, which are used for visualization and comparative analysis.

