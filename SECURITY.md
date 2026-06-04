# Security Policy

## Supported Versions

The latest release of Rustatio (the commit on the `main` branch) is the
only version that currently receives security updates. Older releases
will not be patched — please update to the latest version.

## Reporting a Vulnerability

If you discover a security vulnerability in Rustatio, **please do not
open a public GitHub issue**. Instead, report it privately to the
maintainer:

- **GitHub:** [takitsu21](https://github.com/takitsu21) (open a private
  vulnerability report through GitHub Security Advisories at
  https://github.com/takitsu21/rustatio/security/advisories/new)

You should receive an acknowledgement within 72 hours. The maintainer
will work with you on a fix and a coordinated disclosure timeline.

## Scope

In-scope issues include:

- Authentication bypass on the self-hosted web UI (`AUTH_TOKEN`)
- Remote code execution via the BitTorrent tracker interface
- Information disclosure of user tokens or local data
- Supply-chain issues (compromised dependencies)

Out-of-scope issues:

- Issues affecting the WebAssembly build of the web app where the
  underlying Rust code is unchanged
- Reports about the educational nature of the tool itself (see
  the README warning)

## Safe Use

Rustatio is intended for **educational and research purposes only**
and should not be used against trackers without authorization.
Misuse is the sole responsibility of the user.
