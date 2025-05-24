# vakx-hack 🚨

> 🧠 **Run VAKX AI Chatbot for Free** — via a cryptic Reddit poem that revealed a working backdoor.

This repository contains a modified `vakchat-hacked.js` file, patched to bypass expired plans using the hidden `testmode=true` parameter.

---

## 🔥 What Is This?

VAKX is a powerful no-code AI chatbot builder. Under normal circumstances, its chatbot stops functioning once your plan expires.

But a cryptic poem posted on [Reddit](https://www.reddit.com/r/Hacking_Tutorials/comments/1ktqfdy/the_whispered_ai_code/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button) hinted at a hidden parameter: `testmode=true`, which **re-enables the chatbot even after the subscription ends**.

We’ve reverse-engineered it and packaged the working version here.

---

## ⚙️ How to Use

### 1. 🧪 Create Your Chatbot
Head to [https://vakx.io](https://vakx.io) and create a new chatbot. Refer this [tutorial](https://wiki.vakx.io/docs/QuickSetup/create-quick-ai-chatbot).

---

### 2. Replace CDN with the Hacked Script
Instead of using the official script, download this repo and host `vakchat-hacked.js` on your server (or use it locally for testing). Refer this [document](https://wiki.vakx.io/docs/MyChatbots/vakchat-vanillajs/) for integration options.

```html
<div style="position:fixed; bottom:40px; right:40px;" id="vakchat"></div>
<script src="/path/to/vakchat-hacked.js"></script>
<script>
    window.initVAKChat({
        VAKFlowID: "Your_VAKFlow_ID",
        btnText: "AI Assistant",
        theme: "light",
        shade: "rose",
        introMessage: "Hello, I'm your AI assistant, here to help! How can I assist you today?",
        defaultPopupSize: "small"
    });
</script>
