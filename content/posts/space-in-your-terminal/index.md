---
draft: true
---

# Tabula rasa

Here's a neat custom command for **zsh** for adding some space to your terminal without losing history by running `clear`.

## Add function to `~./zshrc`

```bash
function space() {
    local lines
    lines=$(tput lines)  # Get the number of lines in the terminal
    printf "\n%.0s" $(seq 1 $lines)  # Print newlines equivalent to the terminal height
}
```

## Reload Zsh

Run `source ~/.zshrc`

## Test it out

Type `space` in your terminal and enjoy a fresh workspace!
But fear not, your history is just a scroll away.