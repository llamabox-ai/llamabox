# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in LlamaBox, **please do not open a public issue**.

Instead, send the details via email to:

**aalhad.dev@gmail.com**

Include as much of the following as possible:
- A clear description of the vulnerability
- Steps to reproduce
- Affected versions / build numbers
- Potential impact
- Any suggested mitigations

PGP encryption is optional; if you would like to use it, mention it in your initial email and we will provide a key.

We aim to acknowledge receipt within **72 hours** and will keep you informed as we investigate.

## Scope

This policy covers:
- The LlamaBox Android application (`com.llamabox`)
- This repository and any related public repositories under the `llamabox-ai` GitHub organization
- Build scripts, CI/CD configurations, and release artifacts

## Privacy & Data Collection Notes

LlamaBox performs **all inference on-device** via llama.cpp and collects **no user data** by design. There are no cloud accounts, telemetry endpoints, or remote model servers. Consequently, many classes of traditional "privacy" concerns (e.g., server-side data leaks) do not apply.

That said, if you identify a way that local data (chat history, imported models, images) could be exposed or leaked outside the app boundary, that is still a valid and welcome security report.

## Supported Versions

Only the **latest closed-beta build** is actively supported with security fixes. If you are running an older side-loaded APK, please update to the most recent release before reporting.
