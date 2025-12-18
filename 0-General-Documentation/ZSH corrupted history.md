
```bash
mv ~/.zsh_history ~/.zsh_history_bad
strings ~/.zsh_history_bad > ~/.zsh_history
fc -R ~/.zsh_history
```

**What this does:**

- renames the broken file (backup)
- extracts readable history lines into a new clean file
- reloads it

```bash
mv ~/.zsh_history ~/.zsh_history.backup
touch ~/.zsh_history
```


Reload: 
```bash
fc -R ~/.zsh_history
```

