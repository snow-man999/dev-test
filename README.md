# Nomey Web App
This is the official repository for the Nomey web app, built on the T3 Stack with custom extensions.

## Tech Stack

- [Next.js](https://nextjs.org) - App Framework
- [NextAuth.js](https://next-auth.js.org) - Authentication
- [Prisma](https://prisma.io) - Database ORM
- [Tailwind CSS](https://tailwindcss.com) - CSS Utility Framework
- [tRPC](https://trpc.io) - API Framework
- [Mux]() - Video handling (upload / storage / etc.)
- [tolgee](https://tolgee.io/) - Translation Management
- [Meilisearch](https://www.meilisearch.com/) - Full-text search
- [Upstash](https://upstash.com/) Next compatible redis
- [Qstash](https://upstash.com/docs/qstash) Next compatible queue handling 
- [Vitest](https://vitest.dev/) - Testing Framework

## Testing

This project uses [Vitest](https://vitest.dev/) to run both client-side (browser) and server-side (Node.js) tests.

### Project Structure

Tests are split into two environments:

- **Browser (jsdom)** — for React/browser environment tests.
- **Node.js** — for backend and server-only logic.

### File Naming Conventions

- Node-specific tests: `*.node.test.ts`
- Browser tests: any other `*.test.ts`, `*.test.tsx`, etc.

### Running Tests

Run **all tests**:

```bash
npm run test
```

## Local Development

### Clone and Install
```bash
git clone git@github.com:nomeyy/nomey-next.git
cd nomey-next
npm install
```

### Run Containers

You'll need to have `docker` installed locally. We advise running `./scripts/start-services.sh` to safely start your environment, but a normal docker workflow will also work.

### Run Next

```bash
npm run dev
```

> ⚠️ **Warning:** The T3 stack hard-enforces environment variables to provide type-safety. The project will not build without all environment variables in place. Contact a dev to get their variables to quickly get yourself up and running.

## Learn More

 - [Nomey Documentation (WIP)](https://nomey.mintlify.app/)
 - [Next Documentation](https://nextjs.org/docs)
 - [T3 Stack Documentation](https://create.t3.gg/en/usage/first-steps)
 - [Mux Documentation](https://www.mux.com/docs)

`If you have some question in this project, feel free to reach out.`
