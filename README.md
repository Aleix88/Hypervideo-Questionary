# Hypervideo-SimpleLabel
Questionary plugin for [Hypervideos.js](https://github.com/Aleix88/Hypervideos)
<div>
    <img src="https://github.com/Aleix88/Hypervideo-Questionary/blob/main/questionary.png?raw=true">
</div>

## Features
- Display a questionary with one correct answer.
- Customize the question, description and all the answers.
- Random answers order.

## Installation
### Manual downloading
1. Download the Questionary.js file.
2. Import this file in your html.

## Usage
Add this plugin to the hypervideo configuration object with the text paràmeter on config:

    const config = {
        ...

        "tags": [
          {
            ...

            "plugin": {
                "name": "Questionary",
                "config": {
                    "title": "Your question",
                    "subtitle": "Your description text",
                    "correctAnswer": "The correct answer",
                    "wrongAnswers": [
                      "Incorrect answer 1",
                      "Incorrecta answer 2", 
                      ...
                    ]
                }
            }

          }, 
          ...
        ]
      };

## Config params

| Field | Type | Description |
| ------------- | ------------- | ------------- |
| title | string | Question text to display |
| subtitle | string | Question subtitle or description to display |
| correctAnswer | string | The correct answer text |
| wrongAnswers | array of strings | The multiple wrong answers |