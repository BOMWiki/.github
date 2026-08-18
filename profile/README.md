<div align="center">

<pre>
██████╗  ██████╗ ███╗   ███╗██╗    ██╗██╗██╗  ██╗██╗
██╔══██╗██╔═══██╗████╗ ████║██║    ██║██║██║ ██╔╝██║
██████╔╝██║   ██║██╔████╔██║██║ █╗ ██║██║█████╔╝ ██║
██╔══██╗██║   ██║██║╚██╔╝██║██║███╗██║██║██╔═██╗ ██║
██████╔╝╚██████╔╝██║ ╚═╝ ██║╚███╔███╔╝██║██║  ██╗██║
╚═════╝  ╚═════╝ ╚═╝     ╚═╝ ╚══╝╚══╝ ╚═╝╚═╝  ╚═╝╚═╝
</pre>

**The free encyclopedia of what things are made of.**

Open-source BOM (bill of materials) knowledge and browser CAD tools.

[![License: AGPL-3.0](https://img.shields.io/github/license/BOMWiki/bomwiki?style=flat-square&color=blue)](https://github.com/BOMWiki/bomwiki/blob/main/LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/BOMWiki/bomwiki?style=flat-square)](https://github.com/BOMWiki/bomwiki/commits/main)
[![Runtime dependencies](https://img.shields.io/badge/runtime_deps-3-blue?style=flat-square)](https://github.com/BOMWiki/bomwiki/blob/main/package.json)
![No framework](https://img.shields.io/badge/framework-none-success?style=flat-square)
![Node](https://img.shields.io/badge/node-%E2%89%A5%2022-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square)](https://github.com/BOMWiki/bomwiki/blob/main/CONTRIBUTING.md)

[**bomwiki.com**](https://bomwiki.com) · [Policies](https://bomwiki.com/policies) · [Governance](https://bomwiki.com/about/governance) · [Verification](https://bomwiki.com/about/verification)

</div>

---

[bomwiki.com](https://bomwiki.com) is a free, openly editable encyclopedia of bills of materials: what products are made of, exploded down to individual parts. Every page is versioned, every change is attributed and reviewed, and every product links to the shared parts it is built from.

```text
cordless-drill
├─ motor-assembly ×1
│  ├─ brushless-motor ×1
│  └─ planetary-gearbox ×1
├─ battery-pack ×1
│  └─ 18650-cell ×5
├─ keyless-chuck ×1
└─ housing-shell ×2
```

Sub-assemblies are shared: the same bearing or Li-ion cell is one node that appears on every product that uses it. The catalog is one graph.

## Projects

- **[bomwiki](https://github.com/BOMWiki/bomwiki):** the public AGPL-3.0 wiki-engine source set used within bomwiki.com. Node.js and Postgres, no web framework, three runtime dependencies (`pg`, `marked`, `sanitize-html`). It is an allowlisted reading mirror for review and contributions, not a complete standalone checkout; private production integrations are omitted.
- **[PartMode](https://github.com/BOMWiki/partmode):** open-source, local-first 3D parametric CAD that runs in the browser, powered by OpenCascade WASM. Try it at [partmode.com](https://partmode.com/).
- **BOM Intelligence:** the analysis engine that reviews every proposed change. Closed source, but [its interface is documented](https://bomwiki.com/intelligence) so any instance can supply its own analyzer.

## Contributing

- **Fix the content:** open an account on [bomwiki.com](https://bomwiki.com) and click Edit on any page. New contributors' changes are reviewed; trust is earned. See the [policies](https://bomwiki.com/policies).
- **Improve the public engine:** review the source and propose changes on [BOMWiki/bomwiki](https://github.com/BOMWiki/bomwiki). The mirror is not a complete standalone service, so read its [scope](https://github.com/BOMWiki/bomwiki#readme) and [CONTRIBUTING guide](https://github.com/BOMWiki/bomwiki/blob/main/CONTRIBUTING.md) first.
- **Report security issues:** privately, to [admin@bomwiki.com](mailto:admin@bomwiki.com). See [SECURITY](https://github.com/BOMWiki/bomwiki/blob/main/SECURITY.md).

## How the site is run

Founder-led, with open contribution and transparent machinery: [governance](https://bomwiki.com/about/governance) · [how verification works](https://bomwiki.com/about/verification).
