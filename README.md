# Vite TypeScript Starter Template

A starter template for [bolt.diy](https://github.com/stackblitz-labs/bolt.diy).

## Purpose

This template is designed for use with **<https://github.com/stackblitz-labs/bolt.diy>**. bolt.diy fetches
these files at runtime and imports them into a fresh WebContainer project when you ask for a Vite + TypeScript
project, so everything here needs to install and build with no extra setup.

Modified by [Dustin Loring](https://github.com/Dustinwloring1988) (Dustinwloring1988) in October 2026.

## Stack

| Package | Version |
| --- | --- |
| Vite | ^8.3.4 |
| TypeScript | ^7.0.2 |

Node 20 or newer is required.

## Commands

```bash
npm install   # install dependencies
npm run dev   # vite — dev server
npm run build # tsc && vite build — type-check then build
npm run preview # vite preview — local preview server
```

## About this template

A Vite project with TypeScript strict mode. The build script runs `tsc` first for type checking, then
`vite build` for production output. `main.ts` is the default entry point.

## Upgraded to Vite 8, TypeScript 7.0.2 (October 2026)

Moved from Vite 5 and TypeScript ~5.5. Vite was upgraded stepwise (5→6→7→8) and verified with `npm install`
and `npm run build` after each step. TypeScript was upgraded from ~5.5.0 to ^7.0.2.

TypeScript 7.0.2 is the bare `tsc` variant — no `svelte-check` or `typescript-eslint` constraints apply,
so the latest major is used. All other templates in this org target TS ~6.0.3 to satisfy Angular,
React Router, and svelte-check peer ranges.

Tailwind CSS and ESLint were also updated to their latest Vite 8-compatible versions (Tailwind 4.3.3,
ESLint 10).

## Verification

- `npm install` and `npm run build` pass without errors
- The `tsc` type-check step completes successfully
- `npm run preview` serves the production build locally