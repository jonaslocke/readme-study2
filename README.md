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

---

# Table of Contents

## Best Practices

- [Code Reviews](docs/Best%20Practices/Code%20Reviews/Intro.md)
- [JIRA](docs/Best%20Practices/JIRA/Intro.md)
- [Redux Toolkit](docs/Best%20Practices/Redux%20Toolkit/Intro.md)
- [Typescript](docs/Best%20Practices/Typescript/Intro.md)
- [Unit Tests - Jest](docs/Best%20Practices/Unit%20Tests%20-%20Jest/Intro.md)
- [Using Nx](docs/Best%20Practices/Using%20Nx/Intro.md)

## Development Best Practices

- [Coding Best Practices](docs/Development-Best-Practices/Coding-Best-Practices.md)
- [Performance Optimization](docs/Development-Best-Practices/Performance-Optimization.md)

## IEX

- [Introduction](docs/IEX/intro.md)
- [project-structure](docs/IEX/project-structure.md)

## 24.3

- [HIX-174068](docs/24.3/Tickets/HIX-174068.md)
- [HIX-174077](docs/24.3/Tickets/HIX-174077.md)
- [HIX-174204](docs/24.3/Mobile-Upload-Using-QR-Code/HIX-174204.md)
- [Overview](docs/24.3/ms-telex-ui/Overview.md)
- [Adhoc Notices](docs/24.3/ms-telex-ui/Components/AdhocNotices.md)
- [Failed Table](docs/24.3/ms-telex-ui/Components/FailedTable.md)
- [Notice Full Summary](docs/24.3/ms-telex-ui/Components/NoticeFullSummary.md)
- [Notices Summary](docs/24.3/ms-telex-ui/Components/NoticesSummary.md)
- [Pane Container](docs/24.3/ms-telex-ui/Components/PaneContainer.md)
- [Search Filter](docs/24.3/ms-telex-ui/Components/SearchFilter.md)
- [Widget](docs/24.3/ms-telex-ui/Components/Widget.md)
- [HIX-174231](docs/24.3/ms-telex-ui/HIX/HIX-174231.md)
- [HIX-174237](docs/24.3/ms-telex-ui/HIX/HIX-174237.md)
- [HIX-174239](docs/24.3/ms-telex-ui/HIX/HIX-174239.md)
- [HIX-174244](docs/24.3/ms-telex-ui/HIX/HIX-174244.md)
- [HIX-174248](docs/24.3/ms-telex-ui/HIX/HIX-174248.md)
- [HIX-174250](docs/24.3/ms-telex-ui/HIX/HIX-174250.md)
- [HIX-174252](docs/24.3/ms-telex-ui/HIX/HIX-174252.md)

## Tools

- [Charting Libraries](docs/Tools/Charting%20Libraries/Introduction.md)
- [NPM-Registry-Proxy](docs/Tools/NPM-Registry-Proxy/Intro.md)
