# 🔁 Update Blowfish Theme (Fork + Submodule) — merox.dev

## 📍 1. Intră în submodul
```bash
cd themes/blowfish
```

## 🔄 2. Fetch + merge din upstream
```bash
git checkout main
git fetch upstream
git merge upstream/main
```

> 🔧 Dacă apar conflicte:
- Editează manual fișierele cu `<<<<<<<`, `=======`, `>>>>>>>`
- După rezolvare:
```bash
git add .
git commit -m "Resolve merge conflicts with upstream"
```

## ⬆️ 3. Trimite update-ul în fork-ul tău
```bash
git push origin main
```

## 🔙 4. Înapoi în root & update submodul
```bash
cd ../..
git add themes/blowfish
git commit -m "Update Blowfish submodule from upstream"
git push
```

---

## ��️ Script alternativ (`update-blowfish.sh`)
```bash
#!/bin/bash
cd themes/blowfish
git checkout main
git fetch upstream
git merge upstream/main
git push origin main
cd ../..
git add themes/blowfish
git commit -m "Update Blowfish submodule from upstream"
git push
```

Rulează cu:
```bash
bash update-blowfish.sh
```

