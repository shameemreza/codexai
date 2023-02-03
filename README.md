# Codex AI
ChatGPT and OpenAI integration using JavaScript


## How to configure


### OpenAI API configuration

Create a `.env' inside the server folder add OpenAI API like below:

```
OPENAI_API_KEY = "Paste your API keys here"
```

Run the server using this command to get the server URL:

```
npm run server
```

Now, open `script.js` from client folder and change the server keys (Line: 83):

```
const response = await fetch('Add your server URL here', {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json'
    },
    body: JSON.stringify({
      prompt: data.get('prompt')
    })
  })
```

Now run the clinet using this command:

```
npm run dev
```


### Deply on Live

* Go to `https://render.com` and add your repositer as the public source. Add server folder and your OpenAI API key as the environment variable. Once the deployment complete, copy the URL and use it as the server URL.

* Go to `https://vercel.com` and add the client to deploy the front end. Make sure to change the server URL to work it like a charm.

