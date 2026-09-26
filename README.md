# Hi, I'm Miguel 👋

Full stack developer from Santiago, Chile, and Computer Engineer (Universidad Andrés Bello, 2025). React, Next.js and TypeScript up front; databases, APIs, auth and cloud behind them.

I do my best work on messy integrations: external APIs that can't be trusted, legacy systems that have to keep running, and slow requests that need a real fix.

## What I'm building

### [Pulso](https://github.com/mbarradev-debug/pulso) · [live demo](https://pulso-cyan-zeta.vercel.app)

An API layer and dashboard over the Banco Central de Chile API. The upstream API responds in ISO-8859-1, returns `200 OK` with the error hidden in the body, and includes dates with no data that come back empty or as `0`. Pulso decodes the responses, detects errors in the body, filters out those phantom values and caches each indicator with its own fallback, so one broken series doesn't take the others down.

Parallel upstream calls plus caching took responses from **~19s to ~0.23s**. Tested with Vitest and Playwright, CI on GitHub Actions.

### [Pulso for Chrome](https://chromewebstore.google.com/detail/pulso-uf-y-d%C3%B3lar/opakpmmcepebnccjjkhkgioopeadgihp?hl=es-419)

The UF, the dollar and other Chilean indicators one click away, served by the Pulso API. Published on the Chrome Web Store. Built with WXT, React and TypeScript.

## Things I've shipped

- **DOM Digital** · Forcast: SaaS for municipal construction permits, built from scratch to replace a Microsoft Project workflow. I owned the architecture, database design and full backend, and coordinated an intern.
- **E-Hive** · Forcast: scan a QR code, verify the license plate, start charging the car. Built solo in Angular on top of Dockerized microservices.
- **iSalud** · Valuesite: modernized the virtual branch used by 18,000+ members of Codelco's Isapre, migrating critical legacy flows and adding ASP.NET MVC endpoints over Oracle PL/SQL.
- **Ewreka** (internship): shipped features for a Flutter mobile app with the team.

## How I work

- **A `200 OK` is not proof of success.** I validate the body and give each piece of data its own fallback.
- **Measure before optimizing.** A speedup only counts if you timed the "before".
- **End-to-end tests where failure is expensive.** Playwright for critical flows, fast unit tests for parsing logic that's easy to get wrong.
- **Schema first, screens later.** The data model is the hardest thing to change afterwards.

## Stack

- **Frontend:** React, Next.js, TypeScript, Tailwind CSS, Angular
- **Backend:** Node.js, NestJS, ASP.NET MVC
- **Data & auth:** PostgreSQL, Oracle PL/SQL, Supabase, Firebase Auth
- **Cloud & tooling:** Azure, GCP, Vercel, Docker, GitHub Actions
- **Testing:** Vitest, Playwright · **Mobile:** Flutter, Ionic

## Off the clock

I read a bit of everything, from Agatha Christie to Japanese cozy novels. I also listen to all kinds of music; lately it's a lot of Los Tres. And I spend more time than I should tuning my setup: a [LazyVim config](https://github.com/mbarradev-debug/lazyvim-config), tmux, a [Solarized theme with the contrast fixed](https://github.com/mbarradev-debug/solarized-dark-contrast) and a [script that sets up a new Mac from zero](https://github.com/mbarradev-debug/macos-dev-setup-scripts).

## Contact

[miguelbarra.cl](https://miguelbarra.cl) · [LinkedIn](https://www.linkedin.com/in/miguelbarrarios) · [mbarra.git@gmail.com](mailto:mbarra.git@gmail.com)
