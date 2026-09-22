# A list of some of my projects

Each project has two ratings, scored between 0 and 10 (10 being the most difficult):

- **Use** — how much effort it takes to try it out. Most apps you can just click the link and use without creating an account.
- **Size** — how big the app is. E.g. a single page app hosted on GitHub Pages with no server is a 0, but something that needs a server, DNS config etc. is higher.

## <img src="https://www.remote-desktop.co/favicon.svg" alt="App Icon" height="25px"> Remote Desktop

![No account](https://img.shields.io/badge/no%20account-blue) ![Windows](https://img.shields.io/badge/windows-blue) ![Android](https://img.shields.io/badge/android-blue) ![End to end encrypted](https://img.shields.io/badge/end%20to%20end%20encrypted-blue) ![Self hostable](https://img.shields.io/badge/self%20hostable-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Link](https://www.remote-desktop.co/) · [GitHub](https://github.com/TheoGibbons/remote-desktop)

To use: 1. Download the Windows app and/or the Android APK. 2. Paste the same relay URL and session key into both devices. 3. Approve the pairing prompt on the other device.

Control a Windows PC from Android, control Android from Windows, control one PC from another, and move files in any of those directions. Pair once with a shared session key — there's no login, no token expiry, and no re-authentication after updates.

- Phone → PC: touchpad-style pointer, full on-screen keyboard (including Win, Ctrl, Alt and Shift), every monitor stitched into one canvas, pinch to zoom
- PC → Phone: tap, swipe, Back, Home and Recents on the phone's screen
- PC ↔ PC: the same screen stream plus your physical keyboard and mouse, and a Ctrl+Alt+Del button
- File explorer in both directions, so files never pass through a storage service
- End-to-end encrypted with AES-256-GCM — the relay only ever sees ciphertext
- Every install has its own keypair, and a new device triggers an approve/deny prompt with a device code to compare
- Scan a QR code to copy the server URL and key between devices
- Self-host the relay with one `docker compose` deployment, standalone or behind Traefik
- Windows app in C#/WPF (.NET 8), Android app in Kotlin, relay in Node.js

**Use:** 3 · **Size:** 9

## <img src="https://theogibbons.github.io/notes/favicon.png" alt="App Icon" height="25px"> Notes (aka Simple Drawing Pad)

![No account](https://img.shields.io/badge/no%20account-blue) ![Offline](https://img.shields.io/badge/offline-blue) ![PWA](https://img.shields.io/badge/pwa-blue) ![Export Image](https://img.shields.io/badge/export%20image-blue) ![Local Save](https://img.shields.io/badge/local%20save-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Link](https://theogibbons.github.io/notes) · [GitHub](https://github.com/TheoGibbons/notes)

To use: click the link. No account needed.

Simple drawing pad with an infinite canvas.

- Works offline and online
- Installable PWA (Progressive Web App)
- Draw arrows
- Draw rectangles
- Draw circles
- Draw text
- Pen drawing
- Insert images (crop, rotate)
- Ctrl+V to paste images
- Ctrl+S to instantly save
- Save as PNG, WebP etc.
- Save the project in LocalStorage

Built because I was tired of Paint's limited drawing space and simplistic functions. The complexity of GIMP/Illustrator isn't suitable for simple everyday tasks either, so this app sits somewhere between the two.
Very functional, but I haven't done any work on making the UI pretty.

**Use:** 0 · **Size:** 4

## <img src="https://www.sinkmailer.com/favicon.ico" alt="App Icon" height="25px"> Sink Mailer

![Account required](https://img.shields.io/badge/account%20required-blue) ![Hosted](https://img.shields.io/badge/hosted-blue) ![SMTP](https://img.shields.io/badge/smtp-blue) ![Multi user](https://img.shields.io/badge/multi%20user-blue)

[Link](https://www.sinkmailer.com)

To use: 1. Create an account. 2. Add the SMTP credentials to your app's config.

Targeted at testing email on staging/local servers.
Send any email from your app with the knowledge that it won't reach a real user, then log in to your Sink Mailer account to see everything that has been captured.

- Create multiple inboxes (one per project, or per environment)
- Invite other users to your inboxes
- Save emails as `.eml` files
- Never worry about emails reaching their destination

**Use:** 3 · **Size:** 8

## <img src="https://www.mysql-browser.com/favicon.svg" alt="App Icon" height="25px"> MySQL Browser

![Desktop app](https://img.shields.io/badge/desktop%20app-blue) ![Windows](https://img.shields.io/badge/windows-blue) ![Electron](https://img.shields.io/badge/electron-blue) ![SSH](https://img.shields.io/badge/ssh-blue) ![Auto updates](https://img.shields.io/badge/auto%20updates-blue)

[Link](https://www.mysql-browser.com/)

The fastest and simplest MySQL and Postgres browser you'll use.

- Multi-threaded, so one query doesn't slow down another
- Windows app
- Auto updates
- Built on Electron
- Unsigned exe, so Windows complains on first install
- Supports SSH
- Supports SSH with AWS IAM credentials

**Use:** 2 · **Size:** 8

## <img src="https://baby.sinkmailer.com/icon.svg" alt="App Icon" height="25px"> Measure the Baby

![Account required](https://img.shields.io/badge/account%20required-blue) ![PWA](https://img.shields.io/badge/pwa-blue) ![PDF print](https://img.shields.io/badge/pdf%20print-blue) ![CSV](https://img.shields.io/badge/csv-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Link](https://baby.sinkmailer.com/) · [GitHub](https://github.com/TheoGibbons/measure-the-baby)

Easily track your baby's weight, height, head circumference and BMI. From birth to age 5, this app tells you what percentile your baby's numbers are in.

- Percentile numbers taken directly from the WHO (World Health Organisation) Child Growth Standards
- Print a well formatted PDF, ready to take to your doctor
- Installable PWA (install on mobile or desktop)
- Easy sign-in (email and password), no email verification, no MFA
- CSV import and export

**Use:** 1 · **Size:** 4

## <img src="https://baby-sign-language.vercel.app/_next/image?url=%2Fstatic%2Fimages%2Flogo.png&w=128&q=75" alt="App Icon" height="25px"> Baby Sign Language

![No account](https://img.shields.io/badge/no%20account-blue) ![Next.js](https://img.shields.io/badge/next.js-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://baby-sign-language.vercel.app/) · [GitHub](https://github.com/TheoGibbons/baby-sign-language)

To use: click the link. Optionally create an account to save signs to a list.

Re-skin of [babysignlanguage.com](https://www.babysignlanguage.com).

- Instant search
- Log in with only a username
- Create favourite lists
- Add/remove signs from lists
- Embedded YouTube links
- Many list view options
- Next.js

**Use:** 0 · **Size:** 4

## <img src="https://www.shred-link.com/favicon.svg" alt="App Icon" height="25px"> Shred Link

![No account](https://img.shields.io/badge/no%20account-blue) ![Self destructing](https://img.shields.io/badge/self%20destructing-blue) ![File uploads](https://img.shields.io/badge/file%20uploads-blue)

[Link](https://www.shred-link.com/)

Share a secret over a link that destroys itself. Paste text, attach files, set a view limit and/or a time limit, and the content is erased from the server the moment either limit is reached. One container, no external services, no accounts.

**Use:** 0 · **Size:** 4

## <img src="https://theogibbons.github.io/password-generator/favicon.svg" alt="App Icon" height="25px"> Password Generator

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/password-generator/index.html) · [GitHub](https://github.com/TheoGibbons/password-generator)

Generates passwords... Simple.

**Use:** 0 · **Size:** 1

## <img src="https://theogibbons.github.io/timezone-converter/favicon.ico" alt="App Icon" height="25px" style="background:white"> Timezone Converter

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Link](https://theogibbons.github.io/timezone-converter/index.html) · [GitHub](https://github.com/TheoGibbons/timezone-converter)

What time is it in another timezone? Add as many timezones as you want.

- Page state saves automatically to LocalStorage
- The list of available timezones comes from the browser's JavaScript environment, so every timezone is supported

**Use:** 0 · **Size:** 1

## Chatbot Widget

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Vanilla JS](https://img.shields.io/badge/vanilla%20js-blue) ![Backend agnostic](https://img.shields.io/badge/backend%20agnostic-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/chatbot/index.html) · [Full page](https://theogibbons.github.io/chatbot/fullpage.html) · [Embedded](https://theogibbons.github.io/chatbot/embedded.html) · [GitHub](https://github.com/TheoGibbons/chatbot)

A drop-in chat widget that floats on the bottom-right of any website. It ships with a fake in-memory backend, so it works straight from a clone with no server at all — point it at your own endpoints when you're ready.

- Three layouts: floating widget, full page, or embedded inside a panel
- Conversations, participants and a user picker
- File uploads with progress, and attachments on messages
- SMS / WhatsApp / Email channels, with the WhatsApp 24-hour window enforced
- Send now or schedule for later
- Read receipts, typing indicators and online presence
- Optimistic UI that reconciles when the server acknowledges
- Drafts autosave as you type
- Light, dark and auto themes
- Small JS API on `window.ChatbotAPI`
- No dependencies and no build step

**Use:** 5 · **Size:** 5

## <img src="https://theogibbons.github.io/crafting-calc/favicon.svg" alt="App Icon" height="25px"> Crafting Calculator

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Local save](https://img.shields.io/badge/local%20save-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/crafting-calc/index.html) · [GitHub](https://github.com/TheoGibbons/crafting-calc)

Design and optimise a production chain on an infinite canvas. Add machines, give them input and output rates, wire them together, and it works out the throughput and shows you where the bottlenecks are. Inspired by the production planners people build for factory simulation games.

- Infinite canvas — drag, zoom and pan
- Add, rename and configure machines with custom inputs and outputs
- Connect machines to visualise item flow
- Automatic efficiency and bottleneck calculation
- Autosaves to LocalStorage every 10 seconds and reloads on open
- Save and load designs to share them

**Use:** 0 · **Size:** 5

## Tailwind Class Search

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/tailwind-class-search/frontend/public/index.html) · [GitHub](https://github.com/TheoGibbons/tailwind-class-search)

Search a Tailwind CSS build by class name *or* by the CSS property it produces. Useful when you know the CSS you want but not what Tailwind calls it.

- Search in both directions: class name → CSS, or CSS property → class name
- A build script downloads a Tailwind CSS file and flattens it into JSON, so you can point it at any version — or any other stylesheet
- The generated JSON is committed, so the demo is a plain static page

**Use:** 0 · **Size:** 1

## Colour Matcher

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/colour-matcher/index.html) · [Colour average](https://theogibbons.github.io/colour-matcher/color-average.html) · [GitHub](https://github.com/TheoGibbons/colour-matcher)

Find the part of an image that most closely matches a colour you pick. Built for matching yarn against a photo, but it works for anything.

- Drag squares over the image to sample the average colour of those areas
- Add one or more target colours and see which sampled area is closest
- Match percentage for every colour
- Average colour across everything you sampled
- Second page for averaging a list of colours on its own
- Canvas based, so nothing is uploaded anywhere

**Use:** 1 · **Size:** 1

## QR Video

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![For fun](https://img.shields.io/badge/for%20fun-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Encode](https://theogibbons.github.io/qr-video/encode.html) · [Decode](https://theogibbons.github.io/qr-video/decode.html) · [GitHub](https://github.com/TheoGibbons/qr-video)

Turn any file into a video where every frame is a QR code, then turn it back into the original file. Entirely in the browser. Why would you want to do this? No idea.

- The encoder slices the file into chunks and paints each one as a QR frame
- The decoder scans the frames back in any order and rebuilds the file
- A SHA-256 hash is embedded in the header frame and verified on decode
- Advanced pages expose FPS, codec, error-correction level and the choice of QR recogniser
- Tries several QR engines: ZXing (JS and WASM), plus the browser's `BarcodeDetector` when it exists
- Fast path muxes via WebCodecs, falling back to `MediaRecorder`

Inspired by a Reddit post suggesting you could shrink files this way and back them up on YouTube. In practice any video compression makes the QR codes unreadable, so that part doesn't work — but the round trip does. A 59 KB JPG becomes a 1.5 MB, 10 second video.

**Use:** 1 · **Size:** 1

## <img src="https://theogibbons.github.io/image-measurer/favicon.ico" alt="App Icon" height="25px"> Image Measurer

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Export Image](https://img.shields.io/badge/export%20image-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/image-measurer/index.html) · [GitHub](https://github.com/TheoGibbons/image-measurer)

Measure distances and angles on an image. Set a units-per-pixel scale and the measurements come out in real-world units.

- Drag and drop any image
- Set a scale and a unit label to convert pixels into metres, mm, or anything else
- Hold Ctrl to show the interior angle to the previous line
- Hold Shift to chain measurements together
- Adjust line width, font size and colour
- Download the image with the measurements drawn on it
- Runs entirely in the browser, so nothing is uploaded

**Use:** 1 · **Size:** 1

## Audio Visualiser

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Microphone](https://img.shields.io/badge/microphone-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/audio-visualiser/demo.html) · [GitHub](https://github.com/TheoGibbons/audio-visualiser)

Visualises microphone input in real time on a canvas. Include two scripts, point it at a canvas element, and call one function.

- Multiple visual themes — bars, borders, bezier curves and several circular styles
- Real time, straight from the live microphone stream
- Two-line integration

**Use:** 0 · **Size:** 1

## JS Zoomer

![No account](https://img.shields.io/badge/no%20account-blue) ![npm package](https://img.shields.io/badge/npm%20package-blue) ![jQuery](https://img.shields.io/badge/jquery-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Simple demo](https://theogibbons.github.io/js-zoomer/demo-simple.html) · [Complex demo](https://theogibbons.github.io/js-zoomer/demo-complex.html) · [npm](https://www.npmjs.com/package/js-zoomer) · [GitHub](https://github.com/TheoGibbons/js-zoomer)

Adds image zooming to a web page. Wrap an image in a `.zoomer-container` div, include the CSS and JS, and that's the whole integration.

- Click to zoom
- Pinch to zoom on touch screens
- Mouse wheel to zoom
- Pan with the mouse or by dragging
- Mobile friendly
- Works at any image size
- Published on npm as `js-zoomer`
- Requires jQuery

**Use:** 2 · **Size:** 2

## Tank Track Simulator

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![No dependencies](https://img.shields.io/badge/no%20dependencies-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/tank-simulator/index.html) · [GitHub](https://github.com/TheoGibbons/tank-simulator)

Drive a tank with an accelerator, a steering wheel and a gear lever, and watch those three inputs get converted into thrust for each individual track. A demonstration of differential drive kinematics on an HTML5 canvas.

- Accelerator, steering wheel, and a Forward/Neutral/Reverse gear lever
- Live thrust readouts for the left and right track
- Tracks are colour coded — green for forward, red for reverse
- At full lock the tank pivots around one track
- Wrap-around world, so the tank reappears on the opposite edge
- Plain HTML, CSS and JavaScript with no dependencies

**Use:** 0 · **Size:** 0

## Bezier Curve Drawer

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/bezier-curve-drawer/index.html) · [GitHub](https://github.com/TheoGibbons/bezier-curve-drawer)

A visualiser for the canvas `bezierCurveTo()` function. Click four times to place a curve's points, then drag any of them around to see what the arguments actually do. Each new curve continues from the last one's end point.

**Use:** 0 · **Size:** 0

## Infinite Spinner

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![No dependencies](https://img.shields.io/badge/no%20dependencies-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Simple demo](https://theogibbons.github.io/infinite-spinner/demo-simple.html) · [Options demo](https://theogibbons.github.io/infinite-spinner/demo-multiple.html) · [GitHub](https://github.com/TheoGibbons/infinite-spinner)

A loading spinner drawn on a canvas. One script, no dependencies — call `infiniteSpinner(canvas)` and it runs.

- Configurable rotation speed, arc length, stroke colour, line width and line cap
- One file, no build step, no dependencies

**Use:** 0 · **Size:** 0

## Matrix Multiplication Calculator

![No account](https://img.shields.io/badge/no%20account-blue) ![Client side](https://img.shields.io/badge/client%20side-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[Demo](https://theogibbons.github.io/matrix-multiplication/index.html) · [GitHub](https://github.com/TheoGibbons/matrix-multiplication)

Multiply two matrices. Add or remove rows and columns on either matrix, and the result updates as you type.

**Use:** 0 · **Size:** 0

## Professionator

![Game addon](https://img.shields.io/badge/game%20addon-blue) ![World of Warcraft](https://img.shields.io/badge/world%20of%20warcraft-blue) ![Lua](https://img.shields.io/badge/lua-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[GitHub](https://github.com/TheoGibbons/professionator)

To use: drop the folder into `World of Warcraft\_classic_\Interface\AddOns`. Reagent pricing comes from the Auctionator addon, so install that too.

A World of Warcraft Classic addon that works out the cheapest way to level a profession from one skill level to another. It opens alongside the trade skills window and tells you what to craft at every skill point along the way.

- Weighs every candidate recipe at each skill point and picks the cheapest overall path, rather than just the cheapest next step
- Prices reagents from the auction house and vendors through Auctionator
- Spends the reagents already in your bags and bank before costing anything you'd have to buy
- Knows which recipes your character already has, so it doesn't charge you to train them twice
- Factors in training cost and cast time
- Recipe database is generated from game data — Enchanting and Engineering so far, the rest are on the TODO list
- Ships with its own in-game unit test runner (`/professionator test`)
- Built on Ace3, with an options panel in the Blizzard settings window

**Use:** 5 · **Size:** 5

## Astroneer EVA Spawn Fix

![Game mod](https://img.shields.io/badge/game%20mod-blue) ![Windows](https://img.shields.io/badge/windows-blue) ![Single player](https://img.shields.io/badge/single%20player-blue) ![Lua](https://img.shields.io/badge/lua-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[GitHub](https://github.com/TheoGibbons/astroneer_spawn_eva)

To use: install the UE4SS mod loader, drop in `main.lua`, enable it in `mods.txt` and `mods.json`, then press Ctrl+Y in game.

A one-file mod that fixes the bugged "Need Input" mission in Astroneer, where EVA never spawns in the Sun Room and the quest can't be completed. It binds Ctrl+Y to spawn EVA in front of you so you can talk to her.

- Fixes a crash-induced softlock that otherwise blocks the rest of the mission chain
- Single player only — it doesn't affect multiplayer, and it won't cost you achievements
- Adds files to the game directory rather than modifying any game files, so uninstalling is just deleting them again
- Also covers the later missions that need EVA: *You Are a Very Good Helper*, *I Am a Fox* and *S-O-S*
- The README walks through every step, including backing up your saves first

**Use:** 3 · **Size:** 1

## Unix Simple Website Backup

![Server side](https://img.shields.io/badge/server%20side-blue) ![PHP](https://img.shields.io/badge/php-blue) ![MySQL](https://img.shields.io/badge/mysql-blue) ![AWS S3](https://img.shields.io/badge/aws%20s3-blue) ![Open source](https://img.shields.io/badge/open%20source-blue)

[GitHub](https://github.com/TheoGibbons/unix-simple-website-backup)

To use: upload `backup.php` to your server, fill in `.config.php`, and add it to crontab.

Dumps your MySQL databases, zips them up alongside your web directories, and uploads the lot to S3. Aimed at the small single web server running a couple of sites, where a full backup product is overkill.

- Handles multiple sites and multiple databases in one zip
- Uploads to S3 using an IAM user scoped to a single bucket
- Prunes old backups on a sensible schedule instead of keeping everything:
  - Older than a week: only Mondays and the 1st of the month are kept
  - Older than a month: only the 1st of the month is kept
  - Older than a year: only the 1st of January is kept
- `restore.php` walks you back through a restore with a wizard
- Runs from crontab

**Use:** 6 · **Size:** 3

# Info

*Are these all just vibe coded apps?*

> Most of these were built before LLMs were a thing, but were never published publicly. LLMs made publishing and generating READMEs simpler, hence them being published recently.
