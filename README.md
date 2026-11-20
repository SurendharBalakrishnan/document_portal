# Project Details
```
Project Name : Document Portal 
Description : This will be the end to end project for "llm-ops"
```

# First Step :
```
I used conda for virtual environment

step 1 - install env using conda

conda create -p <env or user preference>  python=3.10 -y 

step 2 - Activate conda
conda activate <your env path>
```
# Add Required Files 
```
1 .gitignore
2 requirements.txt
3 README.md
```
# Initial Commit
```
Created a Repository from my github account
and follow the below steps
git init
git add .
git commit -m "<your commit message goes here>"
git branch -M main
git remote add origin <your created repo link>
git push -u origin main
```

# Use Case

```
Document Portal - what you can do with this document portal?
1. Analysis any documents
2. Compare 2 documents
3. you can talk with single document
4. you can talk with multiple different document (pdf, word, pptx, etc)
we can add on with any use cases
We are going to build langchain 
Rag Based Architecture?
Rag architecture - How it Works?
```

# Deployment Architecture

```
Monolith Architecture and microservice Architecture
ci cd pipeline
llm based project -> RAG and Agent 
```

# Folder Structure
```
setup.py -> install project as a package
Logging -> for performing logging , dump log
Exception -> implement custom exception, raise and log it
src -> sourcecode complete code base 
    doccompare
    docanalysier
    multidocchat
    singledocchat
utlis - keep all utilities in this folder
notebook - experiments.ipynb
config - to manage all the configuration for this project
prompt - prompt details
app.py - 
templates - ui components , html
static - js files, css components
```

# Minimum Requirement 

```
1. LLM Model - groq, openai, gemini, calude, huggingface, ollama
2. Embedding Model - openai, huggingface, gemini
3. vectordatabase - cloud 
    3 variant 
        1. in memory
        2. ondisk
        3. cloudbased
```

# environment setup - deployment 

```
.env
aws secret manager - industry grade practice

GROQ_API_KEY=your_groq_api_key_here
GEMINI_API_KEY= your_gemini_api_key_here
```