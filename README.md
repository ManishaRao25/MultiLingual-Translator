# MultiLingual-Translator
This project is a simple web-based multilingual translator built using Gradio, Transformers, and gTTS (Google Text-to-Speech). It supports translation between English, French, Spanish, German, and Dutch, with the additional feature of generating audio for the translated text.
![Multilingual Translator Output](![Screenshot 2024-09-18 185247](https://github.com/user-attachments/assets/e0e64114-04ec-46ab-b861-2037d218115f)
)


## Features
Text Translation: Translate between five languages:
English ↔ French
English ↔ Spanish
English ↔ German
English ↔ Dutch

Audio Transcription: The translated text is converted to speech using GTTS.
User-Friendly Interface: The app uses Gradio to provide an easy-to-use interface for language translation.
Demo
The interface allows users to enter text, select the source and target languages, and get both the translated text and audio version of the translation.

## Libraries Used
- Gradio: To create the user interface for interacting with the translator.
- Transformers (Hugging Face): For loading pre-trained translation models from Helsinki-NLP.
- gTTS: To convert translated text into speech.

#### Setup Instructions
1. **Clone the Repository**  ```python  git clone https://github.com/your-username/multilingual-translator.git
cd multilingual-translator

2.  **Install Required Libraries**
Ensure you have the following dependencies installed. You can install them using pip:  ```python pip install gradio transformers torch gtts

3. **Running the Application**
You can run the translator locally with the following command:  ```python  python app.py

4. **Using the Translator**
**Input:** Enter the text you wish to translate.
**Select Source and Target Languages:** Choose the languages from the dropdown menu.
**Output:** You will get the translated text and an audio version of the translation.

## Code Explanation
The key function of this app is translate_text(), which:

- Loads the appropriate translation model based on the selected language pair.
- Translates the input text using the pre-trained model.
- Uses gTTS to generate an audio file from the translated text.
- Returns both the translated text and the path to the audio file.
- The Gradio interface is then used to make this functionality accessible via a web-based app.

## Example Usage
You can use the translator to convert text between languages. For instance, translating "Hello" from English to French will return "Bonjour" along with an audio file that pronounces "Bonjour."

## Supported Language Pairs
English ↔ French
English ↔ Spanish
English ↔ German
English ↔ Dutch

## Contribution
If you'd like to contribute:

## Fork the repository.
Create a new branch for your feature or bug fix.

## Submit a pull request with your changes.

## License
This project is licensed under the MIT License.



