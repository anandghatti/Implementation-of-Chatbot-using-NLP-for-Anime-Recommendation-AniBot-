# AniBot: Anime Recommendation Chatbot

Welcome to AniBot! This repository contains the code for a chatbot designed to recommend anime and engage in conversations using Natural Language Processing (NLP). Built with Python, Streamlit, and Logistic Regression, AniBot aims to provide a fun and interactive experience for anime enthusiasts.

## Features

- **Anime Recommendations:** Suggests anime based on user input and interests.
- **Intent Recognition:** Uses NLP to classify user inputs into predefined intents.
- **Interactive Web Interface:** Powered by Streamlit for a seamless chat experience.
- **Conversation History:** Logs user-chatbot interactions for review.

## Technologies Used

- **Python Libraries:**
  - `nltk` for natural language processing
  - `sklearn` for machine learning (Logistic Regression and TF-IDF Vectorizer)
  - `streamlit` for the web interface
  - `csv` for saving chat logs
- **Dataset:** Custom JSON file containing intents and responses.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your_username/anibot.git
   cd anibot
   ```

2. **Create a virtual environment and activate it:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download NLTK data:**
   Run the following Python script to download the required NLTK data:
   ```python
   import nltk
   nltk.download('punkt')
   ```

## Usage

1. **Run the chatbot:**
   ```bash
   streamlit run main.py
   ```

2. **Chat with AniBot:**
   Open the Streamlit app in your browser and start chatting. The chatbot will recommend anime or respond to your queries based on its training.

3. **View Conversation History:**
   Access the "Conversation History" menu in the sidebar to review past interactions.

## Project Structure

```
.
├── intents.json            # Dataset of intents and responses
├── main.py                 # Main chatbot script
├── nltk_data/              # NLTK data directory
├── requirements.txt        # List of dependencies
├── README.md               # Project documentation
├── chat_log.csv            # Chat log file (generated at runtime)
```

## Extending the Project

- Add more intents and patterns to `intents.json` to enhance the chatbot's understanding.
- Implement more advanced NLP techniques like deep learning for intent classification.
- Improve the anime recommendation logic using collaborative filtering or content-based filtering.

## Contribution

Contributions are welcome! Feel free to fork this repository and submit a pull request. Please ensure your code adheres to the repository's coding style.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgments

- The anime community for inspiration.
- [Streamlit](https://streamlit.io/) for the fantastic web application framework.
- OpenAI and the NLP research community for making tools and resources accessible to developers.
