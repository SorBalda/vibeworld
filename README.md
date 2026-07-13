# VibeWorld

A neon multiplayer world that runs in your terminal. One small download, voice chat built in, and a moon you fly to and scream at when the agent deletes your tests.

[![Latest release](https://img.shields.io/github/v/release/SorBalda/vibeworld?label=release)](https://github.com/SorBalda/vibeworld/releases/latest)
[![Mod SDK: Apache-2.0](https://img.shields.io/badge/Mod%20SDK-Apache--2.0-blue)](mod-sdk/)
[![Platforms: Linux · macOS · Windows](https://img.shields.io/badge/platforms-Linux%20%C2%B7%20macOS%20%C2%B7%20Windows-informational)](#install)

![The whole way down: space, the turning globe, a region, a city corner conversation, the Stargazer's Ledge, and the moon](docs/screenshots/journey.gif)

*GIFs are rendered video. Want proof it's a real terminal? [Play the raw asciinema recording](https://sorbalda.github.io/vibeworld/#cast) — timestamped bytes, not a re-render.*

> A neon planet of nine continents. Eight sciences orbit the Agora, the
> crossroads at the center, and you walk a terminal map of your own field,
> meeting other devs at street corners named after the people and papers you
> argue about. Keep each other company at 2am while the code misbehaves. And
> when your AI agent "fixes" the failing test by deleting it, take a rocket to
> the moon and scream.

Discord became a list of servers.\
Slack became work.\
Social media became feeds.

**We wanted a place.**

So we built one: a shared world in your terminal. Not a picture of a world — a
real one you walk street by street, a neon planet lit like a cyberpunk city. It
does things terminals are not supposed to do: voice chat, a pixel-art avatar
editor with a mouse that really works, and a rocket to the moon where you type
what your LLM did and launch the scream into orbit for the whole planet to read.

You don't join it like a chat server; you show up and walk around. Come with
friends and take a street corner, or arrive alone at 3am and watch comets from a
ledge. Both work. Installing it just to look at it is fine too.

**▶ [See it on the landing site](https://sorbalda.github.io/vibeworld/)** · **[Download a release](https://github.com/SorBalda/vibeworld/releases)**

**Jump to:** [Install](#install) · [The planet](#a-planet-of-eight-sciences-and-a-crossroads) · [Cities](#cities-are-street-graphs) · [The moon](#the-moon) · [The arcade](#the-arcade-at-the-crossroads) · [Keys](#keys) · [Under the hood](#under-the-hood) · [Privacy](#privacy--safety) · [License](#license)

## Install

```sh
curl -fsSL https://raw.githubusercontent.com/SorBalda/vibeworld/main/install.sh | sh
vibeworld
```

![The one-liner in action: curl pipes to sh, the binary downloads, the SHA256 verifies, and it says "See you on the moon"](docs/screenshots/install.gif)

One command, one small download — voice chat included, no extra packages to
install.

**Windows:** download [`vibeworld-windows-amd64.exe`](https://github.com/SorBalda/vibeworld/releases/latest) from Releases, then run `vibeworld`.

No account needed. More on how it all works is [under the hood](#under-the-hood).

If this made you smile, a ⭐ helps the next person find it.

## You, but honest

Nobody here is "passionate about technology". When you first log in, you pick a
field and write one honest line about yourself. It shows on your card to everyone
you meet.

![Choosing a specialization](docs/screenshots/specialization.png)

Met someone you want to stay in touch with? Your card can hold a **GitHub and/or
LinkedIn link** (press `p` to edit your profile), and anyone can press `g`/`l` to
open them — after a two-step confirm, so no surprise clicks.

Then, that first time only, you make an avatar. There's a real pixel editor:
colors, undo, mirror mode, fill, and a 3D preview. We had to stop somewhere, so
the canvas is 16x16 pixels.

Yes, the mouse works. In the terminal. Not just in the editor — click a corner, a
person, a button, the map. Come back later and you land straight on the globe, no
setup again.

![The avatar studio](docs/screenshots/avatar-editor.png)

## A planet of eight sciences and a crossroads

Log in and you float between Terra and Luna. Pick a direction and you go there.
Each continent is a field of science — Artificial Intelligence is one landmass,
Engineering another, eight sciences around the world. The Agora, the crossroads
at the center, sits where they all meet. You orbit, you pick, you go down.

![The globe you orbit to pick a continent, Terra and Luna hanging in space](docs/screenshots/globe.png) — *animated version on the [site](https://sorbalda.github.io/vibeworld/)*

## Cities are street graphs

Your field already has famous names: the people and papers everyone argues
about. Here they are real streets, a neon map you *walk* corner to corner — and
the streets are live: everyone in the city walks the same map at the same
moment, each under their own @handle.

![Walking the Deep Learning streets while ten other people do the same, live](docs/screenshots/city-crowd.gif)

A corner is a room; a monument is a meeting place. Press `Enter` on one and it
goes full 3D: the monument fills the screen, whoever else is there stands at its
base, and a chat panel keeps the talk. Walk up and you are in it.

![Inside The Knuth Plaza in full 3D: a rite just performed, the shockwave still ringing, two avatars at the base](docs/screenshots/city-3d.png)

Want to leave a mark that lasts? Every landmark keeps a **rite**: press `!` on an
empty chat line inside a monument and it lights up the whole screen, and the
plaque remembers it ("rite performed 12× in living memory · last by @you"). Chat
at a corner comes and goes; what happens at a monument is kept.

## The Ten Commandments of Science

In the Agora stands the Tablet of the **Ten Commandments of Science** ("Your
agent 'fixed' the test. It is gone."):

![The Tablet of the Ten Commandments, in the Agora](docs/screenshots/agora-tablets.png)

They are carved at the crossroads because everyone walks past them on the way to
their own continent. You have broken at least three this week. Nobody follows
them. That is why they are carved in stone.

## The Stands

Also at the Agora: **The Stands**, a shared board. Post a line or drop a PDF, and
like what speaks to you. The best ones stay, liked and stacked, so the crossroads
remembers what people found worth saying.

![The Stands — post a phrase or share a PDF, and like what resonates](docs/screenshots/stands-likes.png)

## The HELP flare

Stuck on a bug at 2am? Step into a corner, press `!`, and say what is wrong: a red
ribbon with a countdown goes up over your corner, and anyone in the city can walk
over. Help from people, not from a ticket queue.

![A HELP beacon, seen by another player](docs/screenshots/help-flare.png) — *animated version on the [site](https://sorbalda.github.io/vibeworld/)*

## The moon

Some nights you need to scream. Some nights you need the sky. Take the rocket
to Luna, the thoughtful moon: it gives you both, and they are opposites.

**Screaming.** At the **Complaint Crater** there is a booth. You type what your
LLM did to you this time; the RAGE meter fills as you write, and it has opinions —
SHOUTING counts triple, a row of "???" counts six times, so real anger fills the
meter long before a calm paragraph would. Then you launch your rant into orbit:
it goes up on the wall under `▼ LAST SCREAM HEARD FROM SPACE`, and *everyone sees
it* — anyone looking up from anywhere on the planet gets your words by the moon,
and they stay even after a server restart. Screaming into the void, except the
void has a player count.

![Typing a scream at the Complaint Crater: the input line fills with "MY AGENT DELETED THE FAILING TEST. THE TEST WAS THE FEATURE???", the RAGE meter climbs, the rocket launches, and the scream tops the wall](docs/screenshots/complaint-crater.gif)

**Stargazing.** The moon also has quiet places. At the **Stargazer's Ledge** you
sit with whoever is there and watch the sky put on its own show: comets, auroras,
a supernova, the Earth passing overhead, the odd space battle, and now and then
something that is *no moon*. Eleven kinds of event, mixed so no two nights look
the same, and shared with everyone at the Ledge. Press `ctrl+n` for lo-fi
classical (Beethoven, at a gentle volume, on the actual moon). The
**Contemplation Dome** next door is music only: no voice, no noise. Some places
should stay that way.

![Watching the sky together from the Stargazer's Ledge](docs/screenshots/stargazing.png) — *animated version on the [site](https://sorbalda.github.io/vibeworld/)*

## The people

Some things are easier to type. Corner chat, city chat, DMs that carry images and
PDFs, profiles, block and report, and slash emotes:

![Two players trading emotes: an /explode and a /kiss](docs/screenshots/kiss.png)

`/kiss`. Pixel hearts. `*mhua*`. `/explode` for when the build does. No
microtransactions were involved. (There's a whole set: `/punch`, `/jump`,
`/rocket`, `/explode`, `/dance`, `/facepalm`, `/highfive`, `/coffee`, `/d20`.)

Want to know if your friends are on? Press `]`: the social column shows them
live, with a `●` when they are online and where they are, so you know whether to
walk over or take the rocket up. Friend requests cross time zones — send one to
someone offline and it arrives at their next login, and requests coming *your*
way wait in a `⇄ REQUESTS` row you accept or decline there.

Finding one person in a nine-continent world should be easy. The same column also
has **People**: everyone online right now, and where. Search by handle, GitHub
login, or field, then open a profile, DM, or add them from the list.

## Voice, with zero installs

Some arguments are faster out loud. Press `ctrl+V` and you are talking; press it
again to stop. The first press is your mic consent; until then you only listen,
and when your mic is live the status line turns **red** and reads `ON AIR`, so you
always know when the world can hear you. No extra audio software — it is all in
the one download.

![ON AIR at the Ledge](docs/screenshots/voice-on-air.png)

(That object in the sky showed up on its own during the screenshot. We kept it.
You would have too.)

## The arcade at the crossroads

Sometimes the fix is shooting something. Two of the Agora's monuments are not
really monuments. Step into **The Arena** and you are in **THE GRID**: a
first-person neon corridor shooter where the gun is the git blame cannon, one
magazine is 24 commits, reloading runs `git commit -am "reload"`, and the wave 5
boss is THE AGENT THAT DELETED YOUR TESTS. Step into **The Pulvinar** for
**GLITCH COLLECTOR**: hold the firewall and squash the glitches before they eat
through it. The other two are honest — **The Furnace** prints a receipt for
whatever you burn, and **The Crowd**'s ROAR meter barely moves for one voice,
then maxes out for a full house.

The point: **the games are multiplayer.** Walk in while someone is already
playing and you don't watch — you *join the running match*, mid-wave, score and
all. The others stand in the game with their own avatars and @handles — pixel
busts on the Glitch field, full 3D billboards in the corridors of THE GRID. A
CREW row keeps the count, and whoever started the match holds the restart key;
press `R` as a guest and the game tells you whose match you walked into.

![Two players in the same Glitch Collector match, crew tally and score climbing](docs/screenshots/arcade-multiplayer.gif)

No quarters. The cabinet at the center of the world runs on karma.

![THE GRID: a corridor shooter where the enemies are your actual backlog — one labeled "PEER REVIEWED", another "8 more revisions requested" — closing in fast](docs/screenshots/grid-labels.gif)

## Fine on your own, too

It's 3am and nobody you know is awake. That's fine. Leave VibeWorld open on a
second monitor while you work — it uses very little memory (see
[under the hood](#under-the-hood)). It is not asking for your attention; it just
sits there, like any open window.

![Working on the main screen, VibeWorld alive on the second](docs/screenshots/second-monitor.svg)

Go sit in a room, watch the sky from the Ledge, or read the last scream heard
from space. The planet, the moon, the beacons, the wall — the world itself is
company. This is not an offline mode; you are on the real server, just quiet some
nights. Someone usually wanders in.

And "quiet" doesn't mean "nothing to do". Alone, on any given night, you can:
walk a continent you've never visited and read street signs named after papers
you've argued about; try the day's Oracle riddle (it's genuinely hard); honour
a monument and leave your mark on its plaque; proclaim a finding at The Stands
for whoever comes next; water the plant on the Ledge before it wilts; clear a
few waves in the arcade; scream at the moon and watch your words orbit the
planet. The multiplayer is the soul, but the world is built to be *walked* —
if you like terminals at all, exploring it solo is the point, not the fallback.

![Terra and Luna, seen from space](docs/screenshots/space.png)

## Keys

| Key | Does |
|-----|------|
| `←↑↓→` / `hjkl` | walk the streets · orbit the planet |
| mouse | click anything: corners, people, buttons, the map. works everywhere |
| `Tab` | cycle worlds, regions, cities, chat tabs |
| `Enter` | descend · enter a corner or monument · send chat |
| `Esc` | back out, all the way to space |
| `c` | chat in the city |
| `m` | cycle monuments |
| `!` | raise a HELP flare (in a corner) · perform the rite (at a monument) |
| `/kiss` `/punch` `/rocket` … | emotes, typed in chat |
| `ctrl+V` | voice: press to talk, press again to stop |
| `ctrl+n` | lo-fi classical, on the moon |
| `]` | social column: friends, live presence, requests, People, DMs |
| `p` | edit your own profile (bio, GitHub/LinkedIn links) |
| `:` | command console (`/profile` · `/logout` · `/quit`) |
| `?` | every key, in-world |
| `q` / `ctrl+C` | quit (the HELP flare, sadly, only works in-world) |

## House rules

- **No recording voice chat.** People talk because it is not saved.
- **The Contemplation Dome is a sanctuary.** Music only. Take the argument to the
  Complaint Crater, that's what it's for.
- Block and report exist and work. Be someone worth stargazing with.

## Under the hood

A few notes, for anyone who wants them.

**One binary.** VibeWorld is a single pure-Go binary — no browser, no Electron,
no extra packages. The audio codec ships inside it, so voice chat needs no
PortAudio, no Opus package, nothing else installed.

**Install & updates:** the script picks the right build for your OS and
processor, verifies the SHA256, and drops one file in `~/.local/bin`. Updating is
the same command — it always fetches the latest release, and at login VibeWorld
shows a `▲ update available` line with what to run.

**Platforms:** Linux x64/arm64 · Apple Silicon · Windows x64 `.exe` · **Intel Mac
soon**.

**Server:** built in at **`wss://vibecity-andrea.fly.dev/ws`**. It is early — one
trial server, capped at 350 people, that sleeps until someone connects, so a slow
login is just the server waking up.

**Also:** about 30 MB of RAM (less than a browser tab). `vibeworld --anon` to
stay nobody; `vibeworld --offline` for a full world on your own machine, with
nothing sent out.

## Privacy & safety

Plain facts, no marketing. Your connection is encrypted (TLS, `wss://`). Every
handle, message, bio, filename, HELP line, and complaint that reaches your
terminal is cleaned of control and escape sequences before it is shown, so a
hostile user or server cannot take over your terminal through a chat line
(`internal/textsafe`, on both ends). What we *don't* do: there is no end-to-end
encryption. The server passes on your text, DMs, files, and voice, and can see
all of it, so don't send anything you would mind a server operator reading. Voice
is not recorded either. Block and report exist and work.

## For developers

Modding starts at [`mod-sdk/`](mod-sdk/) (Apache-2.0): worldpacks are data, not
code.

## License

VibeWorld ships as **free binaries**. The **Mod SDK** ([`mod-sdk/`](mod-sdk/))
is **Apache-2.0**; the client source is planned to open under **PolyForm
Perimeter**.

Full text: [`LICENSE`](LICENSE). The name is reserved: [`TRADEMARK.md`](TRADEMARK.md).

---

Your terminal has been a place of work for decades. It can be a place, full
stop. See you on the moon. ✦
