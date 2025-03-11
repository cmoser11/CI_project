# **Analyzing Confucius Institute Influence on University Syllabi**  

## **Overview**  
This project investigates the influence of **Confucius Institutes (CIs)** on university syllabi by analyzing large-scale academic course data. The study employs **natural language processing (NLP) and survival regression modeling** to assess how course content evolves in response to CI partnerships.  

Key components of the analysis:  
- **Extensive data cleaning** of millions of university syllabi  
- **Natural Language Processing (NLP) models** to detect content shifts  
- **OpenAI-powered university classification** for unidentified syllabi  
- **Survival analysis regressions** to quantify syllabus changes over time  

## **Methodology**  
### **1. Data Collection & Cleaning**  
- Processed **millions of university syllabi** from diverse institutions  
- Extracted metadata such as course titles, instructor names, and institutional identifiers  
- Implemented **custom regex and heuristic matching** to clean and standardize text data  

### **2. Predicting University Affiliation with OpenAI**  
Many syllabus files **lacked explicit university identifiers** (e.g., email addresses, university logos, or headers). To address this, we:  
- Trained an **OpenAI-powered text classification model** to infer university affiliation based on syllabus content  
- Used a **fine-tuned GPT model** to analyze course structure, terminology, and academic jargon to predict likely institutions  
- Implemented **few-shot learning techniques**, providing OpenAI models with labeled examples to improve accuracy  
- Validated predictions by comparing them to a subset of syllabi with known institutional affiliations  

### **3. NLP Analysis of Course Content**  
- **Tokenization, lemmatization, and topic modeling** to detect thematic changes  
- **TF-IDF and word embeddings (SpaCy, Scikit-learn)** to compare pre- and post-CI syllabi  
- **Sentiment and keyword analysis** to assess ideological or structural shifts in coursework  

### **4. Survival Analysis & Regression Modeling**  
- Utilized **Cox Proportional Hazards models** to examine syllabus changes over time  
- Measured whether **CIs influenced the longevity and prevalence** of specific course topics  
- Assessed **institutional characteristics** that correlated with higher or lower changes in course content  

## **Technologies & Tools**  
- **Programming Languages:** Python  
- **Data Processing:** Pandas, NumPy  
- **Natural Language Processing (NLP):** NLTK, SpaCy, OpenAI API  
- **Machine Learning & AI:** OpenAI GPT models, Scikit-learn  
- **Statistical Modeling:** Statsmodels, Lifelines (Survival Analysis)  
- **Visualization:** Matplotlib, Seaborn  
- **Development Environment:** Jupyter Notebook  


## **Key Findings & Insights**  
- **OpenAI-powered classification** successfully inferred university affiliations with **high accuracy**, particularly for institutions with distinct course structures  
- Found **institutional variations** in the degree of CI influence based on policy and governance structures  
