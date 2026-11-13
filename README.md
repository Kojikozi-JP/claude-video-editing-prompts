# Let Claude Edit Your Phone Videos (No Editing App, No Code)

The 4 prompts from my video: **No Premiere. No DaVinci. Claude Edited My Entire Video.**

You don't edit anything. You paste 4 prompts, look at what Claude makes, and say what you'd like changed. Claude does the editing with Python and ffmpeg on your computer.

Wary of my prompts? Ask an AI in another chat first: "Anything risky in this?" (lol)

**Why the prompts look short:** on the Pro plan you have usage limits. So Claude keeps the storyboard small, makes the rough cuts light (540p), and spends full quality only where it shows: a style sample of the opening and ending, then the final export. Big effects go only on the hook, the best moment and the ending.

---

## ✅ Before you start

1. Install the **Claude desktop app** (Windows or Mac) and sign in on a paid plan (Pro or higher).
2. Make one folder on your computer (for example, `my_video` on the desktop). Copy 3 to 10 phone clips into it. No need to sort or rename them. Move them with a cable, or download them from iCloud Photos or Google Photos.
3. For your first try, aim for a **30-second Short**. It's the quickest and lightest on your usage limit.
4. Download 1 to 3 songs you like from the **Audio Library** in YouTube Studio into the same folder. They're free and safe to use on YouTube. If a song says "attribution required", tell Claude.
5. Open a **new chat** in the Claude app. Paste Prompt 1 and send.
6. Paste Prompts 2 to 4 into the **same chat**, one at a time. Don't start a new chat.
7. Claude will ask "Allow?" a few times. If it's about your clips folder, allow it.

Use the copy button at the top-right of each box below.

---

## 📋 Prompt 1: Setup

**What you'll get:** a list of your files and a 5-second test clip. Usually 5 to 15 minutes.

```text
You're my video editor. Turn my phone clips into a YouTube video with Python and ffmpeg. Aim for the best video you can make, not a quick draft.
Rules: I can't code, so use plain words, go one step at a time and wait for my reply. Save every output in my folder with a version number; never overwrite. Follow the storyboard panel by panel. Never fake, skip or quietly simplify anything; if you can't do something, say so. Check before calling anything done. Save effort: reuse one script, keep ffmpeg output short, check with one small contact sheet, keep replies short.
First: open my folder and list the files, set up Python and ffmpeg (or give me exact steps), tell me your limits, then cut a 5-second test.
```

> 👉 **YOU:** Pick your clips folder and allow access when Claude asks. Installing the free tools can take a few minutes.
>
> When Claude says the 5-second test is saved, open your folder and play it.
> - It plays → paste Prompt 2.
> - It doesn't → tell Claude exactly what you see, like "the file won't open".

---

## 🎬 Prompt 2: Questions, then a storyboard

**What you'll get:** a few questions, then a numbered storyboard. No video yet. Usually 10 to 20 minutes.

```text
Study every clip and song in my folder: length, fps, rotation, HDR, content, camera motion, best moments. Ask what you need in one numbered message with suggested answers: format and length, topic, audience, text language, narration, which song, what must not appear, the feeling it should leave.
Then a storyboard, no editing yet: numbered 3-5 s panels (about 8-10 for 30 seconds) with time, clip, on-screen text, narration, motion, effect, sound, privacy check and a still from the clip. Pick one look first (color, text style, transition) and keep it to the end. Effects are Python-drawn and must point at something in the shot (arrow, circle, self-drawing line, counter, before/after wipe, beat-synced transition); no decoration. Like a pro, use at most 3 big ones, on the hook, the best moment and the ending; keep the rest clean. Hook in the first 3 seconds; end on the most moving shot with one short line that names the moment. Wait for my notes.
```

> 👉 **YOU:** First, answer the numbered questions briefly in your own words.
> Example: "1. Short 2. My dog's first beach trip 3. Family". Not sure? "Use your suggestions" is fine.
>
> Then read the storyboard panel by panel and send changes by number.
> Example: "4: use the clip where he jumps".
> Not sure what to change? Ask "What would you change?"
>
> Happy with it → paste Prompt 3.

---

## ✂️ Prompt 3: Rough cut, fix by panel number

**What you'll get:** a style sample (opening and ending only), then the whole video in light quality. The first rough cut can take 20 to 40 minutes.

```text
Approved. First, a style sample: only the opening and ending panels at full quality; wait for my OK. Then make the whole rough cut at 540p 30fps, with panel number and time top-left.
Beat a phone app's auto-edit: cut on the song's beats, keep every shot moving slightly, one color grade, bold outlined text (2 lines max, clear of Shorts buttons), soft audio at joins, sound from the start. Constant fps, HDR to SDR, frame-accurate cuts, render per panel.
Before showing me, check every panel against the storyboard and review like a picky editor (frames, beats, audio); fix what you find. Show a contact sheet (one frame per panel) and a pass/fail list per rule. I'll give notes by panel number: change only those, and list what you changed.
```

> 👉 **YOU:** Look at the style sample and say what you like and what you don't. Then say OK.
>
> When the rough cut arrives, open it from your folder and watch it to the end. The number in the top-left corner is the storyboard panel. Send notes by number.
> Examples: "2: text too small", "5: end it 1 second earlier", "music too loud", "add an arrow to 4 too".
>
> If it looks cheap or doesn't match the storyboard, send:
> "Compare every panel with the storyboard and fix all differences."
>
> Every fix is saved as a new version, so you can always go back. Expect 2 to 5 rounds.
>
> Love it → paste Prompt 4.

---

## 📤 Prompt 4: Final export

**What you'll get:** the finished video, plus a title, description, thumbnail frame and ideas for next time. Usually 10 to 30 minutes.

```text
Approved. Export the final without panel numbers: 1080p, H.264 CRF 18, BT.709, AAC 320 kbps, -14 LUFS, peaks under -1 dB. Check it and tell me the file name. Then suggest a title, a description (with song credit if required), a thumbnail frame and 3 ideas for my next video.
```

> 👉 **YOU:** Open the finished video from your folder and watch it once.
>
> Upload it with **+** in the YouTube app, or on a computer at studio.youtube.com → **Create** → **Upload videos**.
>
> Just for family? Choose **Unlisted** and send them the link. Grandma can watch it on her phone, no account needed.

---

## 🆘 Stuck?

- **Looks frozen:** rendering takes time. Keep the app open and don't let the computer sleep.
- **Stopped halfway:** send "continue".
- **An error appears:** copy the message and paste it to Claude as is.
- **Hit the usage limit:** wait until it resets, then send "continue". Your files and versions stay in your folder.
- **Want to go back:** say "Go back to version 2 of the rough cut" (or whichever version you liked).
