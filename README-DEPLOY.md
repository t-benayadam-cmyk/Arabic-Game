# 🚀 Put Letter Adventure online (permanent link for your class)

You do NOT need to be a programmer. Follow these 4 steps.
Everything below is free. Total time: about 10 minutes.

---

## Step 0 — Unzip this folder
Unzip `letter-adventure-vercel.zip`. You will get a folder called
`letter-adventure` with the game files inside.

---

## Step 1 — Put the game on GitHub (free file storage)

1. Go to **github.com** → click **Sign up** (if you don't have an account)
2. Click the **+** at the top right → **New repository**
3. Name it: `letter-adventure` → choose **Public** → click **Create repository**
4. On the new page, click the link **"uploading an existing file"**
5. Open your unzipped `letter-adventure` folder, press **Ctrl+A** (select all
   files INSIDE the folder, not the folder itself) and **drag them** into the
   browser
6. Click **Commit changes** and wait for the upload to finish

> ⚠️ Make sure you upload the files INSIDE the folder (package.json,
> src, public, …) — not the zip and not the wrapper folder.

---

## Step 2 — Put the game on Vercel (free hosting = your link)

1. Go to **vercel.com** → click **Sign Up** → choose **Continue with GitHub**
2. Click **Add New… → Project**
3. Find `letter-adventure` in the list → click **Import**
4. Don't change any settings → click **Deploy**
5. Wait 2–3 minutes. You will get a link like:
   `https://letter-adventure-xxxx.vercel.app`

🎉 The game already works at that link! But do Step 3 so the
**class leaderboard** records every student across ALL devices.

---

## Step 3 — Add the free database (for the 🏆 class leaderboard)

1. In your Vercel project page, open the **Storage** tab
2. Click **Create Database** → choose **Neon** (the free one)
3. Name: `leaderboard` → click **Create**
4. When asked **"Connect to project"** → choose `letter-adventure`
   (this adds the database address automatically)
5. When it offers a **Redeploy** → accept it

Done! Now every kid that plays — on any phone, tablet or computer —
is recorded and ranked on the same leaderboard.

---

## ✅ Check it works

1. Open your Vercel link on your phone
2. Create a test player, play a round, earn some coins
3. Tap the **🏆 Leaderboard** button — you should see your player listed
4. Now share the link with your students!

---

## 🔒 Teacher code (deleting players)

- Open the link → **Players** → **🔒 Teacher mode** → your code is **9537**
- Want a different code? Before Step 1, open the file
  `src/lib/admin.ts` in any text editor (Notepad works), change the
  line `const TEACHER_CODE = "9537";` to your own 4 digits, then upload.

---

## ❓ Troubleshooting

| Problem | Fix |
|---|---|
| Vercel build fails | Make sure you uploaded the files INSIDE the folder (see Step 1 warning) |
| Leaderboard shows "can't load" | Database not connected — redo Step 3, then redeploy |
| Lost your link | vercel.com → your project → top of the page shows the URL |
