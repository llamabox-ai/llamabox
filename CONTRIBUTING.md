# Contributing to LlamaBox

Thank you for your interest in LlamaBox! This document explains how you can get involved.

## Project Status

LlamaBox is currently in **closed beta** on Google Play. The full source code will be opened to the public soon under a dual-license model. If you would like to be notified the moment the source is published, please **star and watch** this repository.

## How to Contribute (once the repo is public)

1. **Fork** the repository.
2. **Create a branch** for your change: `git checkout -b feat/your-feature-name` or `fix/your-bug-description`.
3. **Make your changes**, following the code-style notes below.
4. **Commit** using [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat:` new feature
   - `fix:` bug fix
   - `docs:` documentation only
   - `style:` formatting, missing semi-colons, etc.
   - `refactor:` code change that neither fixes a bug nor adds a feature
   - `perf:` performance improvement
   - `test:` adding or correcting tests
   - `chore:` build process or auxiliary tool changes
5. **Open a Pull Request** against the `main` branch with a clear description of the problem and solution.

## Contributor License Agreement

> **Important:** Because LlamaBox is **dual-licensed** (AGPL-3.0 for open-source use and a separate commercial license for closed-source commercial use), every contributor must sign a **Contributor License Agreement (CLA)**. The CLA grants the project the right to re-license your contribution under both licenses.
>
> Until a CLA bot (e.g., CLA Assistant) is wired up, **incoming contributions will be held** pending manual CLA verification.
>
> **TODO:** Add CLA Assistant (or equivalent) integration and the exact CLA text before the public source release.

## Code Style

- **Match the surrounding code.** Consistency within a file matters more than strict global rules.
- **TypeScript** is used throughout; avoid implicit `any`.
- **React Native `Animated` only** — we do not use Reanimated because it crashes under the New Architecture in our setup.
- **Zustand** for state management; keep stores small and focused.
- **Expo FileSystem v19** patterns preferred (`FileSystem.File` / `FileSystem.Directory`) except where legacy `copyAsync` is explicitly required.
- Run the existing lint rules (`eslint`, `prettier`) before pushing.

## Reporting Bugs

- Search existing [Issues](../../issues) first to avoid duplicates.
- Open a new issue with a clear title, reproduction steps, and your device / Android version.
- For crash reports, include relevant logs if possible.

## Reporting Security Issues

**Do not open a public issue for security vulnerabilities.**

Please see [SECURITY.md](./SECURITY.md) for our responsible disclosure policy and contact instructions.

## Community Standards

All contributors are expected to adhere to our [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md). Be kind, be patient, and be welcoming.
