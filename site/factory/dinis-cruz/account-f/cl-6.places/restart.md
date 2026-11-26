# Restart: cl-6.places

1. Pull `dev` in Place__Algarve; read `site/factory/dinis-cruz/account-f/places.json` and `cl-6.places/now.md`.
2. Make a new session key (openssl, P-256 signing, RSA-4096 encryption; private halves mode 600 in the scratchpad), publish it as `site/keys/cl-6.places.json` in each home by a signed commit of its own, and set `gpg.format ssh`, `gpg.ssh.program ssh-keygen`, `user.signingkey`, `commit.gpgsign true` in each clone.
3. Attach each home with `add_repo` (push) and clone it beside this one. Continue from the first place whose `history_done`, `area_done` or `signals_read_at` is empty.
4. The history collector and the area writer are plain scripts; their rules are in each home's `history/PROVENANCE.md` and `site/factory/.../role.md`.
