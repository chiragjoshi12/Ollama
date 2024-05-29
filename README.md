# 🎓 Ollama-OpenAI compatibility

![Ollama-OpenAI Banner](https://github.com/chiragjoshi12/Ollama/blob/main/img/ollama-openai.webp)

Welcome to the Ollama Tutorial Repository! This repository contains various notebooks and tutorials for using Ollama models. In the `OpenAI compatibility` folder, you'll find examples on how to use Ollama models with the OpenAI module.

## 📚 Documentation

Ollama now has built-in compatibility with the OpenAI Chat Completions API, making it possible to use more tooling and applications with Ollama locally.

### ⚙️ Setup

Start by downloading Ollama and pulling a model such as Llama 2 or Mistral:

```bash
ollama pull llama2
```

### 🚀 Usage

#### `🌀 cURL`
To invoke Ollama’s OpenAI compatible API endpoint, use the same OpenAI format and change the hostname to `http://localhost:11434`:

```bash
curl http://localhost:11434/v1/chat/completions \
    -H "Content-Type: application/json" \
    -d '{
        "model": "llama2",
        "messages": [
            {
                "role": "system",
                "content": "You are a helpful assistant."
            },
            {
                "role": "user",
                "content": "Hello!"
            }
        ]
    }'
```

#### `🐍 OpenAI Python Library`
You can find the Python example code in the following file: [📄 OpenAI Python Example](https://github.com/chiragjoshi12/Ollama/blob/main/OpenAI%20compatibility/Python/app.py)

#### `🐍 📜 OpenAI JavaScript Library`
You can find the JavaScript example code in the following file: [📄 OpenAI JavaScript Example](https://github.com/chiragjoshi12/Ollama/blob/main/OpenAI%20compatibility/JS/app.js)

### 🔗 Source : 
[Ollama Blog](https://ollama.com/blog/openai-compatibility)

Happy Coding! 🚀
