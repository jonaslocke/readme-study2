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

- [QR code mobile upload](docs/24.3/Mobile-Upload-Using-QR-Code/HIX-174204.md)
- [Telex](docs/24.3/ms-telex-ui/Overview.md)
- [HIX-174068](docs/24.3/Tickets/HIX-174068.md)
- [HIX-174077](docs/24.3/Tickets/HIX-174077.md)

## Tools

- [Charting Libraries](docs/Tools/Charting%20Libraries/Introduction.md)
- [NPM-Registry-Proxy](docs/Tools/NPM-Registry-Proxy/Intro.md)
