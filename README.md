# Julio Arias Pabón

### Senior Network Engineer (Tier 3) moving into Cloud & Systems Engineering.

I keep mission-critical networks running for DoD and enterprise environments — and I build the monitoring tools, cloud infrastructure, and automation that keep them running with less manual effort.

Most cloud engineers learn networking second. I started there.

<table>
  <tr>
    <td><strong>💼 Role</strong></td>
    <td>Network Engineer, Tier 3 — DoD &amp; enterprise networks</td>
  </tr>
  <tr>
    <td><strong>🎯 Target Roles</strong></td>
    <td>Cloud Engineer</td>
  </tr>
  <tr>
    <td><strong>📜 Certifications</strong></td>
    <td>Cisco CCNA · CompTIA Security+</td>
  </tr>
  <tr>
    <td><strong>📬 Contact</strong></td>
    <td>
      <a href="mailto:julioarias1496@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email Julio Arias" /></a>
      <a href="https://www.linkedin.com/in/julio-arias-pabon-3b4a15388"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="Julio Arias on LinkedIn" /></a>
      <a href="https://www.julioarias.cloud/"><img src="https://img.shields.io/badge/Portfolio-0B4D3B?style=flat-square&logo=googlechrome&logoColor=white" alt="julioarias.cloud portfolio" /></a>
    </td>
  </tr>
</table>

---

## What I've built

### NetMonTool — monitoring and reporting for environments that can't buy it

**The problem:** Commercial monitoring platforms like SolarWinds and PRTG cost five figures a year, and in secured government environments they often can't be installed at all. Teams end up with no visibility and no uptime data to show leadership.

**What it does:** Turns any Windows machine into a live operations dashboard tracking up to 15 devices in real time, and automatically produces the daily and weekly availability reports that management actually asks for.

**Under the hood:** Single-file PowerShell 5.1, zero external dependencies — no agents, no licenses, no install. Async .NET `SendPingAsync` polls every node in parallel, holding a true 5-second refresh even when nodes are timing out. A per-node state machine drives five status tiers; cumulative counters are crash-safe and reload after a restart; weekly latency is aggregated with correct weighting rather than averaging averages. Status changes are written to CSV incident timelines and surfaced in the Windows Event Log with dedicated event IDs, so there's an audit trail independent of the tool itself.

Shipped like a real project, not a script dump: MIT licensed, versioned changelog, architecture documentation, PSScriptAnalyzer linting, and contribution guidelines.

**→ [github.com/jariax/NetMonTool](https://github.com/jariax/NetMonTool)**

---

### julioarias.cloud — AWS infrastructure, built the secure way

**The problem:** Anyone can put a resume online. Running the infrastructure behind it — correctly, with the bucket actually locked down — is a different claim.

**What it does:** Serves my portfolio at [julioarias.cloud](https://julioarias.cloud), and doubles as a working reference architecture for a secure static site on AWS.

**Under the hood:** S3 origin with *Block All Public Access* enabled, so the bucket is never directly reachable — content is served only through CloudFront using Origin Access Control. TLS certificate managed in ACM (us-east-1), DNS through Route 53, and a GitHub Actions pipeline that builds and deploys automatically on every push to `main`. No manual uploads, no public buckets.

**→ [github.com/jariax/julioarias-cloud](https://github.com/jariax/julioarias-cloud)**

---

### MortDrop — a production web application, start to finish

**The problem:** Most mortgage payoff calculators are ad-choked lead-generation traps that hide the number you came for.

**What it does:** Shows homeowners exactly what extra payments save them in interest and how many years they cut off the loan — clean, ad-free, and free to use. Live at **[mortdrop.com](https://mortdrop.com)**.

**Under the hood:** An amortization engine computing full payoff schedules and interest-savings comparisons across payment scenarios. Complete authentication flow — registration, login, password reset — plus user account management and an internal admin dashboard. Installable as a mobile web app (PWA), served on a custom domain over TLS, with the privacy policy and terms a real product needs.

I designed, built, and shipped it end to end.

*Also in development: **Tend**, a nutrition and health app with AI coaching and Stripe subscription billing.*

---

## Toolbox

**Cloud** — AWS: S3, CloudFront (Origin Access Control), Route 53, ACM, IAM · secure-by-default architecture · least-privilege access

**Automation & CI/CD** — PowerShell (advanced) · GitHub Actions · Python · scripted deployment and reporting pipelines

**Monitoring & operations** — availability and latency metrics · event logging and audit trails · incident timelines · NOC operations · escalation-tier troubleshooting

**Networking** — Cisco routing & switching · VLANs · TCP/IP and network troubleshooting · CSfC and secured-environment networking

**Security** — CompTIA Security+ · Microsoft Sentinel (SIEM lab)

**Development** — JavaScript / TypeScript · HTML & CSS · REST APIs · authentication flows

**Currently learning:** Terraform and infrastructure-as-code, plus AWS Solutions Architect Associate.

---

## Also on this profile

A few repos here are forks I use as working labs rather than original work — a Microsoft Sentinel SIEM lab, an AI job-search framework, and Python coursework. They're public on purpose: the learning is part of the record.

---

## Get in touch

I'm actively looking for **Cloud Engineer** roles, and I'm glad to walk through the architecture or code behind anything above.

<p align="center">
  <a href="mailto:julioarias1496@gmail.com">
    <img src="https://img.shields.io/badge/Email%20Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email Julio Arias" />
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/julio-arias-pabon-3b4a15388">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Julio Arias on LinkedIn" />
  </a>
  &nbsp;
  <a href="https://www.julioarias.cloud/">
    <img src="https://img.shields.io/badge/Portfolio-0B4D3B?style=for-the-badge&logo=googlechrome&logoColor=white" alt="julioarias.cloud portfolio" />
  </a>
</p>
