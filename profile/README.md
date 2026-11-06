# Hagenberg Jams

Jams at the [University of Applied Sciences Upper Austria](https://fh-ooe.at/en/campus-hagenberg), Hagenberg Campus: teams create a game or an animation on one topic within a weekend. Students, alumni and guests take part, on site or remotely.

| Jam | Website | Since |
| --- | --- | --- |
| Hagenberg Game Jam | [hagenberg-gamejam.at](https://hagenberg-gamejam.at) | 2011 |
| Hagenberg Animation Jam | [hagenberg-animationjam.at](https://hagenberg-animationjam.at) | 2021 |

The websites announce the next jam, reveal its topic at the set time, take the registrations and keep an archive of everything the teams made.

## Repositories

| Repository | Content |
| --- | --- |
| [jam-engine](https://github.com/Hagenberg-Jams/jam-engine) | The shared engine behind all jam websites: pages, commands, registration, topic reveal and the build and deployment workflow |
| [hagenberg-gamejam.at](https://github.com/Hagenberg-Jams/hagenberg-gamejam.at) | Content and settings of the Game Jam website |
| [hagenberg-animationjam.at](https://github.com/Hagenberg-Jams/hagenberg-animationjam.at) | Content and settings of the Animation Jam website |

Each jam's team maintains its own website repository. The README there explains the whole jam year step by step. Features that help every jam go into the engine, and each website picks up a new engine version through a pull request.

## How it works

- The websites are static pages built with [HydePHP](https://hydephp.com) and hosted on Cloudflare Pages.
- Every push to `main` of a website repository goes live after its checks. Pull requests get a preview link.
- The topic of a jam stays secret until its reveal. It is never in a repository, and the server only hands it out from the release time on.
- Registrations are stored with Cloudflare and deleted automatically 90 days after the jam.

## Contributing

Found a mistake or have an idea? Open an issue in the repository of the website, or in [jam-engine](https://github.com/Hagenberg-Jams/jam-engine/issues) if it concerns all jams. Pull requests are welcome.
