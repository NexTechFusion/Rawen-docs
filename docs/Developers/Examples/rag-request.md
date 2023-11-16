---
sidebar_position: 1
---

# RAG request

Basic RAG request with the Inbound IDE and the SDK.

## Inbound IDE

1. Open the Rawen app.
2. Route to "Settings" and the "Commands" tab and hit the "Add" button
3. Add a new Action and select "LLM-Doc-Request"
4. Add a new Action and select "LLm-Request"
5. Adjust the Prompt
(![image](https://user-images.githubusercontent.com/9094011/137638885-2b6b8b0a-0b0b-4b0a-8b0a-0b0a0b0a0b0a.png))
6. Save and hit the "Debug" button

## SDK

1. Clone the Command Maker repository from [here](https://gihub.com/rawen-io/command-maker)
2. Open project and paste in the same code as above into the `index.ts`.

```javascript
const docs = await callKnowledge("What?", {
    key: "MY_OPENAI_KEY",
    type: "OPENAI"
});
const response = await callRag("What?", {
    key: "MY_OPENAI_KEY",
    type: "OPENAI"
});
await addResult(response);
```
3. Run the project by typing `npm run start` in the terminal.