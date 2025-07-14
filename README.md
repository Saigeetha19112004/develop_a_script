# Reddit User Persona Generator

This project scrapes a Reddit user's comments and posts using the Reddit API (PRAW) and generates a basic user persona based on the content. The generated persona is saved to a text file, including citations linking back to the source data.

## Features

*   Scrapes comments and posts from a specified Reddit user.
*   Performs basic Natural Language Processing (NLP) to clean and process the text data.
*   Analyzes word and bigram frequencies to identify potential user interests and common topics.
*   Generates a basic user persona based on the analysis.
*   Outputs the user persona and basic citations to a text file.

## Prerequisites

Before running the script, we need to have the following installed:

*   Python 3.6 or higher
*   Required Python libraries (listed below)
*   A Reddit API application and credentials (Client ID and Client Secret)

## Setup
* Install Required Libraries:
  * praw, nltk, spacy
  * download en_core_web_sm
* Set up Reddit API Credentials:
* We need to create a Reddit API application to get the Client ID and Client Secret. Follow these steps
    * Go to the Reddit applications page: https://www.reddit.com/prefs/apps
    * Scroll down and click on "create app" or "create another app".
    * Fill in the details:
      * name: Choose a name for your app.
      * type: Select "script".
    * redirect url: Enter http://localhost:8080.
    * Click "create app".
      * Your Client ID and Client Secret will be displayed.
      * It is highly recommended to set your Client ID and Client Secret as environment variables to keep them secure and avoid hardcoding them in your script.
* Place your script:
    * Python script (generate_persona.py or whatever you named it) is in the project directory.
