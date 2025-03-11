# Cold Hiring Mail Generator

Cold email generator for company using groq, langchain and streamlit. It allows users to input the URL of a company's careers page. The tool then extracts job listings from that page and generates personalized cold emails. These emails include relevant portfolio links sourced from a vector database, based on the specific job descriptions.

### Imagine a scenario:

- Any Service company lets say 'A' needs a Principal Software Engineer and is spending time and resources in the hiring process, on boarding, training etc
  
- Another company say 'B' is Software Development company can provide a dedicated software development engineer to comapny A. So, the business development executive from company B is going to reach out to company A via a cold email.


## User Interface :
<img width="1413" alt="Screenshot 1946-12-20 at 4 02 12 PM" src="https://github.com/user-attachments/assets/cdb419f6-5ed8-47dd-9898-37f81f501fc3" />

## Set-up:
1 . To get started we first need to get an `API_KEY` from here: [Groq](https://console.groq.com/keys). Inside `app/.env` update the value of `GROQ_API_KEY` with the API_KEY you created.

2 . To get started, first install the dependencies using:

```bash
 pip install -r requirements.txt
```

3 . Run the streamlit app:

```bash
streamlit run app/main.py
```

## Tech Stack :
- Python
- LangChain
- Groq (Mixtral-8x7B)
- ChromaDB (Vector Database for semantic search)
- Streamlit (Web UI)
- Pandas (Data handling)
- WebBaseLoader (Web scraping)

## How it Works:
- Scrape Job Listings → Extract job postings from LinkedIn.
- Extract & Structure Data → LLM processes text into JSON format.
- Store & Retrieve Portfolio Projects → Use ChromaDB for semantic search.
- Generate Cold Email → AI crafts personalized outreach messages.
- Streamlit UI → Provides an easy-to-use dashboard.

#### Note:- The code is specifically written for macOS 2014 Pro model , it'll run on windows and other os , if issues are raised , please let me know.
