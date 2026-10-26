# AAA ExpressVPN Test Lab

### Check location and protocol combinations on your Windows connection

**AAA Software Studio** · Windows 10/11 x64 · **4.2.3 single-file build**

[Releases](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/releases) · [Report an issue](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/issues)

AAA ExpressVPN Test Lab brings location selection, protocol checks, live results and connection reports into one Windows dashboard. It works with the official ExpressVPN application already installed and signed in on your computer.

**Independent project. Not affiliated with or endorsed by ExpressVPN. No VPN subscription or credentials are included.**

## Download and run

Download **AAA-ExpressVPN-TestLab-4.2.3-Windows-x64.exe** from the release Assets and open it. This build is a single EXE: **no separate Python installation, support folder or installer is required.** Third-party notices are included inside the application under **Help → About / Third-party licenses**.

You still need the **official ExpressVPN Windows application**, a compatible `expressvpnctl.exe` and your own active account. Sign in through ExpressVPN's own window. The utility may request administrator rights when controlling VPN connections.

The release file is the manually attached **.exe**, not GitHub's automatic **Source code** ZIP/TAR downloads. Those contain this documentation repository only. The download is available once the release is published.

## What you can do

- Select countries, individual locations or all locations returned by your installed client.
- Choose Automatic, Lightway UDP/TCP, WireGuard and OpenVPN TCP/UDP, subject to client support.
- Adjust connection timeouts, retries and post-connection observation.
- Follow verified connections, all attempts and live diagnostic output.
- Copy results or export CSV/JSON reports to your computer.
- Enable an optional HTTPS check and review a warning before connection changes.

A verified result combines official connected status, a matching location and a public IP change against a disconnected baseline, plus HTTPS when enabled. It is not a bandwidth benchmark, a list of every physical server or proof that a failed location is blocked.

## Before starting a scan

Scanning intentionally changes VPN connections and does **not** restore the original connection or protocol. After connection changes begin, finish, Stop and handled errors attempt disconnection and verify status. Forced termination, shutdown or crashes can prevent cleanup. Read the in-app confirmation and avoid tasks that require an uninterrupted VPN connection while testing.

Preflight errors, cancellation and Stop before connection changes are covered by automated regression tests using simulated CLIs.

## Build and validation

Version 4.2.3 changes packaging to a single executable and adds an embedded notices viewer. VPN scan logic is unchanged from 4.2.2. The preceding folder-based 4.2.2 GUI was opened successfully on the creator's Windows PC. New build and standalone startup results will be recorded in the 4.2.3 release notes; this does not imply a full live VPN test or compatibility with every Windows installation.

The binary is unsigned. No publisher signature or independent security audit is claimed.

## Data and privacy

Settings and reports are stored under `%LOCALAPPDATA%\AAA-ExpressVPN-TestLab`; they are not placed beside the EXE. Reports may contain public IPs, timestamps, selected locations and CLI diagnostics. Remove private information before sharing them.

Public-IP requests use ipify, with Amazon checkip as fallback; optional HTTPS checks use Cloudflare. These endpoints observe request source IPs. The official ExpressVPN app has its own network behavior and policies.

## Feedback and project scope

For now, use [GitHub Issues](https://github.com/aaa-software-studio/aaa-expressvpn-test-lab-showcase/issues) for feedback, with private details removed. Direct studio contact details will be added later.

This repository hosts the product introduction, documentation and executable releases. Development source remains private. No open-source license for the private application is granted by this showcase. Third-party rights and notices remain applicable; ExpressVPN names and marks belong to their respective owners.

Built by [AAA Software Studio](https://github.com/aaa-software-studio), from the creator's idea with AI assistance.
