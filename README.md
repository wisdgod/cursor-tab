# Cursor Tab Protocol Buffers

A reverse-engineered Protocol Buffers definition project that enables Cursor Tab functionality for other platforms.

## Overview

This project provides Protocol Buffers definitions for integrating Cursor Tab features into third-party applications and platforms through reverse engineering efforts.

**Current Version**: 3.13.10

> **Important Notice**
> 
> - This project is based on reverse engineering
> - Updates are provided on an irregular basis
> - The project may be discontinued at any time without notice

## Branches

| Branch | Description |
|--------|-------------|
| `main` | Core protocol definitions — contains only the essential `.proto` files directly related to Cursor Tab functionality |
| `extracted` | **Complete extraction** — contains the full set of `.proto` files recovered from reverse engineering, including all internal services, agent tools, AI server interfaces, and supporting definitions (170 files across 6 directories) |

> **Which branch should I use?**
>
> - If you only need Cursor Tab integration → use `main`
> - If you need the full protocol surface (agent, aiserver, anyrun, internapi, etc.) → use `extracted`

## Installation

```bash
# Clone the repository
git clone https://github.com/wisdgod/cursor-tab.git
cd cursor-tab

# For core definitions only (default)
git checkout main

# For the complete set of extracted protocol files
git checkout extracted
```

## Usage

Choose a Protocol Buffers library for your preferred programming language and compile the `.proto` files according to your language's documentation.

### Extracted Branch Structure

```
.
├── agent/v1/          # Agent service, tools, and execution protocols
├── aiserver/v1/       # AI server interfaces (chat, composer, fastapply, etc.)
├── anyrun/v1/         # Dev container and pod management
├── google/protobuf/   # Standard Google protobuf dependencies
└── internapi/v1/      # Internal API definitions
```

## License

This project is dual-licensed under:

- [MIT License](LICENSE-MIT)
- [Apache License 2.0](LICENSE-APACHE)

You may choose either license for your use case.

## Contributing

While Pull Requests are not accepted, you are welcome to report issues or suggestions through GitHub Issues.

## Disclaimer

**This is an unofficial, independently maintained project produced entirely through reverse engineering. It is not affiliated with, endorsed by, sponsored by, or in any way officially connected to Anysphere Inc. or the Cursor product.**

By using the contents of this repository, you acknowledge and agree that:

- **No Warranty**: All protocol definitions are provided "AS IS" without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, or non-infringement.
- **Accuracy Not Guaranteed**: The definitions may be incomplete, inaccurate, or outdated. They are derived from reverse engineering and may not reflect the actual or current state of any service.
- **Use at Your Own Risk**: The maintainers assume no liability for any damages, losses, account restrictions, service disruptions, or other consequences arising from the use or misuse of these files.
- **Legal Responsibility**: Users are solely responsible for ensuring that their use of this project complies with all applicable laws, regulations, and terms of service. Reverse engineering and interoperability laws vary by jurisdiction.
- **No Support Obligation**: Support is provided on a best-effort basis only. There is no guarantee of continued maintenance, updates, or responses to issues.
- **Subject to Removal**: This project may be modified, archived, or removed at any time without prior notice.

## Support

As this is a reverse-engineered project with irregular updates, support is provided on a best-effort basis through [GitHub Issues](https://github.com/wisdgod/cursor-tab/issues).
