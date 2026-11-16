<p align="center">
  <a href="https://endorium.space">
    <img src="https://raw.githubusercontent.com/Endorium-Group/EndoriumFort-CE/master/assets/logo-full-blue.png" alt="EndoriumFort" height="72">
  </a>
</p>

<p align="center">
  <b>Privileged access you host yourself.</b><br>
  EndoriumFort is a sovereign PAM bastion: one audited gateway between your people and your infrastructure.
</p>

<p align="center">
  <a href="https://endorium.space">Website</a> ·
  <a href="https://endorium.space/docs/">Documentation</a> ·
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/releases">Releases</a> ·
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/discussions">Discussions</a>
</p>

<p align="center">
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/releases"><img src="https://img.shields.io/github/v/release/Endorium-Group/EndoriumFort-CE?style=flat-square&label=release" alt="Latest release"></a>
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/Endorium-Group/EndoriumFort-CE/ci.yml?branch=master&label=CI&style=flat-square" alt="CI"></a>
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/actions/workflows/codeql.yml"><img src="https://img.shields.io/github/actions/workflow/status/Endorium-Group/EndoriumFort-CE/codeql.yml?branch=master&label=CodeQL&style=flat-square" alt="CodeQL"></a>
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-source--available-orange?style=flat-square" alt="License"></a>
</p>

---

Operators shouldn't carry admin passwords and SSH keys around. With EndoriumFort they
sign in once, open a session from the browser, and the bastion does the rest: it injects
credentials from its vault, applies your rules, and writes every action to a hash-chained
audit log. No SaaS control plane, no license server, and it runs fine air-gapped.

```bash
docker run -d -p 80:80 ghcr.io/endorium-group/endoriumfort:latest
```

Then open `http://localhost`. The [quick start](https://github.com/Endorium-Group/EndoriumFort-CE#quick-start)
covers Compose, building from source and production setups.

### Activity

<p align="center">
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE/commits/master">
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=NergYR&theme=github-compact&hide_border=true&area=true" alt="Contribution activity" width="100%">
  </a>
</p>

<p align="center">
  <a href="https://github.com/Endorium-Group/EndoriumFort-CE"><img src="https://github-readme-stats.vercel.app/api/pin/?username=Endorium-Group&repo=EndoriumFort-CE&hide_border=true" alt="EndoriumFort CE"></a>
  <a href="https://github.com/Endorium-Group/EndoriumSpace"><img src="https://github-readme-stats.vercel.app/api/pin/?username=Endorium-Group&repo=EndoriumSpace&hide_border=true" alt="EndoriumSpace"></a>
</p>

<p align="center">
  <a href="https://star-history.com/#Endorium-Group/EndoriumFort-CE&Date">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Endorium-Group/EndoriumFort-CE&type=Date&theme=dark">
      <img src="https://api.star-history.com/svg?repos=Endorium-Group/EndoriumFort-CE&type=Date" alt="Star history" width="600">
    </picture>
  </a>
</p>

### The ecosystem

| Project | Role | Status |
|---|---|---|
| **[EndoriumFort CE](https://github.com/Endorium-Group/EndoriumFort-CE)** | The bastion itself: web SSH, HTTP proxy, remote browser isolation, vault, MFA, audit. C++ backend, React console. | Public |
| **EndoriumFort DrawBridge** | Local Go agent that tunnels native clients (RDP, raw TCP) through the bastion, with `endoriumfort://` deep links. | Enterprise |
| **EndoriumFort Bird** | Mobile companion: approve access requests from a push notification, TOTP and passkey authenticator. | In development |
| **[EndoriumSpace](https://github.com/Endorium-Group/EndoriumSpace)** | [endorium.space](https://endorium.space): product site, docs, community Q&A, sizing calculator. | Public |

### Editions

The **Community Edition** is source-available and free for personal, educational, research
and internal non-production use. The **Enterprise Edition** adds RDP/VNC, Kubernetes shells,
session recording, just-in-time access, SIEM export and HA, with licenses verified fully
offline. The split is documented in [OPEN-CORE.md](https://github.com/Endorium-Group/EndoriumFort-CE/blob/master/docs/OPEN-CORE.md).

### Also from Endorium

- [EndoriumNetworkingTool](https://github.com/Endorium-Group/EndoriumNetworkingTool): visual configuration for Kea DHCP and BIND DNS
- [EndoriumUtils](https://github.com/Endorium-Group/EndoriumUtils): the small Python library (logging, versions, config) our tools share

### Get involved

Found a bug or want a feature? [Open an issue](https://github.com/Endorium-Group/EndoriumFort-CE/issues/new/choose).
Questions about deploying it go to [Discussions](https://github.com/Endorium-Group/EndoriumFort-CE/discussions).
Security reports go through a [private advisory](https://github.com/Endorium-Group/EndoriumFort-CE/security/advisories/new), never a public issue.

For Enterprise licensing or anything else: **contact@endorium.space**

### Team

<table>
  <tr>
    <td align="center"><a href="https://github.com/NergYR"><img src="https://github.com/NergYR.png?size=120" width="80" alt="NergYR"><br><b>NergYR</b></a><br><sub>Creator, lead developer</sub></td>
    <td align="center"><a href="https://github.com/BluenessDev"><img src="https://github.com/BluenessDev.png?size=120" width="80" alt="BluenessDev"><br><b>BluenessDev</b></a><br><sub>Releases</sub></td>
    <td align="center"><a href="https://github.com/sohukia"><img src="https://github.com/sohukia.png?size=120" width="80" alt="sohukia"><br><b>sohukia</b></a><br><sub>Contributor</sub></td>
  </tr>
</table>

Want your name here? Start with a [good first issue](https://github.com/Endorium-Group/EndoriumFort-CE/issues) or a pull request.
