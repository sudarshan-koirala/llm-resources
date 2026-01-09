# Opencode related stuffs

- [Opencode website](https://opencode.ai/docs/)
- [Oh-my-opencode](https://github.com/code-yeongyu/oh-my-opencode)   


Global Config 👇

```
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "ollama": {
      "npm": "@ai-sdk/openai-compatible",
      "name": "Ollama (local)",
      "options": {
        "baseURL": "http://localhost:11434/v1"
      },
      "models": {
        "llama3.2:latest": {
          "name": "Llama 3"
        }
      }
    }
  },
  "mcp": {
    "agno": {
      "type": "remote",
      "url": "https://docs.agno.com/mcp",
      "enabled": true
    }
  },
   "plugin": [
     "oh-my-opencode"
    ]
}

```
