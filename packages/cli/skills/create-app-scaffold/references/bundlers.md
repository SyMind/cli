# Bundler Options

Targets `@tanstack/cli` v0.71.0.

## Supported values

- `vite` (default)
- `rsbuild`

## Usage

```bash
npx @tanstack/cli create app --framework react --bundler vite -y
npx @tanstack/cli create app --framework solid --bundler rsbuild -y
```

Rsbuild supports full TanStack Start and router-only projects, including the
standard and `--blank` presets, built-in example pages, Tailwind, ESLint, and
Biome. It does not currently support templates, deployment adapters, or
catalog business/example add-ons. `tanstack add` is limited to ESLint/Biome in
Rsbuild projects.

Use the bundler-aware catalog view before constructing an Rsbuild command:

```bash
npx @tanstack/cli create --list-add-ons --bundler rsbuild --json
```
