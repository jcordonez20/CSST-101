# AI Chatbot Project Setup Guide

If you encounter an error like "API key not valid. Please pass a valid API key." while using the Chatbot, follow these steps:

## Get Your free API Key

1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey).
2. Navigate to the API key section and create a new API key. It's free!

Your API key will look something like this: AIzaSyAtpnKGX13bTgmx0l_gQeatYvdWvY_wOTQ

## Insert Your API Key

1. Open your project folder in VS Code.
2. Navigate to the `script.js` file.
3. Find the `API_KEY` variable and replace `PASTE-YOUR-API-KEY` with your actual API key.

## Save and Test

1. Save the `script.js` file after adding your API key.
2. Open `index.html` in your browser to verify that Chatbot is working correctly.

## Important Information

This chatbot uses the Gemini beta model, gemini-1.5-flash, which allows more free requests within a shorter timeframe. If you need greater reliability, you can switch to the stable model, gemini-1.5-pro. While the free version of this model has stricter request limits, upgrading to a paid plan will remove these restrictions.

To switch to the gemini-1.5-pro stable model, update the API_URL in the `script.js` file as follows:
const API_URL = `https://generativelanguage.googleapis.com/v1/models/gemini-1.5-pro:generateContent?key=${API_KEY}`;

## Customization Tips

This chatbot uses the free Gemini API to generate responses to any questions. You can customize it by adding your company information, and the chatbot will respond accordingly.

Simply update line 24 of `script.js` file with the following code:

```javascript
const chatHistory = [
  {
    role: "model",
    parts: [{ text: `Your company information here` }],
  },
];
```

If you still get an error or get stuck, feel free to message me on Buy Me a Coffee.
https://buymeacoffee.com/codingnepal

---

Happy coding!
