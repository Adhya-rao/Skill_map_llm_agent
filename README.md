# Generative AI Job Market Assistant

## Overview
This project is a **Generative AI Job Market Assistant** built using *LangChain Agents*, *Google Gemini*, and the *JSearch API*.  
The assistant analyzes **industry demand for a specific skill** and retrieves **relevant job openings in India**.

It demonstrates important **Generative AI concepts** such as:
* LLM-powered reasoning
* Tool calling
* External API integration
* Structured data responses

---

## Features
* Check **industry demand** for specific AI or technology skills.
* Retrieve **real-time job openings** using an external API.
* Uses **LangChain Agent** for intelligent tool orchestration.
* Integrates **Gemini LLM** for reasoning and decision making.
* Returns **structured job results** including title, company, location, and application link.

---

## Tech Stack
* Python
* LangChain
* Google Gemini LLM
* RapidAPI JSearch API
* Requests Library
* Google Colab Secrets for API keys

---

## Project Architecture
The system works in the following steps:

1. User sends a query asking about **skill demand and job openings**.
2. The **LangChain Agent** analyzes the query.
3. The agent calls the appropriate tools:
   * `skill_demand_tool` → checks demand for the skill.
   * `search_jobs` → retrieves job openings from the JSearch API.
4. The results are combined and returned to the user.

---

## Tools Implemented

### Skill Demand Tool
This tool checks the **industry demand** for a given skill.

Example output:
* Generative AI → Very High Demand
* Python → High Demand
* Machine Learning → High Demand

---

### Job Search Tool
This tool retrieves **job openings** using the JSearch API.

Returned job information includes:
* Job Title
* Company Name
* Location
* Application Link

Example result:

Title   : Generative AI Engineer  
Company : ShellKode  
Location: Bagaluru  
Apply   : https://job-link  

---

## Installation

### Clone the Repository
git clone https://github.com/yourusername/genai-job-assistant.git  
cd genai-job-assistant  

### Install Dependencies
pip install langchain requests  

---

## API Keys Setup
This project requires the following API keys:

* RapidAPI Key (for JSearch API)
* Gemini API Key

In **Google Colab**, store them using Secrets:

RAPIDAPI_KEY = "your_api_key_here"  
GEMINI_API_KEY = "your_api_key_here"  

---

## Example User Query
What's the demand for generative ai in the industry and show me related job openings in India

---

## Example Output

Demand:  
The demand for Generative AI is very high. Companies are actively hiring for roles like LLM Engineers, AI Engineers, and Prompt Engineers.

Job Openings:

Title   : Research Intern – Generative AI Agents  
Company : SynergyLabs  
Location: Gurugram  
Apply   : https://job-link  

Title   : Generative AI Engineer  
Company : ShellKode  
Location: Bagaluru  
Apply   : https://job-link  

---

## Key Concepts Demonstrated
* Generative AI Agents
* Tool Calling with LangChain
* External API Integration
* LLM-based reasoning
* Structured job data extraction

---

## Future Improvements
* Add **Streamlit UI for interactive job search**
* Implement **automatic skill extraction from user queries**
* Add **resume matching with job descriptions**
* Integrate **vector database for job recommendations**

---

## Author
Adhya

---

## License
This project is created for **educational and demonstration purposes**.
