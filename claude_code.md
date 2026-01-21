# This file holds information related to Claude Code

Claude Code from Anthropic -> https://anthropic.skilljar.com/claude-code-in-action

---
## Claude Code with Ollama (Run Claude Code for Free)
- [Ollama Anthropic Compatibility](https://docs.ollama.com/api/anthropic-compatibility)
- [Claude Code Integration](https://docs.ollama.com/integrations/claude-code)

----
### Installation in macOS
```
# Install Ollama
brew install ollama

OR download from website
https://ollama.com/download/mac

ollama --version
curl http://localhost:11434

ollama list
ollama run qwen3-coder:30b
ollama run qwen3-vl:2b # https://ollama.com/library/qwen3-vl


---

# Install Claude Code
curl -fsSL https://claude.ai/install.sh | bash
export ANTHROPIC_AUTH_TOKEN=ollama

export ANTHROPIC_BASE_URL=http://localhost:11434
claude --model qwen3-coder:30b
claude --model qwen3-vl:2b

OR run with env variables inline
ANTHROPIC_AUTH_TOKEN=ollama ANTHROPIC_BASE_URL=http://localhost:11434 claude --model qwen3-coder:30b
```

**Switching back to Claude API if you intend to use**
```
unset ANTHROPIC_BASE_URL
unset ANTHROPIC_AUTH_TOKEN

```

Happy Coding 😎
