<div align="center">

<br/>

<pre>
 ░█████╗░░██████╗░███████╗███╗░░██╗████████╗
 ██╔══██╗██╔════╝░██╔════╝████╗░██║╚══██╔══╝
 ███████║██║░░██╗░█████╗░░██╔██╗██║░░░██║░░░
 ██╔══██║██║░░╚██╗██╔══╝░░██║╚████║░░░██║░░░
 ██║░░██║╚██████╔╝███████╗██║░╚███║░░░██║░░░
 ╚═╝░░╚═╝░╚═════╝░╚══════╝╚═╝░░╚══╝░░░╚═╝░░░

 ░█████╗░███████╗███████╗██╗░█████╗░███████╗
 ██╔══██╗██╔════╝██╔════╝██║██╔══██╗██╔════╝
 ██║░░██║█████╗░░█████╗░░██║██║░░╚═╝█████╗░░
 ██║░░██║██╔══╝░░██╔══╝░░██║██║░░██╗██╔══╝░░
 ╚█████╔╝██║░░░░░██║░░░░░██║╚█████╔╝███████╗
 ░╚════╝░╚═╝░░░░░╚═╝░░░░░╚═╝░╚════╝░╚══════╝
</pre>

### A 3D office your team shares with its coding agents

*"Whatever you do, work heartily, as for the Lord and not for men."*
*— Colossians 3:23 (ESV)*

<br/>

[![Release](https://img.shields.io/github/v/release/MananShukla007/Manan-CLAUDE-OFFICE?style=for-the-badge&color=e8c547&label=release)](https://github.com/MananShukla007/Manan-CLAUDE-OFFICE/releases)&nbsp;[![Build](https://img.shields.io/github/actions/workflow/status/MananShukla007/Manan-CLAUDE-OFFICE/release.yml?style=for-the-badge&label=build)](https://github.com/MananShukla007/Manan-CLAUDE-OFFICE/actions)&nbsp;[![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)](LICENSE)&nbsp;[![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org)&nbsp;[![Platform](https://img.shields.io/badge/macOS%20%7C%20Linux%20%7C%20Windows-555555?style=for-the-badge)](#run-locally)

<br/>

</div>

```sh
curl -fsSL https://raw.githubusercontent.com/MananShukla007/Manan-CLAUDE-OFFICE/main/install.sh | bash
```

<div align="center">

[**Run locally**](#run-locally) · [**Deploy to AWS**](#deploy-to-aws-ec2) · [**Azure**](#deploy-to-azure) · [**Any server**](#deploy-to-any-ubuntu-or-debian-server) · [**Add users**](#add-users) · [**Controls**](#controls) · [**Features**](docs/features.md) · [**How it works**](docs/how-it-works.md)

</div>

---

<div align="center">

<pre>
  ╔══════════════════════════════════════════════════════════╗
  ║  🌤   ROOFTOP    Bar · Arcade · Office Dog 🐕            ║
  ╠══════════════════════════════════════════════════════════╣
  ║  🔧   FLOOR N    your-org / repo-c      🤖  🤖  🤖      ║
  ╠══════════════════════════════════════════════════════════╣
  ║  💡   FLOOR 2    your-org / repo-b      🤖  💻  ✅      ║
  ╠══════════════════════════════════════════════════════════╣
  ║  🚀   FLOOR 1    your-org / repo-a      🤖  ⌨️   ⏳      ║
  ╠══════════════════════════════════════════════════════════╣
  ║  🛗   LOBBY      Elevator · Chat · Voice · Whiteboard    ║
  ╚══════════════════════════════════════════════════════════╝
</pre>

<sub>Every GitHub repo is a floor. Every floor has desks for coding agents.</sub>

</div>

---

## What's inside

<table>
<tr>
<td width="50%" valign="top">

### 🗂️ One floor per project
Ride the elevator, pick one of your GitHub repos, and the office clones it and opens a floor for it. Every worker, board and queue on that floor works in that checkout.

</td>
<td width="50%" valign="top">

### 🤖 Workers at every desk
Walk up to an empty desk, press **E**, and hire Claude Code, Codex or OpenCode. The agent's live terminal shows on the laptop in front of it — anyone can open it and type.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔔 See who needs you
A worker waiting on input jumps up and down and dings. Press **N** to jump straight to the one that has waited longest.

</td>
<td width="50%" valign="top">

### 📋 GitHub on the walls
Issues and pull requests hang on cork boards. Hand an issue to a worker, queue tasks, give a worker its own git worktree and open its PR — all with one key.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔗 Cross-project tasks
One task can span several repos. Each worker gets a worktree of each, and a PR in each that links the others.

</td>
<td width="50%" valign="top">

### 👥 Together
Voice, chat, screen sharing on the lounge TV and a shared whiteboard. Plus a rooftop bar, an office dog and an arcade.

</td>
</tr>
</table>

There's a lot more — see [docs/features.md](docs/features.md).

---

## Requirements

On the machine that runs the office:

| | Requirement | Notes |
|:---:|---|---|
| ⚙️ | **Node.js 20+** | |
| 🤖 | **An agent CLI** | At least one of: `claude` (Claude Code), `codex`, or `opencode` — signed in as the user running the office. With [accounts](#add-users), everyone can sign in to their own Claude instead. |
| 🐙 | **git + GitHub CLI** | Run `gh auth login` — needed for cloning repos, the issue boards, and PR management. |

---

## Run locally

```bash
# macOS / Linux
curl -fsSL https://raw.githubusercontent.com/MananShukla007/Manan-CLAUDE-OFFICE/main/install.sh | bash
```

```powershell
# Windows (PowerShell)
irm https://raw.githubusercontent.com/MananShukla007/Manan-CLAUDE-OFFICE/main/install.ps1 | iex
```

This puts `Manan-CLAUDE-OFFICE` on your PATH. Run the install line again to update.

**First start** walks you through setup in the terminal:

```
  1 ──► Where to clone your projects   (suggests folders you already have, else ~/Manan-CLAUDE-OFFICE)
  2 ──► GitHub sign-in                 (offers to run gh auth login if not already done)
  3 ──► Your first project             (pick a repo by number, or type owner/name)
```

Then the office opens in your browser, already signed in, with a one-time link. The terminal also prints the office password (saved in `~/Manan-CLAUDE-OFFICE/.Manan-CLAUDE-OFFICE/config.json`).

**Common options:**

```bash
Manan-CLAUDE-OFFICE ~/code/my-project              # use an existing project as the first floor
Manan-CLAUDE-OFFICE --password 'correct horse'     # set the password
Manan-CLAUDE-OFFICE --port 4700                    # custom port
Manan-CLAUDE-OFFICE --agent codex                  # default agent: claude, codex or opencode
Manan-CLAUDE-OFFICE --no-open                      # print the sign-in link instead of opening a browser
Manan-CLAUDE-OFFICE setup                          # re-run first-start walkthrough (office stopped)
```

> [!NOTE]
> The office listens on `127.0.0.1` by default — only your machine can reach it. `--host 0.0.0.0` opens it to your network over plain HTTP (voice and screen sharing won't work). For team use, deploy to a server.

To run from a clone:

```bash
git clone https://github.com/MananShukla007/Manan-CLAUDE-OFFICE && cd Manan-CLAUDE-OFFICE
npm install       # also builds the client and server
npm install -g .  # puts Manan-CLAUDE-OFFICE on your PATH
Manan-CLAUDE-OFFICE
```

Every option is in [docs/configuration.md](docs/configuration.md). Model and provider config per worker is in [docs/agents.md](docs/agents.md).

---

## Deploy

<table>
<tr>
<th width="33%">☁️ AWS (EC2)</th>
<th width="33%">🔷 Azure</th>
<th width="33%">🖥️ Any Ubuntu / Debian</th>
</tr>
<tr>
<td valign="top">

Needs: **AWS CLI** signed in, `ssh`, `curl`, and a clone of this repo.

<pre>deploy/aws.sh up \
  --project owner/repo \
  --claude-token \
    "$(claude setup-token)"</pre>

Launches a **t3.xlarge** (4 vCPU, 16 GiB, 50 GiB disk), opens SSH only to your IP, and installs the office as a systemd service. Finishes in ~2 minutes.

<a href="docs/aws.md">Full reference →</a>

</td>
<td valign="top">

Needs: **Azure CLI** signed in, `ssh`, `curl`, and a clone of this repo.

<pre>deploy/azure.sh up \
  --project owner/repo \
  --claude-token \
    "$(claude setup-token)"</pre>

Launches a **Standard_D4as_v5** (4 vCPU, 16 GiB, 64 GiB Premium SSD), puts everything in its own resource group, static IP.

<a href="docs/azure.md">Full reference →</a>

</td>
<td valign="top">

Run one line on the server as root or sudo:

<pre>curl -fsSL \
  https://raw.githubusercontent.com/\
MananShukla007/Manan-CLAUDE-OFFICE/main/\
deploy/provision.sh | bash</pre>

Installs Node 22, git, `gh`, Claude Code, and the office as a systemd service. Add `--domain office.example.com` for HTTPS or `--tailscale` for Tailscale.

<a href="docs/self-hosting.md">Full reference →</a>

</td>
</tr>
</table>

### 🔒 On Tailscale — no tunnels needed

Add `--tailscale` to any deploy command. The machine joins your tailnet, Tailscale Serve puts the office on `https://Manan-CLAUDE-OFFICE.<tailnet>.ts.net` with a real cert. No terminal to keep open, no SSH keys, no IPs to allow.

```bash
deploy/aws.sh up --tailscale --project owner/repo --claude-token "$(claude setup-token)"
```

### Day-to-day commands (AWS & Azure)

```bash
deploy/aws.sh open                # SSH tunnel + open office in browser  (Ctrl-C closes tunnel)
deploy/aws.sh status              # machine state, address, who's invited
deploy/aws.sh logs                # tail the office logs
deploy/aws.sh ssh                 # shell on the machine
deploy/aws.sh update              # install latest Manan-CLAUDE-OFFICE and restart
deploy/aws.sh resize t3.2xlarge   # upgrade or downgrade, same address
deploy/aws.sh pause               # stop machine — only disk + IP are billed
deploy/aws.sh resume              # start it again and open it
deploy/aws.sh destroy             # delete everything created (asks first)
```

You can also upgrade from inside the office: **☰ → ⬆️ Upgrade the office**.

---

## Add users

Everyone gets their own account — their name shows on their character, in chat, and in every terminal they type into.

### 1 · Give them access to the server

> On a **Tailscale** office, anyone on your tailnet can already open it — skip to step 2.

For non-Tailscale deployments, a teammate needs their SSH key on the machine. Open **☰ → 👥 Invite teammates** and enter their GitHub username, or from your terminal:

```bash
deploy/aws.sh invite octocat        # fetches keys from github.com/octocat.keys
deploy/aws.sh allow 203.0.113.7     # or allow by IP ("allow anywhere" opens to every IP)
```

This prints a command to send them. They run it and open http://localhost:4600:

```
ssh -L 4600:localhost:4600 office@<your-office-ip>
```

Their key logs in as a locked-down `office` user — no shell, only port forwarding.

### 2 · Create their account

Open **☰ → 🔑 Accounts** and generate an invite link (works once, 7-day TTL). Or from the terminal:

```bash
Manan-CLAUDE-OFFICE accounts                       # list accounts and open invites
Manan-CLAUDE-OFFICE accounts invite ada --admin    # prints a single-use /join#… link
Manan-CLAUDE-OFFICE accounts role ada member       # change a role
Manan-CLAUDE-OFFICE accounts revoke ada            # signs them out within seconds
```

### 3 · Their own Claude & GitHub

With accounts, each person's workers run on their own Claude plan and GitHub actions appear under their name. On first visit, **🔐 Your sign-ins** (☰ menu) lets them sign in with Claude or GitHub — or paste a token directly.

### 4 · Turn off the shared password

Once everyone has an account, disable it in **🔑 Accounts** or with:

```bash
Manan-CLAUDE-OFFICE accounts password off
```

---

## Controls

| Key | Action |
|:---:|---|
| `W` `A` `S` `D` | Walk · hold `Shift` to run |
| `Space` | Jump |
| Mouse drag / wheel | Orbit / zoom the camera |
| `E` | Interact — hire a worker, open its terminal, read a board, sit down, ride the elevator |
| `P` | Give a task to a new worker, or to the one at this desk |
| `C` | Worker's changes — diff, commit, open a PR |
| `N` | Jump to the next worker waiting on you |
| `X` | Send a worker home |
| `T` / `Enter` | Chat |
| `V` | Join voice · hold `V` to talk |
| `M` | Mute / unmute in voice |
| `Tab` | Open the ☰ menu |
| `Esc` | Close any window |
| `Ctrl` + `[` | Send Esc to a terminal (close Claude menus / interrupt) |

Full list: [docs/controls.md](docs/controls.md)

---

## Development

```bash
npm install
npm run dev          # Vite with hot reload on :5173, server on :4600 (password: dev)
npm run typecheck
npm test
```

> Server edits restart the server, not the workers. After changing `ptyhost.ts`, bump `PTY_PROTOCOL` in `ptys.ts` so the next server replaces the PTY host.

Every change that lands on `main` is published as a GitHub release by [`.github/workflows/release.yml`](.github/workflows/release.yml), and `install.sh` always installs the newest one. Bump `package.json`'s version to start a new minor.

---

## Docs

| | |
|---|---|
| [Features](docs/features.md) | Everything in the office, room by room |
| [Agents](docs/agents.md) | Claude Code, Codex and OpenCode — models, effort levels, and the office's prompts |
| [Configuration](docs/configuration.md) | Every command-line option, and where the office keeps its data |
| [AWS reference](docs/aws.md) | Tailscale, service tunnels, upgrades, and every `deploy/aws.sh` command |
| [Azure reference](docs/azure.md) | VM sizes, pausing, and every `deploy/azure.sh` command |
| [Self-hosting](docs/self-hosting.md) | One-line setup for any Ubuntu/Debian server, or by hand behind Caddy or nginx |
| [How it works](docs/how-it-works.md) | Architecture and security notes |

---

<div align="center">
<sub>MIT License · <a href="LICENSE">LICENSE</a></sub>
</div>
