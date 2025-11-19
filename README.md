<div align="center">
  <img width="840" alt="RUST banner" src="./assets/banner.svg" />
  <br/>
  <strong>Tagline:</strong> Actions‑First CI/CD & Pipeline Hub for Rust and beyond.
  <!-- if you’re reading this you’re officially part of the conspiracy -->
</div>

<p align="center">
  <a href="https://img.shields.io/github/actions/workflow/status/Snapwave333/RUST/test.yml?branch=main"><img alt="Build" src="https://img.shields.io/github/actions/workflow/status/Snapwave333/RUST/test.yml?branch=main&label=tests" /></a>
  <a href="https://img.shields.io/github/actions/workflow/status/Snapwave333/RUST/security.yml?branch=main"><img alt="Security" src="https://img.shields.io/github/actions/workflow/status/Snapwave333/RUST/security.yml?branch=main&label=security" /></a>
  <a href="https://img.shields.io/github/actions/workflow/status/Snapwave333/RUST/release.yml?branch=main"><img alt="Release" src="https://img.shields.io/github/actions/workflow/status/Snapwave333/RUST/release.yml?branch=main&label=release" /></a>
  <a href="./LICENSE"><img alt="License" src="https://img.shields.io/badge/License-MIT-blue" /></a>
</p>

<p align="center">
  <img alt="Rust" height="26" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rust/rust-plain.svg" />
  <img alt="GitHub Actions" height="26" src="https://img.shields.io/badge/Actions-CI%2FCD-%23181717?logo=github" />
  <img alt="Docker" height="26" src="https://img.shields.io/badge/Docker-Container-%232496ED?logo=docker" />
</p>

## Quick Overview

This repository hosts production‑grade GitHub Actions workflows and documentation for CI/CD, security, releases, containers, rollback, and benchmarks. It is designed to be code‑agnostic until you add a Rust crate or other application.

## Workflows

- Test & Coverage: `.github/workflows/test.yml`
- Security: `.github/workflows/security.yml`
- Release (staging/production): `.github/workflows/release.yml`
- Container (GHCR): `.github/workflows/container.yml`
- Rollback (GHCR retag): `.github/workflows/rollback.yml`
- Benchmarks (Criterion): `.github/workflows/benchmarks.yml`

## Environments & Secrets

- Environments: create `staging` and `production` with required reviewers in repo settings.
- Secrets:
  - `CODECOV_TOKEN` (repository secret)
  - `SLACK_WEBHOOK_URL` (environment secrets for staging and production)

## Usage

- Push to `develop` or open a PR → triggers Test/Security
- Create `release-*` branch → staging prerelease
- Tag `v*` → production release; optional container build if a Dockerfile exists

## Documentation

See `docs/ci-cd.md` for the complete pipeline overview.

## Notes

- No placeholder assets are used. Banner SVG is procedurally generated and versioned.
- Demo media is not applicable here until application code exists.

<details>
  <summary>Hidden delight</summary>
  <p>If you read this line, you gain +5 developer XP. The owl knows.</p>
  <p><a href="#">.</a></p>
</details>
