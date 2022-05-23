##Chatbot.js the neural network javascript library

### Get Started
Include the library in your `.html` file
```JS
<script src="//zhiftydk.github.io/chatbot/chatbot.js"></script>
```

### How to use
Example: How to train your neural network from intents
```JS
const bot = new chatBot("./intents.js");
bot.train();
```

Example: How to train your neural network from new intents untop of your current model
```JS
const bot = new chatBot("./intents.js", "./model.js");
bot.train(); // When training is done model.json file will be downloaded
```

Example: How to run your model after training
```JS
const bot = new chatBot("./intents.js", "./model.js");
bot.run("How are you?"); // Greeting response sentence
```

Create `intents.json` file and format the intents like this:
```JSON
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
  ]
}
```
