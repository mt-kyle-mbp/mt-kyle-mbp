### Hi, I'm Kyle

I'm a musician, mix engineer and game audio director in Los Angeles. I also write software: music tools at Style Audio and a game at MoonTech Studios. The code for these projects is in private repositories, so this page describes what is in them.

---

## GAGE: a generative music engine

GAGE Sampler is a multi-sampling instrument paired with a generative engine that composes and plays its own music from a saved template. It runs as a standalone app and a VST3/AU plug-in on Mac and Windows. GAGE Player plays the same templates on iOS, and GAGE Core is the engine as a library for games.

- C++ with JUCE, Swift and SwiftUI for the iOS player, and a PHP and SQLite licence server
- A real-time audio engine with a weighted-random music generator (look-ahead, chord modes, key and scale arrangement)
- GAGE Core for Godot (GDExtension), a C API for other game engines, and OSC control from games
- Signed and notarized installers for macOS and Windows built with GitHub Actions, signed licence files, and an in-app instrument store
- An automated test suite

GAGE Sampler 1.1.0 is available at [style-audio.com](https://style-audio.com/).

<img src="images/gage-sampler.jpg" alt="GAGE Sampler" width="720">

---

## MoonTech Game Table: a fantasy role-playing game (in development)

MoonTech Game Table (MTGT) is a 3D fantasy role-playing game with a dungeon building kit, made in Godot 4 for iPad, Mac and PC. The game runs tabletop rules, with or without a live Dungeon Master, and each player can throw their own dice or fight in real time.

- About 65,000 lines of GDScript, Python and Swift tools for the art and voice pipelines, and over 640 automated tests
- Real-time six-second rounds, with players who roll their own dice in the same fight
- Play across devices through a relay server on Cloudflare Workers or over local Wi-Fi, with lockstep orders
- A Dungeon Master mode that sees the whole map and can rebuild anything the players haven't reached
- A level builder, a character creator, barter trading, voiced dialogue, and live music from GAGE Core
- Builds for iPad (TestFlight), Mac (notarized) and Windows

<img src="images/mtgt-title-108.jpg" alt="MTGT title screen" width="720">

<img src="images/mtgt-toll-108.jpg" alt="The Sexton meets the party in the village of the Toll at Midnight" width="356"> <img src="images/mtgt-builder-108.jpg" alt="Building the Bone Cellar in the dungeon builder" width="356">

<sub>Captures from development build 108. I made the title painting and the interface art with Midjourney. Much of the 3D art is licensed stand-in work by other creators: Necropolis by Cryptic Realms; Demonic Village, Fantasy Dungeon, Dwarven Dungeons and Merlin's Cave by Leartes Studios; Medieval Dungeon by Infuse Studio; Dungeon Environment by PackDev; Modular Medieval Tavern by Danilo Waselciac; Medieval Village Props by DuplexG; Ancient Treasures by Dekogon Studios; Soul: Cave by Epic Games; Quixel Megascans; trees from Poly Haven; figures and animations from Adobe Mixamo and Quaternius; fonts by Natanael Gama (Cinzel) and Huerta Tipográfica (Alegreya Sans). Earlier stand-in models are credited at [moontechstudios.com/mtgt-credits.html](https://moontechstudios.com/mtgt-credits.html).</sub>

---

## MoonTech MIDI Editor: free, in the browser

A piano-roll MIDI editor in a single HTML file. It opens and saves Standard MIDI Files, highlights the key and scale, and has Pro Tools-style keyboard editing, quantize and a velocity pencil. It needs no install, works offline, and uses [@tonejs/midi](https://github.com/Tonejs/Midi) to read and write the files. It's free at [moontechstudios.com/midi-editor](https://moontechstudios.com/midi-editor/).

---

## Also

- The websites for [moontechstudios.com](https://moontechstudios.com/) and [style-audio.com](https://style-audio.com/), built with Python static site builders and their own deploy scripts

I'd be happy to walk through any of this code. You can reach me through [moontechstudios.com](https://moontechstudios.com/about.html).
