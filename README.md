# sops demo

shows a minimal example of how secrets could be managed between a team in git

- `apps/age-demo` shows the basics of age to encrypt / decrypt files
- `apps/sops-demo` uses age to encrypt / decrypt secrets in a git friendly way

### notes on sops

- sops looks for age private keys in `~/Library/Application Support/sops/age/keys.txt`
- key helper:
  ```
  mkdir -p ~/Library/Application\ Support/sops/age
  vim ~/Library/Application\ Support/sops/age/keys.txt
  ```

- `.sops.yaml` is at the repo root is used even while in `apps/` subdirectories
