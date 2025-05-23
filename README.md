# 💫 Git & GitHub Survival Guide for Gen Z ✨

yatakatai said i'm pretty

## 🚀 Hai Nashwa & Yattaqi!
Bosen sama tutorial yang kaku? Sama! Makanya kita bikin README yang sefresh mungkin buat kalian yang lagi belajar Git via CMD. No cap, after this you'll be a Git wizard fr fr!

---

## 📱 Quick Links (Tap & Go!)
- [Setup Awal](#-setup-awal-yuk-gas)
- [Basic Commands](#-basic-commands-ezpz)
- [How to Flexing](#-flexing-your-project)
- [Oops Moments](#-oops-moments-damage-control)
- [Collab Time](#-collab-time-squad-goals)

---

## 🔥 Setup Awal, Yuk Gas!

### Install Git dulu dong
```bash
# Download dari https://git-scm.com/downloads
# Cek udah bener belom:
git --version  # Kalo muncul versinya = ✅
```

### Intro yourself ke Git
```bash
# Kasih tau Git siapa dirimu!
git config --global user.name "Si Keren"
git config --global user.email "sikerenbanget@mail.com"

# Cek udah bener?
git config --list  # Harusnya muncul data kamu
```

### Connect ke GitHub
```bash
# Bikin kunci rahasia (SSH Key)
ssh-keygen -t rsa -b 4096 -C "emailmu@example.com"

# Copy SSH key:
# Windows gang:
clip < ~/.ssh/id_rsa.pub
# Mac gang:
pbcopy < ~/.ssh/id_rsa.pub

# Add ke GitHub:
# Settings > SSH and GPG keys > New SSH key > Paste > Save
# Ez pz ✨
```

---

## 👾 Basic Commands (EZPZ)

### Mulai Project
```bash
# Bikin repo baru di folder kosong
git init  # Folder sekarang: 📁 → 📁✨

# Clone repo orang
git clone https://github.com/username/repo.git  # Ctrl+C → Ctrl+V development
```

### Git Flow Harian
```bash
# Cek status (kaya IG story "seen by")
git status

# Add file (like adding friends)
git add index.html    # Add satu file
git add .             # Add semua file (squad goals)

# Commit (like posting to your feed)
git commit -m "✨ Update landing page, tambah efek glitter"

# Push (share to the world)
git push origin main  # Go viral! 🚀
```

### Pull Request Workflow
```bash
# Create & switch to new branch
git switch -c fitur-keren

# Do your magic ✨🧙‍♀️

# Push branch kamu
git push origin fitur-keren

# Buka GitHub → Create PR → wait for the vibes check
```

---

## 🔮 Flexing Your Project

### Remote Control
```bash
# Connect local repo ke GitHub
git remote add origin https://github.com/usernamemu/repo-keren.git

# Liat remote apa aja yang ada
git remote -v

# Upload karya ke GitHub (first time push)
git push -u origin main  # -u = set upstream (default push location)
```

### Abaikan File Ga Penting
Bikin file `.gitignore` dengan isi:
```
# File rahasia jangan di-upload!
rahasia.txt
.env
password.txt

# Folder besar & ga penting
node_modules/
dist/
build/

# Temporary/cache files
.DS_Store
*.log
```

---

## 🆘 Oops Moments (Damage Control)

### Undo-Undo Club
```bash
# "Aduh, gajadi deh" (batal modifikasi)
git restore namafile.js
git restore .  # Batal semua

# "Kecepetan pencet add" (batal staging)
git restore --staged namafile.js

# "Salah commit message" (amend commit terakhir)
git commit --amend -m "Pesan baru yang lebih aesthetic"

# "Mau balik ke commit lama" (travel waktu)
git reset --hard a72f3c2  # Ganti dengan hash commit tujuan
```

### Stash = Simpen Dulu
```bash
# "Bentar, aku mau ngerjain yang lain dulu"
git stash  # Simpan progress

# "Ok, lanjut yang tadi"
git stash pop  # Ambil lagi progress
```

---

## 👯 Collab Time (Squad Goals)

### Branching Strategy
```bash
# Liat branch yang ada
git branch  # Yang ada tanda * = branch aktif

# Bikin & pindah branch baru
git switch -c fitur-login  # -c = create

# Mau balik ke main
git switch main

# Branch ga kepake? Delete!
git branch -d fitur-lama
```

### Merge Your Magic
```bash
# Pindah dulu ke branch tujuan
git switch main

# Gabungin fitur baru ke main
git merge fitur-login

# Kalo conflict = adu design
# Fix conflicts → git add . → git commit
```

### Team Project Flow
```bash
# Update dari repo utama
git pull origin main

# Rebase branch kamu
git switch fitur-kamu
git rebase main

# Push hasil rebase
git push origin fitur-kamu -f  # -f = force push (hati2!)
```

---

## 💅 Pro Tips (No Cap!)

### Shortcuts & Aliases
Setup di `.gitconfig`:
```
[alias]
  s = status
  c = commit
  p = push
  l = log --oneline
  yeet = push origin main -f  # DANGEROUS but funny
```

### Git Log but Make It Fashion
```bash
# Pretty log
git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
# (Pro tip: Make this an alias called 'git pretty')
```

### Git Hooks = Automation
Cek folder `.git/hooks` untuk bikin automation saat git events

---

## 📲 Extra Resources

- [Cheatsheet Git PDF](https://education.github.com/git-cheat-sheet-education.pdf)
- [Oh Shit, Git!?!](https://ohshitgit.com) - For your panic moments
- [GitHub Learning Lab](https://lab.github.com)
- TikTok hashtag: #GitHubTips #CodingTikTok

---

## 👑 Closing Words

Git emang bikin pusing awalnya, tapi trust the process! Kalian bisa banget jadi Git wizards dalam waktu cepat. Jangan takut buat nyoba-nyoba. Kalau error, itu tandanya kalian lagi belajar!

**Remember**: Commit early, commit often, and don't forget to push! ✨

**Nashwa & Yattaqi**: Go build something awesome! 🚀

Press it!
[#Nashwa_Ligma](<Nashwa Cakep.md>)