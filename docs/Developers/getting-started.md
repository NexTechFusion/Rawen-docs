---
sidebar_position: 1
---

# Getting Started 🚀

## Prepare your environment
Download and install the latest version of Rawen (Apply to whitelist [here](https://rawen.io)).

## Create your first command 

We will create a simple command that will exectue a simply open the app and display "Hello world".

### Variant 1: Inbound IDE

1. Open the Rawen app.
2. Route to "Settings" and the "Commands" tab and hit the "Add" button
3. Add a new Action and select "Client Code"
4. Now copy this code into the editor:

```javascript
await openApp();
await addResult("Hello world!");
```
5. Hit the "Debug" button

### Variant 2: SDK

1. Clone the Command Maker repository from [here](https://gihub.com/rawen-io/command-maker)
2. Open project and paste in the same code as above into the `index.ts`.
3. Run the project by typing `npm run start` in the terminal.





