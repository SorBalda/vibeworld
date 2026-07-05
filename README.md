# VibeWorld

> A neon planet of ten continents — nine sciences orbiting the Agora, the
> crossroads at the center — and you walk a terminal map of your own
> field, meeting other devs at street corners
> named after the people and papers you argue about. Keep each other
> company at 2am while the code misbehaves; and when your AI agent "fixes"
> the failing test by deleting it, take a rocket to the moon and scream.

Discord became a list of servers.\
Slack became work.\
Social media became feeds.

**We wanted a place.**

So we built one — an MMO that runs in your terminal. Not a metaphor:
a multiplayer TUI, a cyberpunk, neon-lit planet you walk street by
street — no browser, no Electron, one pure-Go binary. Then it starts
doing things terminals aren't supposed to do. Voice chat with zero
extra installs — the codec ships inside the binary. A pixel-art avatar
editor with a palette, undo, and working mouse support, in the
terminal. A rocket to the moon, where you type what your LLM did to
you this time and launch the scream into orbit — and everyone on the
planet reads it in the sky, right next to the moon (see *The moon*).

A planet, not another server list. Come with friends and claim a
street corner, or show up alone at 3am and watch comets from a ledge
on the moon — it holds up either way (see *Fine on your own, too*).
Installing it just to see it is a valid use case:

```sh
curl -fsSL https://raw.githubusercontent.com/SorBalda/vibeworld/main/install.sh | sh
vibeworld
```

One binary, zero dependencies, checksum-verified — details in *Install*.

![Terra and Luna, seen from space](docs/screenshots/space.png)

Leave it running on a second monitor while you actually work. It's not
asking for your attention — it's just there, the way a window is.

![Working on the main screen, VibeWorld alive on the second](docs/screenshots/second-monitor.svg)

Take the rocket to Luna and you can just... watch. Alone, or next to
whoever's already sitting at the Stargazer's Ledge — the sky doesn't
check who's there before it's worth looking at.

![Watching the sky together](docs/screenshots/stargazing.gif)

## Install

One command. One binary. Zero dependencies — voice chat included, and
there is *nothing else to install*: the audio codec is pure Go.

```sh
curl -fsSL https://raw.githubusercontent.com/SorBalda/vibeworld/main/install.sh | sh
vibeworld
```

The script detects your OS/arch, verifies the SHA256, and drops a single
binary in `~/.local/bin`. Windows: grab `vibeworld-windows-amd64.exe` from
the [Releases page](https://github.com/SorBalda/vibeworld/releases).
Linux and Apple Silicon (M-series) Macs are supported today; **Intel Mac
support is coming soon**.

The public server is built in: **`wss://vibecity-andrea.fly.dev/ws`**.
VibeWorld is early — one trial server, capped at 350 online at once, and
it sleeps when nobody's around, waking on the first connection. If your
login takes a second, that's the server booting because you showed up:
not a crowd, a feature — an empty world shouldn't run up an idle cloud
bill. Some nights it *will* be quiet. That's fine — the world's still
live and there's plenty to do with no one else online (see *Fine on your
own, too*); someone tends to wander in eventually.

No account needed. `vibeworld --anon` if you'd rather be nobody.

## Update

Same command as installing — the script always fetches the latest release:

```sh
curl -fsSL https://raw.githubusercontent.com/SorBalda/vibeworld/main/install.sh | sh
```

Windows: grab the newest `vibeworld-windows-amd64.exe` from the
[Releases page](https://github.com/SorBalda/vibeworld/releases).

You don't need to check by hand: when a new version is out, vibeworld
shows a `▲ update available` line at login with the exact command to
run. `vibeworld --version` prints what you're running. To stay in the
loop, watch the [Releases page](https://github.com/SorBalda/vibeworld/releases)
(GitHub → Watch → Custom → Releases).

## A planet of nine sciences and a crossroads

Log in and you're floating between Terra and Luna — pick a direction and
you're in it. Continents are disciplines. Artificial Intelligence is a
landmass. Engineering is another. The Agora sits at the center, the
crossroads everyone orbits. You orbit, you pick, you descend.

![The globe turning as you scroll through regions](docs/screenshots/planet-rotate.gif)

In the Agora stands the Tablet of the **Ten Commandments of Science**
("Your agent 'fixed' the test. It is gone."):

![The Tablet of the Ten Commandments, in the Agora](docs/screenshots/agora-tablets.png)

They're engraved at the crossroads of the world because every
discipline walks past them on the way to its own continent. Nobody
follows them. That's why they're carved in stone.

## Cities are street graphs

Every city is a neon plan you actually *walk*, junction to junction.
Corners are named after the people your field argues about.

![Deep Learning city map](docs/screenshots/city-map.png)

Press `Enter` on a corner and it goes full 3D — towers, rain of dead
pixels, whoever else is standing there, and a chat panel. A corner is a
room. A monument is a gathering. Walk up and you're in it.

![A 3D corner scene](docs/screenshots/city-3d.png)

## You, but honest

On your first login you put on a specialization: a macro-area and one
line of truth, shown on your card to everyone you meet.

![Choosing a specialization](docs/screenshots/specialization.png)

Your card can also carry a **GitHub and/or LinkedIn link** (`p` to edit
your own profile). Anyone who likes talking to you can press `g`/`l` on
your card to open them — a two-step confirm, never a one-key surprise
click. It's a social space for people who argue about code at 2am; might
as well let networking happen where it's actually happening.

Then, that first time only, you get an avatar. There is a pixel editor.
It has a palette, undo, mirror mode, a flood fill, and a 3D preview. Yes,
the mouse works. In the terminal. We had to draw the line somewhere and
we drew it as a 16x16 sprite. Come back later and you land straight on
the globe — no re-onboarding.

![The avatar studio](docs/screenshots/avatar-editor.png)

## Other people

Corner chat, city chat, DMs with image and PDF sharing, profiles,
block/report — and slash emotes, because some things a keyboard says
better:

![Two players and a /kiss](docs/screenshots/kiss.png)

`/kiss`. Pixel hearts. `*mhua*`. No microtransactions were involved.

## Voice, with zero installs

Press `ctrl+V` and you're talking — press it again and you stop. The
first press is your mic consent; until then you're listen-only. The
codec is pure Go, the binary you already downloaded is the whole stack:
no PortAudio, no Opus packages, no "please install these 12 system
libraries first".

![ON AIR at the Ledge](docs/screenshots/voice-on-air.png)

(That object in the sky showed up on its own during the screenshot. We
kept it. You would have too.)

## The HELP flare

Stuck at 2am? Step into any corner (`Enter` on it from the street) and
press `!` to type what's wrong. A red ribbon with a countdown goes up
over the junction for everyone in the city to see. It's on-call for
people, not pagers.

![A HELP beacon, seen by another player](docs/screenshots/help-flare.gif)

## The moon

Take the rocket to Luna, the philosophic moon. Two things happen up
there, and they're opposites.

**Screaming.** At the **Complaint Crater** there's a booth. You type
what your LLM did to you this time; the RAGE meter fills as you type;
then you launch your tantrum into orbit. Your scream joins the wall
under `▼ LAST SCREAM HEARD FROM SPACE` — and here's the thing:
*everyone sees it.* Anyone looking at the sky from anywhere on the
planet gets your words next to the moon. Screaming into the void,
except the void has a player count.

![The last scream heard from space](docs/screenshots/moon-scream.gif)

**Stargazing.** The moon also has quiet places. At the **Stargazer's
Ledge** you sit with whoever's there and watch comets, the Earth
passing overhead, and occasionally something that is *no moon*. Press
`ctrl+n` for lo-fi classical — Beethoven, at a sensible volume, on the
actual moon. The **Contemplation Dome** next door is a music-only
sanctuary: no voice, no noise. Some places should stay like that.

## Fine on your own, too

You don't need anyone else logged in for this to be worth it. Leave
VibeWorld open on a second monitor, go sit in a room, watch the sky
from the Ledge, or read the last scream heard from space. The planet,
the moon, the beacons, the wall — the world itself is company. This
isn't `--offline`: you're still on the real server, it's just that some
nights it's quiet. Someone tends to wander in eventually.

## Keys

| Key | Does |
|-----|------|
| `←↑↓→` / `hjkl` | walk the streets · orbit the planet |
| `Tab` | cycle worlds, regions, cities, chat tabs |
| `Enter` | descend · enter a corner or monument · send chat |
| `Esc` | back out, all the way to space |
| `c` | chat in the city |
| `m` | cycle monuments |
| `!` | raise a HELP flare (once inside a corner) |
| `/kiss` `/punch` `/jump` | emotes, typed in chat |
| `ctrl+V` | voice — press to talk, press again to stop |
| `ctrl+n` | lo-fi classical, on the moon |
| `]` | social sidebar (`e` avatar studio · `d` DM) |
| `:` | command console (planet/region) |
| `?` | every key, in-world |
| `q` / `ctrl+C` | quit (the flare, sadly, works only in-world) |

## House rules

- **No recording voice chat.** People talk because it's ephemeral.
- **The Contemplation Dome is a sanctuary.** Music only. Take the
  argument to the Complaint Crater, that's what it's for.
- Block and report exist and work. Be someone worth stargazing with.

## Privacy & safety

Plain facts, no marketing. Your connection is TLS (`wss://`), and every
handle, message, bio, shared filename, HELP line, and complaint that
reaches your terminal is stripped of control and escape sequences before
it renders — so a hostile peer or server can't hijack your terminal
through a chat line (`internal/textsafe`, applied on both ends). What we
*don't* do: there is no end-to-end encryption. The server relays — and
can see — your text, DMs, shared images/PDFs, and voice, so don't send
anything you'd mind a server operator seeing. Voice isn't recorded (it's
ephemeral by design; see *House rules*), but it isn't E2E-encrypted
either. Block and report exist and work.

## For developers

Modding starts at [`mod-sdk/`](mod-sdk/) (Apache-2.0): declarative
worldpacks — data, not code.

## License

Today: VibeWorld ships as **closed binaries** (free to use) talking to a
**closed, proprietary server** — client source isn't public yet, server
stays unpublished. What *is* open right now: the **Mod SDK**
([`mod-sdk/`](mod-sdk/)) is **Apache-2.0**. The client source is
*planned* to open under **PolyForm
Perimeter 1.0.0** (read it, mod it, build it — just don't ship a
competing clone), but there's no date yet — take "soon" as intent, not
a promise, and watch the repo.

Don't want to trust a closed world? **`vibeworld --offline`** runs a
full self-contained world with no server at all — your machine, your
rules, nothing phoned home.

Full text: [`LICENSE`](LICENSE). The name is reserved:
[`TRADEMARK.md`](TRADEMARK.md).

---

Your terminal has been a place of work for decades.
It can be a place, full stop. See you on the moon. ✦
