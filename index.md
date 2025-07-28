---
class:
    - invert
---

# AI Development Tools

For use with Terminal and (Neo)Vim

---

## 🤖 Copilot CLI

by Paulo Diovani


[github.com/cli](https://github.com/cli/cli#installation)
[docs.github.com/.../install-copilot-in-the-cli](https://docs.github.com/en/copilot/how-tos/set-up/install-copilot-in-the-cli)

---

Installation:

```bash
gh auth login
gh extension install github/gh-copilot
```

Usage:

```bash
gh copilot explain "sudo apt-get"
gh copilot suggest "Undo the last commit"
```

---

Suggestion: Create an `alias`

```bash
copilot () {
    gh copilot suggest --target shell "\"$@\""
}
```

Usage:

```bash
gh copilot suggest "Undo the last commit"
```

---

## 🤖 Claude Code

by Alexandre Camillo

[anthropic.com/claude-code](https://www.anthropic.com/claude-code)

---

## 🤖 Open Code

by Marcelo Alexandre

[opencode.ai](https://opencode.ai/)

---

## 🤖 Aider

by Paulo Diovani

[aider.chat](https://aider.chat/)

---

Intallation:

```bash
python -m pip install aider-install
aider-install
```

Usage:

```bash
# Change directory into your codebase
cd /to/your/project

# DeepSeek
aider --model deepseek --api-key deepseek=<key>

# Claude 3.7 Sonnet
aider --model sonnet --api-key anthropic=<key>

# o3-mini
aider --model o3-mini --api-key openai=<key>
```

---

Configuration (`~/.aider.conf.yml`):

```yml
## Use colors suitable for a dark terminal background (default: False)
dark-mode: false

## Set coding theme
code-theme: one-dark

## Enable/disable looking for a git repo (default: True)
git: false
## Do not make git commits
auto-commits: false
```

---

Config with env vars:

[aider.chat/docs/config/dotenv.html](https://aider.chat/docs/config/dotenv.html)

```bash
# Open Router API Key
export OPENROUTER_API_KEY=<YOUR API KEY>

# OpenAI Key for Open Router
export OPENAI_API_BASE=https://openrouter.ai/api/v1
export OPENAI_API_KEY="$OPENROUTER_API_KEY"
```

---

# Vim and Neovim plugins

---

## 🤖 Copilot / Copilot.lua

by Alexandre Saura, Márcio Flávio, and Paulo Diovani

[github/copilot.vim](https://github.com/github/copilot.vim)
[zbirenbaum/copilot.lua](https://github.com/zbirenbaum/copilot.lua)

---

## 🤖 CodeCompanion

by Márcio Flávio, and Paulo Diovani

[codecompanion.olimorris.dev](https://codecompanion.olimorris.dev/)

---

Other Vim/Neovim plugins

- [copilotc-nvim.github.io/CopilotChat.nvim](https://copilotc-nvim.github.io/CopilotChat.nvim)
- [DanBradbury/copilot-chat.vim](https://github.com/DanBradbury/copilot-chat.vim)
- [yetone/avante.nvim](https://github.com/yetone/avante.nvim)

---

The End!
