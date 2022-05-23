### Get Started
Include the library in your `.html` file
```JS
<script src="https://zhiftydk.github.io/chatbot/chatbot.js"></script>
```

### How to use
Example: How to train upon your intents
```JS
const bot = new chatBot();
bot.train();
```

Example: How to run your model after training
```JS
const bot = new chatBot();
bot.run();
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
