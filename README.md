# Blocky: Empowering Creators and Enhancing AI – Ethically
Blocky connects AI companies with artists for ethical AI training & fine-tuning, ensuring fair compensation and redefining digital creativity fairness.

Demo:  https://www.youtube.com/watch?v=RTPljR0zBP0

# Inspiration
Blocky was inspired by the growing need to address ethical issues in AI development, particularly around the use and compensation of creative content. AI companies often scrape the internet for any data they can get their hands on without properly licensing or compensating the creators. OpenAI and Anthropic are currently facing lawsuits for this. AI models are getting incredibly competent at generating art or music in an artist's style, due to being trained on their work. However, it’s becoming an increasingly prevalent issue where the original creators are not being compensated.

# What it does
Blocky serves as a bridge for organizations that aim to ethically train machine learning models that generate creative outputs. By connecting these organizations directly with artists willing to provide their work in exchange for fair compensation, Blocky not only streamlines the model training process but also fosters a fairer environment for artists.

# How we built it
Blocky is an AI-powered platform that links Data Seekers, the AI companies, with Data Providers, the artists and creators.

Here’s how it works: A Data Seeker registers an account on Blocky and details the type of data they need. We fine-tuned the BLOOM-3b language model to extract keywords from this description. These terms are then matched with the keywords listed in the profiles of the Data Providers using cosine similarity, ensuring precise pairings.

Data Seekers can then select their ideal Provider and specify the amount of data required. The transaction is facilitated through a Google Gemini-powered Agent, acting on behalf of the Data Provider. The Agent drafts an Ethereum smart contract to formalize the agreement in real time.

Our matching algorithms and database are designed to efficiently handle a worldwide user base. Additionally, since we do not directly host datasets, our scalability is further enhanced, allowing us to grow without the typical constraints of data storage.

# Challenges we ran into
- Going through multiple iterations of fine-tuning language models to properly extract keywords from the Data Seeker input and then devising a way to match Data Seekers and Providers using keywords.
- Iterated multiple backend servers (FastAPI, Flask).
- Multiple attempts at building an Agent. First, tried to use Fetch.ai's tools, but ultimately used Google Gemini. Also, had difficulties prompting the Gemini Agent to properly interact with the user and create the Ethereum smart contract.

# Accomplishments that we're proud of
- Creating a functioning, full-stack app!
- Aligning our inner motivations to create an ethical project with the potential to better society!
- Successful integration of machine learning for matching.
- Successful implementation of Gemini-powered Agent.

# What we learned
- Complexities of fine-tuning, prompt-engineering, and natural language processing.
- Google AI Studio proficiency (in a few hours!)
- The needs of both artists and AI companies.

# What's next for Blocky
The future of Blocky involves expanding our user base and dataset offerings, enhancing our matching algorithms, and properly deploying our Ethereum smart contracts on the blockchain. Ultimately, we aim to establish Blocky as the standard for ethical AI data sourcing worldwide.

# Tech Stack:
- Flask and Flutter for backend.
- Firebase for database.
- BLOOM-3b, Google Gemini 1.5 Pro, FastText, Google Colab, Python for Machine Learning.

# Team Blocky: Tomasz Jezak, Alex Plashchinsky, Emre Turan
![image](https://github.com/tomaszjezak/Blocky/assets/113561444/fae5a96b-5ce8-478c-97a2-c33996e82795)

### Presented at LA Hacks 2024 to 10 judges!
