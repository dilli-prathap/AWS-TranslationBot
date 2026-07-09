
# Language Translation Bot using Amazon Lex, AWS Lambda & Amazon Translate

A serverless chatbot that translates user-provided text into different languages using Amazon Lex, AWS Lambda, and Amazon Translate.

## Project Overview

This project allows users to:

- Enter a sentence.
- Select a target language.
- Receive the translated text.

The chatbot is powered by Amazon Lex and invokes an AWS Lambda function, which calls Amazon Translate to perform the translation.

---

## Architecture

<img width="1630" height="711" alt="521269186-af219e6b-0850-4582-b8d1-f4228d608be9" src="https://github.com/user-attachments/assets/2ac1bc50-3383-4624-8c0f-94af729e44fd" />


---

## AWS Services Used

- Amazon Lex V2
- AWS Lambda (Python)
- Amazon Translate
- IAM

---

## Features

- Translate text into multiple languages
- Supports:
  - Spanish
  - French
  - German
  - Japanese
  - Chinese
- Serverless architecture
- Automatic intent fulfillment

---

## Lambda Function Workflow

1. Receive user input from Amazon Lex.
2. Extract:
   - Text to translate
   - Target language
3. Map the selected language to its language code.
4. Invoke Amazon Translate.
5. Return the translated text back to Lex.

---

## Example

Input:

```
Text: Hello, how are you?
Language: French
```

Output:

```
Bonjour, comment allez-vous ?
```

---

## Output:
<img width="1498" height="933" alt="Screenshot 2026-07-09 143942" src="https://github.com/user-attachments/assets/b693b629-5be7-4534-8a81-bf870053a13d" />



## Technologies

- Python 3.x
- boto3
- Amazon Lex V2
- Amazon Translate
- AWS Lambda

---

## How to Run

1. Create an Amazon Lex V2 bot.
2. Create the required slots:
   - text
   - language
3. Create an AWS Lambda function.
4. Paste the Python code into the Lambda editor.
5. Attach permissions to access Amazon Translate.
6. Connect the Lambda function to the Lex intent.
7. Build the bot.
8. Test translations.

---

## Learning Outcomes

- Building serverless applications
- Creating conversational bots using Amazon Lex
- Integrating AWS Lambda with Lex
- Using Amazon Translate API
- Managing IAM permissions

---

