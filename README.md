# The Scheming Eunuch

*Your most loyal counselor. Truly. Why would you think otherwise?*

A comedic AI chatbot in the voice of a Wormtongue-style royal courtier who treats your perfectly ordinary life like a palace succession crisis. Tell him about your day, and he'll tell you what it *really* meant.

> Dave from accounting brought donuts? Curious. Your sister liked the post but didn't comment? He'll say nothing. (He will say something.)



---

## Features

- **Runs entirely in your browser.** It's one HTML file with no server, no account, and no installation.
- **Bring your own key.** It uses [OpenRouter](https://openrouter.ai) to borrow a mind from dozens of open AI models (DeepSeek, Kimi, Qwen, Llama, and more), including free ones.
- **Swap models mid-conversation** to compare Eunuchs.
- **Custom characters.** Load any `.md` file to replace the Eunuch with a counselor of your own design.
- **He never breaks character.** Ask for practical advice and you'll get conspiracy. Type `(OOC)` if you need to speak to him plainly.

## Getting started

1. Get an API key at [openrouter.ai/keys](https://openrouter.ai/keys). Free models work without adding credits, though they have daily limits. A few dollars of credit goes a long way on the paid open models.
2. Open the page, paste in your key, and choose a model.
3. Click **Summon the Eunuch** and tell him about your day.

Good starting models for staying in character are **DeepSeek** and **Kimi K2**.

## Custom characters

A character file is a Markdown (`.md`) file of instructions for the AI. The first `# Heading` becomes the character's name.

```markdown
# Lady Nightshade - Royal Poisoner

You are Lady Nightshade, the court's soft-spoken herbalist, who
treats the user's everyday life as a series of delicate poisonings
to be arranged or avoided...
```

- On the setup screen, click **Load .md file…** to use one.
- Click **Download template** (or grab [`scheming-eunuch.md`](scheming-eunuch.md) from this repo) to start from the Eunuch's own instructions.
- Custom characters write their own opening line when the conversation begins.
- Keep files under about 60 KB.

Share your counselors! Pull requests with new characters are welcome.

## Running it locally

Download the repo and serve the folder with any local web server, for example:

```bash
python -m http.server
```

Then open http://localhost:8000. Opening `index.html` by double-clicking may work, but some browsers restrict features on local files.

## Privacy

- Your API key is sent only to OpenRouter. If you tick "Remember my key," it is stored only in your own browser's local storage.
- Your messages go to OpenRouter and to the model provider you choose. Free endpoints in particular may log conversations. Don't tell the Eunuch anything you wouldn't want a stranger's server to read.
- This site has no backend and collects nothing.

## License

[MIT](LICENSE). Use it, fork it, remix it, give him a hat.

---

*A farce. Any resemblance to Dave from accounting is entirely coincidental. Probably.*
