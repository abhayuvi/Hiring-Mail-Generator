# Cold Hiring Mail Generator

Cold email generator for company using groq, langchain and streamlit. It allows users to input the URL of a company's careers page. The tool then extracts job listings from that page and generates personalized cold emails. These emails include relevant portfolio links sourced from a vector database, based on the specific job descriptions.

### Imagine a scenario:

- Any Service company lets say 'A' needs a Principal Software Engineer and is spending time and resources in the hiring process, on boarding, training etc
  
- Another company say 'B' is Software Development company can provide a dedicated software development engineer to comapny A. So, the business development executive from company B is going to reach out to company A via a cold email.


## User Interface :
<img width="1413" alt="Screenshot 1946-12-20 at 4 02 12 PM" src="https://github.com/user-attachments/assets/cdb419f6-5ed8-47dd-9898-37f81f501fc3" />

## Set-up:
1 . To get started we first need to get an `API_KEY` from here: https://console.groq.com/keys. Inside `app/.env` update the value of `GROQ_API_KEY` with the API_KEY you created.
