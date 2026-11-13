# Let Claude Edit Your Phone Videos (No Editing App, No Code)

The 4 prompts from my video: **No Premiere. No DaVinci. Claude Edited My Entire Video.**

Paste them into the Claude desktop app one at a time, in the same chat. Use the copy button at the top-right of each box.

Wary of my prompts? Ask an AI in another chat first: "Anything risky in this?" (lol)

## ✅ Before you start

1. Get the Claude desktop app (Windows or Mac) on a paid plan (Pro or higher).
2. Copy 3 to 10 phone clips into a new folder on your computer (cable, iCloud Photos or Google Photos). Start with a 30-second Short.
3. Add 1 to 3 songs to the same folder from YouTube Studio's Audio Library (free, YouTube-safe). If one says attribution required, tell Claude.
4. Open a new chat in the Claude app, paste Prompt 1 and send.
5. Paste Prompts 2 to 4 into the same chat, not a new one.
6. Allow Claude's permission requests about your clips folder.

## 📋 Prompt 1: Setup

```text
You're my video editor. Turn my phone clips into a YouTube video with Python and ffmpeg. Aim for the best video you can make, not a quick draft.
Rules: I can't code, so use plain words, go one step at a time and wait for my reply. Save every output in my folder with a version number; never overwrite. Follow the storyboard panel by panel. Never fake, skip or quietly simplify anything; if you can't do something, say so. Check before calling anything done. Save effort: reuse one script, keep ffmpeg output short, check with one small contact sheet, keep replies short.
First: open my folder and list the files, set up Python and ffmpeg (or give me exact steps), tell me your limits, then cut a 5-second test.
```

> 👉 YOU: Allow folder access when asked. Play the 5-second test from your folder. Works? Paste Prompt 2. If not, tell Claude what you see.

## 🎬 Prompt 2: Check the clips, storyboard first

```text
Study every clip and song in my folder: length, fps, rotation, HDR, content, camera motion, best moments. Ask what you need in one numbered message with suggested answers: format and length, topic, audience, text language, narration, which song, what must not appear, the feeling it should leave.
Then a storyboard, no editing yet: numbered 3-5 s panels with time, clip, on-screen text, narration, motion, effect, sound, privacy check and a still from the clip. Effects are Python-drawn (arrow, circle, self-drawing line, counter, before/after wipe, beat-synced transition). Like a pro, save the big ones for the hook, the best moment and the ending so they hit harder; keep the rest clean. Each should guide the eye. Hook in the first 3 seconds; end on the most moving shot with one short line that names the moment. Wait for my notes.
```

> 👉 YOU: Answer the numbered questions ("1. Short 2. My dog's first beach trip") or say "use your suggestions". Check the storyboard and fix by number ("4: use the clip where he jumps"). Stuck? Ask "What would you change?" Happy? Paste Prompt 3.

## ✂️ Prompt 3: Rough cut, fix by panel number

```text
Approved. First, a style sample: only the opening and ending panels at full quality; wait for my OK. Then make the whole rough cut at 540p 30fps, with panel number and time top-left.
Beat a phone app's auto-edit: cut on the song's beats, keep every shot moving slightly, one color grade, bold outlined text (2 lines max, clear of Shorts buttons), soft audio at joins, sound from the start. Constant fps, HDR to SDR, frame-accurate cuts, render per panel.
Before showing me, check every panel against the storyboard and review like a picky editor (frames, beats, audio); fix what you find. Show a contact sheet (one frame per panel) and a pass/fail list per rule. I'll give notes by panel number: change only those, and list what you changed.
```

> 👉 YOU: React to the style sample, then the rough cut; the top-left number is the panel. Send notes by number ("2: text too small", "music too loud"). Want more effects? Ask by panel number. Looks cheap or off the storyboard? Send: "Compare every panel with the storyboard and fix all differences." Expect 2 to 5 rounds. Love it? Paste Prompt 4.

## 📤 Prompt 4: Final export

```text
Approved. Export the final without panel numbers: 1080p, H.264 CRF 18, BT.709, AAC 320 kbps, -14 LUFS, peaks under -1 dB. Check it and tell me the file name. Then suggest a title, a description (with song credit if required), a thumbnail frame and 3 ideas for my next video.
```

> 👉 YOU: Upload in the YouTube app (+) or at studio.youtube.com. Just for family? Choose Unlisted and send the link.

## 🆘 Stuck?

Frozen? Keep the app open and the PC awake. Stopped halfway: type "continue". Error: paste it to Claude. Usage limit: wait, then "continue".
