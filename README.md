# Project Setup Guide

Welcome to my GitHub for Rotation Project 2: New Target Proposal (NTP) Generation Using Agentic LLMs. Here you'll find a set of projects that work seperately, each providing unique features.

Reflexion.ipynb: implements langchain's version of Reflexion with PubMed API - this version brings back full text.
RATT_Embedded_V2: Uses the embedded articles + RAG to generate its answers 
RATT_PQA: Uses RATT + Pubmed-API to PaperQA (Not PaperQA2 although can be updated)

Assesment_Agent: A simple assessment agent workflow using AutoGen to assess results of the generated NTPs.

The original code for RATT can be found here: https://github.com/jinghanzhang1998/RATT
and for Langchains version of Reflexion: https://github.com/langchain-ai/langgraph/blob/main/examples/reflexion/reflexion.ipynb
and PaperQA: https://github.com/Future-House/paper-qa

You can find results of the generated NTPs for each of the algorithms alongisde the prompts used in the Results folder.

Follow the steps below to set up your environment and start using the projects.

## Prerequisites

- Ensure you have [Anaconda](https://www.anaconda.com/products/distribution) installed to create and manage environments.
- You will need Python version **3.12.4**.
- The projects make use of **OpenAI** and **Langchain** APIs, so please make sure you have access to these keys.

## Setup Instructions

1. **Clone the Repository**
   ```sh
   git clone <your-repository-url>
   cd <repository-folder>
   ```

2. **Create the Conda Environment**
   Create a new Conda environment with Python 3.12.4:
   ```sh
   conda create -n my_env_name python=3.12.4
   conda activate my_env_name
   ```

3. **Install Dependencies**
   Use `pip` to install the dependencies listed in the `requirements.txt` file:
   ```sh
   pip install -r requirements.txt
   ```

4. **Setup the Environment Variables**
   You will need to create a `.env` file in the root directory of your project. Add your API keys as follows:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   LANGCHAIN_API_KEY=your_langchain_api_key_here  # Required if you plan to use reflexion.ipynb
   ```

5. **Running the Projects**
   - Simply navigate to the project of interest and run the relevant scripts.
   - For using **reflexion.ipynb**, ensure your `.env` is properly configured with both the **OpenAI** and **Langchain** API keys.

## Notes
- If you only plan to use projects other than `reflexion.ipynb`, you can skip adding the `LANGCHAIN_API_KEY`.
- Each project has its own detailed instructions on usage, available in its respective folder.

## Feedback
If you encounter any issues or have suggestions, feel free to open an issue in the repository. Contributions are always welcome!

