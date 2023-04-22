# Vite + React + Module Federation PoC

Quick and simple PoC for module federation with react and vite,
Uses [vite-plugin-federation](https://github.com/originjs/vite-plugin-federation) for module federation.

## Setup

I've used `pnpm` as the package manager, use `npm i -g pnpm` to install the latest version of pnpm

- `pnpm setup-project` to install dependencies in host & remote app
- `pnpm serve:all` to build and preview the applications
- open [http://127.0.0.1:5050](http://127.0.0.1:5050) to see the host application

### Notes

Currently the dev server doesn't work with module federation as of `vite-plugin-federation 1.2.2`

Ref: [vite-plugin-federation#204](https://github.com/originjs/vite-plugin-federation/issues/204)

Hence the use of the combination of `build --watch` and `preview`
