# Mindscript 

The Mindscript library provides an AI-based, lightweight solution for creating chatbot-like interactions. It's designed to be easy to train, making it a great choice for various conversational applications.

## Installation

Install the `mindscript` library using npm:

```bash
npm install mindscript
```

## Usage

1. Create a model JSON file with questions and responses. For example, `model.json`:

```json
[
  {
    "id": 1,
    "question": ["hi"],
    "response": ["Hello!"]
  },
  {
    "id": 2,
    "question": ["how", "are", "you"],
    "response": ["I'm fine, thank you!"]
  }
]
```

2. Use the `Mind` class from the library to generate responses:

```javascript
const Mind = require('mindscript');
const mind = new Mind('./path-to-your-model/model.json');

let input = 'Hi';
console.log(mind.think(input)); // Output: "Hello!"
```

## Benefits

- AI-Based: Leverage AI-powered interactions for your applications.
- Easy Training: Create models quickly and efficiently with predefined questions and responses.
- Lightweight: Built using native Node.js, the library doesn't require excessive resources.
- Customizable: Tailor the models to suit your specific needs and conversations.

