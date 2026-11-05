# pi-skill-handoff

[![Pi Package](https://img.shields.io/badge/pi--package-skill-blue)](https://github.com/IgorGuariroba/pi-skill-handoff)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**handoff** skill for the **[Pi coding agent](https://pi.dev)**, adapted from Matt Pocock's Engineering Skills.

> Compact the current conversation into a handoff document for another agent to pick up.

---

## Installation

Install directly into Pi using `pi install`:

```bash
pi install git:github.com/IgorGuariroba/pi-skill-handoff
```

Or clone into your local/global skills directory:

```bash
# Global Pi skills directory:
git clone https://github.com/IgorGuariroba/pi-skill-handoff.git ~/.pi/agent/skills/handoff

# Or Agent Skills standard path:
git clone https://github.com/IgorGuariroba/pi-skill-handoff.git ~/.agents/skills/handoff
```

---

## Usage

Trigger it explicitly in your session:

```text
/skill:handoff
```

Or let Pi automatically route to it based on conversation context and need.

---

## Credits

- **Original concept & methodology**: [Matt Pocock](https://github.com/mattpocock)
- **Adapted for Pi Agent**: [Igor Guariroba](https://github.com/IgorGuariroba)

---

## License

[MIT](LICENSE)
