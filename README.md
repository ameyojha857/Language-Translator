# Language-Translator
A language Translation app that auto detects the input language and converts it to desired output.
GUI Development with Tkinter:
The project uses the Tkinter library to create a user-friendly GUI. It consists of various frames and widgets:

Input Frame: This frame contains a label instructing the user to enter text and a text input field where users can input the text they want to translate.

Output Frame: This frame displays the translated text once the user clicks the "Translate" button. It also contains a label to indicate that the displayed text is the translated output.

Controls Frame: This frame contains several widgets for controlling the translation process:

Language Selection: A Combobox widget allows users to select the source language for translation (e.g., English).
Multi-Language Selection: An Entry widget lets users specify the target languages for translation. They can enter multiple languages separated by commas (e.g., "es,fr,de").
Auto-Detect Button: A button labeled "Auto-Detect Language" automatically detects the source language of the input text.
Translate Button: Clicking this button triggers the translation process.
Text-to-Speech Button: Clicking this button converts the translated text into speech.
History Frame: This frame displays a history of translations. It includes a label indicating "Translation History" and a text box that shows the source text, target languages, and translated text for each translation.

Translation Functionality:
The code uses the "googletrans" library to provide translation functionality. Here's how it works:

Users input text into the text field.
They can select a source language from the Combobox or use the "Auto-Detect Language" button to detect it automatically.
Users specify one or more target languages in the Entry field, separated by commas.
Clicking the "Translate" button initiates the translation process.
The code translates the input text into each of the specified target languages and displays the translations in the output frame.
It also appends the translations to the translation history in the history frame.
Text-to-Speech Functionality:
The project utilizes the "pyttsx3" library to enable text-to-speech conversion:

After translation, users can click the "Text to Speech" button.
The code uses the "pyttsx3" library to convert the translated text into speech.
Users can listen to the translated text as audio output.
Error Handling and User Feedback:
The code includes error handling for potential issues, such as API errors during translation requests or text-to-speech conversion failures. When errors occur, appropriate error messages are displayed to the user.

Language Support:
It supports multiple languages for translation, including English, Spanish, French, German, Japanese, Chinese (Simplified), Russian, Arabic, Hindi, Korean, Italian, and more. You can extend the language support by adding additional languages to the supported_languages dictionary in the code.

Overall, this project provides a user-friendly interface for translating text into multiple languages and even experiencing the translations through text-to-speech conversion. 
