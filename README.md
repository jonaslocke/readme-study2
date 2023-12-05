### Installation

```bash
$ pnpm
```

### Local Development

```bash
$ pnpm start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```bash
$ pnpm build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```bash
$ USE_SSH=true pnpm deploy
```

Not using SSH:

```bash
$ GIT_USER=<Your GitHub username> pnpm deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.


-----------
## Table of Contents

[a relative link](docs/Best%20Practices/Code%20Reviews/Intro.md)


### Best Practices
- [Code Reviews](docs/Best%20Practices/Code%20Reviews/Intro.md)
- [JIRA](docs/Best%20Practices/JIRA/Intro.md)
- [Redux Toolkit](docs/Best%20Practices/Redux%20Toolkit/Intro.md)
- [Typescript](docs/Best%20Practices/Typescript/Intro.md)
- [Unit Tests - Jest](docs/Best%20Practices/Unit%20Tests%20-%20Jest/Intro.md)
- [Using Nx](docs/Best%20Practices/Using%20Nx/Intro.md)

### Development Best Practices
- [Coding Best Practices](docs/Development-Best-Practices/Coding-Best-Practices.md)
- [Performance Optimization](docs/Development-Best-Practices/Performance-Optimization.md)

### IEX
- [Introduction](docs/IEX/intro.md)
- [project-structure](docs/IEX/project-structure.md)

### Technical-Document
- [HIX-174068](docs/Technical-Document/24.3/HIX-174068.md)
- [HIX-174077](docs/Technical-Document/24.3/HIX-174077.md)
- [HIX-174204](docs/Technical-Document/24.3/HIX-174204.md)

### Tools
- [Charting Libraries](docs/Tools/Charting%20Libraries/Introduction.md)
- [NPM-Registry-Proxy](docs/Tools/NPM-Registry-Proxy/Intro.md)

### ms-telex-ui
- [Overview](docs/ms-telex-ui/24.3/Overview.md)

#### Components
- [Adhoc Notices](docs/ms-telex-ui/24.3/Components/AdhocNotices.md)
- [Failed Table](docs/ms-telex-ui/24.3/Components/FailedTable.md)
- [Notice Full Summary](docs/ms-telex-ui/24.3/Components/NoticeFullSummary.md)
- [Notices Summary](docs/ms-telex-ui/24.3/Components/NoticesSummary.md)
- [Pane Container](docs/ms-telex-ui/24.3/Components/PaneContainer.md)
- [Search Filter](docs/ms-telex-ui/24.3/Components/SearchFilter.md)
- [Widget](docs/ms-telex-ui/24.3/Components/Widget.md)

#### HIX
- [HIX-174231](docs/ms-telex-ui/24.3/HIX/HIX-174231.md)
- [HIX-174237](docs/ms-telex-ui/24.3/HIX/HIX-174237.md)
- [HIX-174239](docs/ms-telex-ui/24.3/HIX/HIX-174239.md)
- [HIX-174244](docs/ms-telex-ui/24.3/HIX/HIX-174244.md)
- [HIX-174248](docs/ms-telex-ui/24.3/HIX/HIX-174248.md)
- [HIX-174250](docs/ms-telex-ui/24.3/HIX/HIX-174250.md)
- [HIX-174252](docs/ms-telex-ui/24.3/HIX/HIX-174252.md)