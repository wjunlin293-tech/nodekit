# NodeKit

Dead-simple proxy subscription to Clash config converter.

## What

Paste your airport subscription URL → get a ready-to-use Clash YAML config in 10 seconds.

No more hand-editing YAML files.

## Usage

```bash
python3 nodekit.py --url "your_subscription_url" -o config.yaml
```

Then import `config.yaml` into Clash / Clash Verge / any Clash client.

## Example

```bash
$ python3 nodekit.py --url "https://example.com/sub?token=xxx" -o config.yaml
📡 Fetching subscription...
📦 Downloaded 1234 bytes
✅ Parsed 8 SS nodes
   • Hong Kong (1.2.3.4:8388)
   • Tokyo (5.6.7.8:8388)
   • Singapore (9.10.11.12:8388)
   ...
💾 Config saved to config.yaml
```

## Requirements

- Python 3.7+
- Zero dependencies (stdlib only)

## Supported Protocols

| Protocol | Status |
|----------|--------|
| SS (Shadowsocks) | ✅ Supported |
| VMess | 🚧 Planned |
| Trojan | 🚧 Planned |
| Hysteria2 | 🚧 Planned |

## Why

Clash stopped updating. Surge costs $50. Existing tools are either too complex or abandoned.

NodeKit is the zero-config alternative.

## Roadmap

- [ ] GUI version with speed test
- [ ] Multi-subscription management
- [ ] Rule template market
- [ ] Auto node selection

## License

MIT
