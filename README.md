# VibeWorld

Discord became a list of servers. Slack became work. Twitter became a feed.

We built a place instead: a neon multiplayer world that runs *in your terminal*.

[![Latest release](https://img.shields.io/github/v/release/SorBalda/vibeworld?label=release)](https://github.com/SorBalda/vibeworld/releases/latest)
[![Mod SDK: Apache-2.0](https://img.shields.io/badge/Mod%20SDK-Apache--2.0-blue)](mod-sdk/)
[![Platforms: Linux · macOS · Windows](https://img.shields.io/badge/platforms-Linux%20%C2%B7%20macOS%20%C2%B7%20Windows-informational)](#get-in-right-now)

![The whole way down: from space to the turning globe, down through a region into a city, to a HELP flare and a corner conversation](docs/screenshots/journey.gif)

*That's a GIF, i.e. a re-render. Don't believe GIFs. [Play the raw asciinema recording](https://sorbalda.github.io/vibeworld/#cast) instead — real bytes, real timestamps, no editing.*

## Get in. Right now.

```sh
curl -fsSL https://raw.githubusercontent.com/SorBalda/vibeworld/main/install.sh | sh
vibeworld
```

![The one-liner in action: curl pipes to sh, the binary downloads, the SHA256 verifies, and it says "See you on the moon"](docs/screenshots/install.gif)

One command. One small binary. Voice chat already inside it. No account, no
extra packages, nothing else to configure.

**Windows:** grab [`vibeworld-windows-amd64.exe`](https://github.com/SorBalda/vibeworld/releases/latest) from Releases and run it.

If that made you grin, a ⭐ helps the next person find this before you scroll away.

## This is what you walked into

Pick a field — AI, Bio, Physics, whatever you actually do — and you land on its
continent: a neon city where the streets are named after the people and papers
you argue about, and everyone else in that field is walking it *right now*,
live, under their own @handle.

![Walking the Deep Learning streets while ten other people do the same, live](docs/screenshots/city-crowd.gif)

Press `Enter` on a monument and the screen goes full 3D. Whoever's there is
standing at its base. Press `!` on an empty line and you perform the *rite* —
it lights up the whole screen and the plaque remembers it forever ("performed
12× in living memory · last by @you").

![Inside The Knuth Plaza in full 3D: a rite just performed, the shockwave still ringing, two avatars at the base](docs/screenshots/city-3d.png)

You get a face too. Real pixel editor, mouse and all — colors, undo, mirror,
fill, a spinning 3D preview. 16x16 pixels, because we had to stop somewhere.

![The avatar studio](docs/screenshots/avatar-editor.png)

Yes, the mouse works. In a terminal. Click a corner, a person, a button, the
map — all of it.

And when the street feels small: press `Tab`. `#city` is whoever shares your
streets; `#world` is *everyone awake, everywhere* — one channel for the whole
world, reachable from any room, any screen, the moon, even drifting in space.
Every line says where it came from (`·deep-learning`, `·moon`). It never
chimes, never pings you — a murmur you visit, not a noise that finds you.

![A #world message arriving in a street corner, origin tag and all](docs/screenshots/world-chat.png)

## Found your own corner

Don't like what's on the map? Make your own. Press `C`, then `n`, aim with the
mouse, click — a corner appears with your name on it, forever, or until you
tear it down yourself.

![Founding a corner with the mouse: the ghost marker glides across the map with the live "found your corner here" hint, one click, a name typed — and the corner stands there with your handle on it](docs/screenshots/corner-placement.gif)

Found one out past the edge of the map and the city notices — it grows,
threading brand-new streets out to meet you. The map remembers you were here.

![A corner founded on the far edge: fresh green streets now reach out to it, named after its founder](docs/screenshots/corner-edge-growth.png)

Nobody visits yours in 30 days, it crumbles. Use it or lose it.

## Take the rocket. Scream.

Your agent "fixed" the failing test by deleting it. Fine. Take the rocket to
Luna and unload at the **Complaint Crater**. Type it out, watch the RAGE meter
climb — ALL CAPS counts triple, a row of "!!!" counts six times — then launch.
Your scream goes up on the wall for the *entire planet* to read, and it stays
there even after the server restarts.

![Typing a scream at the Complaint Crater: "MY AGENT DELETED THE FAILING TEST. THE TEST WAS THE FEATURE???", the RAGE meter climbing, the rocket launching](docs/screenshots/complaint-crater.gif)

Screaming into the void, except the void has a player count.

## Then go be quiet for a while

Moon's got more than a scream booth. At the **Stargazer's Ledge** you sit with
whoever's there and watch the sky do things: comets, auroras, a supernova, the
odd space battle, occasionally something that is *no moon*. Eleven kinds of
event, never the same night twice. `ctrl+n` for lo-fi Beethoven at a gentle
volume, on the actual moon.

![Watching the sky together from the Stargazer's Ledge](docs/screenshots/stargazing.gif)

There's also a plant. One plant, shared by the whole moon, sitting on the
Ledge. Water it (`!`) and it grows. Ignore it for two days and it dies — really
dies, back to a seed — and nobody brings it back but you.

![The moon plant withered to a bare stalk: "watered by @Andrea · withered · water to revive"](docs/screenshots/plant-dying.png)

The **Contemplation Dome** next door is music only. No voice, no local
chatter, no noise. The one thing that reaches it is `#world` — even the quiet
room can hear the whole planet murmur, softly, if it asks.

## Paint the wall

**The Regolith Wall.** A shared pixel canvas on the moon, and there's exactly
one — everybody who ever visits paints on the same mural. Brush, pen, colors,
eraser, the works.

![Painting The Regolith Wall: a colorful mural mid-progress, brush size and color picker at the bottom](docs/screenshots/graffiti-wall.png)

Zoom back out to the moon overview and there it is — your mural, shrunk down
to a little glowing picture on the side of the building. Visible from orbit.
The whole planet's graffiti, permanent, from space.

![The moon overview: The Regolith Wall building shows the shared mural as a small thumbnail, visible from orbit](docs/screenshots/moon-mural-thumb.png)

## The rest of it

**Ten Commandments of Science**, carved in stone at the Agora crossroads
("Your agent 'fixed' the test. It is gone."). Everyone breaks at least three a
week. That's why they're carved in stone.

![The Tablet of the Ten Commandments, in the Agora](docs/screenshots/agora-tablets.png)

**HELP flares.** Stuck at 2am? Press `!` in a corner, say what's wrong, and a
red countdown ribbon goes up over your head. Anyone in the city can walk over.
Help from people, not a ticket queue.

![A HELP beacon, seen by another player](docs/screenshots/help-flare.png)

**The arcade at the Agora is multiplayer**, not decoration. Walk in
mid-match and you don't watch — you join the running game, score and all,
your avatar standing in the field with the rest of the crew.

![Two players in the same Glitch Collector match, crew tally and score climbing](docs/screenshots/arcade-multiplayer.gif)

In THE GRID the enemies are literally labeled "PEER REVIEWED" and "8 more
revisions requested."

![THE GRID: a corridor shooter where the enemies are your actual backlog, closing in fast](docs/screenshots/grid-labels.gif)

**Voice, zero installs.** `ctrl+V` and you're talking; the status line turns
red and says `ON AIR` so nobody's ever surprised. `/kiss`, `/explode`,
`/rocket`, `/d20` and friends for everything else.

![ON AIR at the Ledge](docs/screenshots/voice-on-air.png)

**Alone at 3am is fine too.** Leave it running on a second monitor. It uses
about as much memory as a browser tab and it's not asking for your attention —
it's just there, like company usually is.

![Terra and Luna, seen from space](docs/screenshots/space.png)

## Keys

| Key | Does |
|-----|------|
| `←↑↓→` / `hjkl` | walk the streets · orbit the planet |
| mouse | click anything: corners, people, buttons, the map |
| `Tab` | cycle worlds, regions, cities, chat tabs |
| `Enter` | descend · enter a corner or monument · send chat |
| `Esc` | back out, all the way to space |
| `c` | chat in the city |
| `C` | corners directory · found your own |
| `m` | jump to the monument · cycle them in the Agora |
| `!` | HELP flare (corner) · perform the rite (monument) · water the plant (moon) |
| `/kiss` `/punch` `/rocket` … | emotes, typed in chat |
| `ctrl+V` | voice: press to talk, press again to stop |
| `ctrl+n` | lo-fi classical, on the moon |
| `]` | social column: friends, live presence, requests, People, DMs |
| `p` | edit your own profile (bio, GitHub/LinkedIn links) |
| `:` | command console |
| `?` | every key, in-world |

## House rules

- **No recording voice chat.** People talk because it isn't saved.
- **The Contemplation Dome is a sanctuary.** Take the argument to the Crater.
- Block and report exist and work. Be someone worth stargazing with.

---

## Under the hood

A few notes, for anyone who wants them.

**One binary.** Pure Go, no browser, no Electron. Voice's audio codec is
built in — no PortAudio, no Opus package, nothing else to install.

**Install & updates:** the script detects your OS/arch, verifies the SHA256,
drops one file in `~/.local/bin`. Same command updates it; VibeWorld itself
tells you when a new build is out.

**Platforms:** Linux x64 · Apple Silicon · Windows x64 `.exe` · Intel Mac and
Linux arm64 soon.

**Server:** built in at `wss://vibecity-andrea.fly.dev/ws`. One trial server,
capped at 350 people, sleeps until someone connects — a slow login just means
it's waking up.

**Also:** ~30 MB of RAM. `vibeworld --anon` to stay nobody. `vibeworld
--offline` for a full solo world on your own machine, nothing sent anywhere.

**Privacy:** your connection is TLS (`wss://`). Every handle, message, bio,
and complaint that reaches your terminal is stripped of control/escape
sequences before it's shown, so nobody can hijack your terminal through a chat
line. There's no end-to-end encryption — the server can see what passes
through it, so don't send anything you'd mind an operator reading. Voice
isn't recorded. Block and report work.

**Modding:** starts at [`mod-sdk/`](mod-sdk/) (Apache-2.0) — worldpacks are
data, not code.

**License:** free binaries. The Mod SDK is Apache-2.0; client source is
planned to open under PolyForm Perimeter. Full text: [`LICENSE`](LICENSE).
Name reserved: [`TRADEMARK.md`](TRADEMARK.md).

---

Your terminal has been a place of work for decades. It can be a place, full
stop. See you on the moon. ✦
