# rustatio-core

Core library for the Rustatio BitTorrent ratio management tool.

## Configuration

The core reads its configuration from a TOML file. An annotated example
configuration is provided in [`config.example.toml`](./config.example.toml)
in this directory.

Copy that file to one of the following locations and adjust the values
to match your environment:

| OS | Path |
|----|------|
| Linux / macOS | `~/.config/rustatio/config.toml` |
| Windows | `%APPDATA%\rustatio\config.toml` |

## Crate structure

- `src/config.rs` — TOML deserialization and default values
- `src/faker.rs` — tracker announce loop and stat simulation
- `src/client/` — per-client peer ID, user-agent, and protocol logic
- `src/tracker.rs` — HTTP announce/ scrape parsing

## License

MIT — see the top-level `LICENSE` file.
