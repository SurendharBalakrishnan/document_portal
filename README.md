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

# Project - "Document Portal" Overview

```
1. What we are doing here?

(Any document -> PDF, Word, Audio, Video, Images, Databases, pptx, xlsx, etc)

Document Analysis - Whatever document we are uploading, we will perform the analysis
    example : Upload a pdf file (Any document) -> it will do complete analysis of the pdf.
                -> Extract the Data
                -> Send Extracted data to LLM

Document Compare - Comparison between two files (Any document). 
    example : we have pdf1 and pdf2, we will compare between two pdf files.
            -> use case : let say you initiated a document, then you made some change and it become a new version of the document. so here we compare v1 and v2

Chat with Doc and MultiDoc - (end to end rag pipeline - Advanced RAG Enable)
either one document (Any document) or with multiple document (Any document), you can chat with all the document  
```

# Business Use cases

```
Use Case -> Assume a Company "Company A" Outsourcing products from 3rd party vendor.
            3rd party vendor - 
                -> sending Reports and Invoices to our Company mail
                -> Received Mail documents will be stored in the datalake like -> S3 , Azure Datalake
        -> We are Having a Portal -> Document Portal 
            1. This Will fetch the information from Reports and Invoices
            2. We can compare the Current invoice with the previous delivered Invoices
            3. We can make Analysis The Reports and Invoices
            4. we can do a Q and A Session with this Portal
        
        How we are Building this document portal - via LLM, RAG, Agents and Gen Ai

-> we can able to implement in any sector / domain. 
```