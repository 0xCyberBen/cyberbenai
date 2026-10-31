# cyberben.ai

> A terminal that boots itself, takes off when asked, and refuses to be hacked. Politely.

This is the source of [cyberben.ai](https://cyberben.ai): one static page, styled as a cockpit terminal, about AI assurance and cybersafety in aviation. Its sibling site is [cybersafety.aero](https://cybersafety.aero).

No framework, no build step, no backend, no cookies, no trackers. Just HTML, CSS, JavaScript and a slightly unreasonable number of `if` statements.

---

## Load sheet

| Item | What it is |
|---|---|
| `index.html` | The whole aircraft. All CSS and JavaScript are inline. |
| `fonts/` | IBM Plex Mono (400, 500) and Space Grotesk (600), self-hosted, with their SIL Open Font Licences. |
| `favicon.*`, `apple-touch-icon.png` | The CyberBen rotor. Ink on light tabs, light on dark tabs. |
| `robots.txt` | Everyone may read the page. The hidden commands stay hidden anyway. |
| `.well-known/security.txt` | Where to report real vulnerabilities (RFC 9116). |
| `.nojekyll` | Tells GitHub Pages to serve `.well-known`. Without it, Jekyll quietly ignores the folder. |
| `CNAME` | `cyberben.ai` |

Total payload: about 100 KB, including fonts. The page makes no requests to other sites. We checked, because that is the job.

---


## For those who dig this deep

You opened the README of a joke terminal. Respect. Here's what the crew would like you to know.

- **There is no AI answering you.** It's `ai@cyberben`, but everything is scripted. Type a full sentence and it will admit this. Honesty is a safety feature.
- **`help` doesn't list everything.** Tab completion won't help either; we made sure. *Pilots tend to find them.*
- **Every investigation starts at the recorder.** Real ones do too. Try `ls` with the flag that shows what's hidden.
- **Some doors only open if you speak tower.** We won't say which door. We will say the alphabet matters.
- **You can't take off with your lights off.** Not in the terminal, and not in real life either. The code is stricter than some airlines.
- **The attack drills only run in flight.** On the ground, systems are cold. Hackers have to wait for take-off like everyone else.
- **If the GPS says you're at 0°N 0°E, you are not.** You are being spoofed. The beaches on Null Island are lovely; the runway does not exist.
- **The flight data recorder survives `clear`.** It does not survive a page reload. Neither would most of us.
- **Space weather is not a cyber attack.** Check the Kp index before you blame the hackers. (Yes, there's a command for that.)
- **The light bar used to hum at 98 Hz.** Engineering asked us to stop. It now glows in silence.
- **A cat checks every file.** A dog checks the cargo hold. One sandwich has been confiscated so far.
- **Water landings are supported.** Life vests inflate on cue. This is why you test your backups.
- **The coffee machine returns HTTP 418.** It has done so since 1998 ([RFC 2324](https://www.rfc-editor.org/rfc/rfc2324)). We see no reason to fix it.
- **There is a challenge coin.** It's still at the mint. Watch this terminal.

### What the page keeps in your browser

No cookies. Three small notes in local storage, which never leave your device:

| Key | Why |
|---|---|
| `cb-theme` | Light or dark, if you chose one. Otherwise the page follows your device. |
| `cb-air-best` | Your best distance in a certain simulator. |
| `cb-coin` | We'll tell you when you've earned it. |

### Accessibility, because it's not optional

The page has keyboard navigation without traps, 44 px tap targets, and 4.5:1 contrast in both themes. Screen readers hear a polite summary instead of every game frame. Under Reduce Motion: no barrel rolls, no blinking, no strobes, everything still works.

---

## Found a real vulnerability?

Not the fake ones we put there on purpose, a real one. Please tell us privately:

- see [`/.well-known/security.txt`](.well-known/security.txt)
- or email **security@cybersafety.aero**, encrypted with our PGP key if it's sensitive.

We don't pay bounties. We do say thank you, and a good report may earn something round and metallic one day.

---

Built in Tallinn · 59°26′N 24°45′E · Cleared for take-off.
© 2026 CyberBen OÜ. Fonts © their authors under the SIL Open Font License 1.1.
