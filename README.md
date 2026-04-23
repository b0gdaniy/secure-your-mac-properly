# 🔒 Secure Your Mac Properly 

🍏💻 Dive into a curated toolkit of macOS privacy and security apps. Lock down your system, protect your data, and stay in control of your digital footprint with these carefully selected tools and resources.

---

**[Hitchhiker's Guide](https://anonymousplanet.org/)**

**[MacOS Security and Privacy Guide](https://github.com/drduh/macOS-Security-and-Privacy-Guide)**

**[MacOS Security Compliance](https://github.com/usnistgov/macos_security)**

**[Macos Secure Profiles](https://github.com/sambacha/macos-secure-profiles)**

**[Article from Oficer CIA](https://x.com/officer_secret/status/1936486233393238028)**

**[Article from Trail Of Bits](https://docs.google.com/document/d/1-_0Wlwch_vtkPM4F-SdEXLjQYaYT7KoPlU2rjt7tkLQ/edit?tab=t.0)**

---

## Content list

(roughly ordered from most critical security layers to more general utilities)

* [Security](#security)
* [Password Managers](#password-managers)
* [VPN](#vpn)
* [Browsers](#browsers)
* [Browser Extensions](#browser-extensions)
* [Email clients](#email-clients)
* [Temporary emails](#temporary-emails)
* [Encryption](#encryption)
* [Communication](#communication)
* [Crypto Wallets](#crypto-wallets)
* [Backup & Sync](#backup--sync)
* [Metadata & File Hygiene](#metadata--file-hygiene)
* [Tools](#tools)
* [Development](#development)
* [Notes](#notes)

---

### Security

* **[LuLu](https://github.com/objective-see/LuLu)** – free and open-source outbound firewall for macOS that lets you monitor and control which apps can access the network, helping block unwanted connections, trackers, and malware.
* **[LittleSnitch](https://www.obdev.at/products/littlesnitch/index.html)** - macOS network monitor and application firewall that shows which apps are connecting to the Internet and lets you allow or block those connections. It provides real-time traffic visibility, per-app and per-domain rules, profiles, blocklists, and detailed connection monitoring to help control unwanted network activity, trackers, or suspicious connections.
* **[Fortress](https://github.com/essandess/macOS-Fortress)** – firewall + privatizing proxy stack for blocking trackers, attackers, malware, adware, and spam. Uses PF, Squid, Privoxy, blocklists, and integrates with ClamAV for on-demand/on-access scanning.
* **[Stronghold](https://github.com/alichtman/stronghold)** – terminal tool that quickly applies recommended macOS security and privacy settings, hardening the system with a single command.
* **[ClamAV](https://github.com/Cisco-Talos/clamav)** – open-source antivirus engine used for scanning files and mail for malware (viruses, trojans, etc.), useful for on-demand scans or integrating into your own scripts and workflows.

#### System hardening & security checks

* **[Pareto Security](https://github.com/ParetoSecurity/pareto-mac)** – menu bar app that audits your Mac’s security settings (FileVault, firewall, auto-updates, screen lock, etc.) and shows what should be enabled or fixed to follow best practices.
* **[Mergen](https://github.com/sametsazak/mergen)** - native macOS security auditing tool that checks your Mac against the CIS Apple macOS benchmark, covering areas like updates, firewall, sharing, privacy, authentication, and encryption. It comes as both a desktop app and a CLI, and can automatically remediate many failed checks and verify the fixes afterward.

#### Application control

* **[Santa](https://github.com/google/santa)** – macOS binary authorization system (from Google) that can work in monitoring or “lockdown” mode, allowing only approved binaries to run and giving you fine-grained control over what can execute on your system.

#### Runtime & privacy monitors (Objective-See)

* **[BlockBlock](https://objective-see.org/products/blockblock.html)** – monitors common persistence locations (LaunchAgents, LaunchDaemons, etc.) and alerts you when something tries to install itself for auto-start, helping catch malware as it attempts to persist.
* **[KnockKnock](https://objective-see.org/products/knockknock.html)** – scans what is already configured to persist on your system and lists launch items, login items, and other auto-start components so you can spot suspicious entries.
* **[OverSight](https://objective-see.org/products/oversight.html)** – watches for microphone and camera access and shows which process is using them, letting you block unexpected or suspicious access.

#### Advanced monitoring & EDR (for power users)

* **[Wazuh Agent](https://documentation.wazuh.com/)** – open-source XDR/HIDS agent for macOS, Linux, and Windows. Provides file integrity monitoring, rootkit detection, log analysis, and alerts when connected to a Wazuh server. Best if you want a mini-SOC at home or in a lab.
* **[OpenEDR](https://github.com/ComodoSecurity/openedr)** – open-source endpoint detection and response platform. Offers real-time monitoring, detection, and response capabilities across endpoints (including macOS), but requires some infrastructure and tuning, so more suitable for advanced users and lab setups.

---

### Password Managers

* **[Bitwarden](https://github.com/bitwarden)** – open-source password manager with end-to-end encryption, cross-platform clients, and browser extensions, ideal for managing logins and secure notes.
* **[Proton Pass](https://proton.me/pass)** – password manager from Proton with open-source apps, end-to-end encryption, and support for email aliases, focused on privacy and cross-platform use.
* **[KeePassXC](https://github.com/keepassxreboot/keepassxc)** – community-driven, cross-platform password manager based on the KeePass format, storing credentials in an encrypted local database under your control.
* **[Pass](https://www.passwordstore.org/)** – “standard Unix password manager” that stores each secret as a GPG-encrypted file, works nicely with Git and the terminal, and has various GUIs and browser integrations.
* **[gopass](https://www.gopass.pw/)** – Go-based, extended implementation of pass with teams support, mounts, and better integration with Git/GPG, suitable for both personal and team setups.
* **[Vault](https://github.com/hashicorp/vault)** – secrets management and encryption-as-a-service platform for securely storing tokens, passwords, certificates, and other sensitive data with fine-grained access control.
* **[Passbolt](https://www.passbolt.com/)** – open-source, self-hostable password manager built for teams, with a focus on sharing credentials securely, managing permissions, and integrating into workflows.

---

### VPN

* **[Proton VPN](https://github.com/ProtonVPN)** – privacy-focused VPN with strong encryption, a strict no-logs policy, and apps for multiple platforms, designed to protect your traffic from surveillance and tracking.
* **[Mullvad VPN](https://github.com/mullvad/mullvadvpn-app)** – VPN service with a strong focus on anonymity and privacy (account numbers instead of email), offering open-source client apps for desktop and mobile.

---

### Browsers

* **[Firefox](https://www.mozilla.org/en-US/firefox/new/)** – a widely-used open-source web browser known for its privacy-focused features and customization options. It prioritizes user security with strong privacy controls and a rich collection of add-ons for personalized browsing experiences.
* **[LibreWolf](https://librewolf.net/)** – Firefox-based browser with hardened privacy and security settings out of the box, telemetry removed, and tighter tracking/fingerprinting protection.
* **[Mullvad Browser](https://mullvad.net/en/browser)** – a privacy-hardened browser developed by Mullvad in collaboration with the Tor Project. It’s based on Firefox ESR and configured to minimize fingerprinting and tracking. Unlike Tor Browser, it’s designed to be used **together with a VPN** (for example, Mullvad VPN) rather than the Tor network, giving a Tor-like anti-fingerprinting profile over a VPN tunnel.
* **[DuckDuckGo](https://duckduckgo.com/)** – a privacy-focused web browser and search engine designed to protect your online privacy. It prioritizes user security with built-in privacy features and a simplified, user-friendly interface for a safer browsing experience.
* **[Tor Browser](https://www.torproject.org/download/)** – a privacy-focused web browser that conceals your identity by routing internet traffic through the Tor network. It's designed for enhanced online anonymity and security.

---

### Browser Extensions

* **[NoScript](https://noscript.net/)** – FOSS extension for Firefox, Chrome, Edge, Brave, and others that lets you selectively allow JavaScript, Java, and other active content on a per-site basis.
* **[uBlock Origin](https://github.com/gorhill/uBlock/)** – efficient, lightweight blocker for Chromium and Firefox, capable of filtering ads, trackers, and malicious domains with very low CPU/memory usage.

---

### Email clients

* **[Thunderbird](https://www.thunderbird.net/)** – free and open-source email client and PIM (mail, contacts, calendars) with strong security options, add-ons, and cross-platform support (Windows/macOS/Linux).
* **[eM Client](https://github.com/emclient)** – email and calendar management software with a user-friendly interface and support for modern mail protocols.

---

### Temporary emails

* **[Maildrop](https://maildrop.cc/)** – free disposable email service that lets you create custom addresses to receive mail without exposing your real inbox.
* **[10MinuteMail](https://10minutemail.com/)** – disposable email inbox that auto-expires after 10 minutes (with an option to extend), useful for quick sign-ups and reducing spam.

---

### Encryption

* **[VeraCrypt](https://github.com/veracrypt/VeraCrypt)** – widely used open-source disk encryption solution for creating encrypted containers or encrypting entire drives, protecting files from unauthorized access.
* **[Cryptomator](https://cryptomator.org/)** – client-side, transparent encryption for cloud storage folders, so your data is encrypted before syncing to providers like Dropbox or Google Drive.

---

### Communication

* **[Signal](https://github.com/signalapp)** – end-to-end encrypted messaging, voice, and video calling app, designed with minimal metadata and strong privacy guarantees.
* **[Matrix](https://matrix.org/)** – open standard and ecosystem for secure, decentralized, real-time communication, used for encrypted chat, collaboration, and bridging other networks.
* **[OnionShare](https://onionshare.org/)** – tool for anonymously and securely sharing files, hosting temporary sites, and chatting over Tor without requiring accounts or central servers.
* **[XMPP with Monal as client](https://xmpp.org/)** – open protocol for federated, extensible messaging with support for secure, private communication; Monal is a native macOS/iOS client.
* **[Cinny](https://github.com/cinnyapp/cinny)** – Matrix client focused on a simple, elegant, and secure interface for everyday encrypted chats.
* **[Element](https://github.com/vector-im/element-web)** – feature-rich Matrix client emphasizing performance, collaboration, and usability.
* **[AppFlowy](https://github.com/AppFlowy-IO/AppFlowy)** – open-source, self-hostable alternative to Notion, useful for collaborative docs and planning where you keep control over your data.

---

### Crypto Wallets

* **[Metamask](https://metamask.io)** – browser extension and mobile wallet for managing Ethereum and compatible networks, interacting with dApps, and signing transactions.
* **[Trezor Suite](https://trezor.io/trezor-suite)** – companion software for Trezor hardware wallets to manage cryptocurrencies, sign transactions, and review balances with strong security.
* **[Ledger Live](https://www.ledger.com/ledger-live)** – companion app for Ledger hardware wallets (Nano S Plus, Nano X, etc.) to manage multiple cryptocurrencies, track portfolios, and securely sign transactions while keeping private keys on the hardware device.
* **[Electrum](https://github.com/spesmilo/electrum)** – lightweight Bitcoin wallet with support for hardware wallets, multisig, and cold storage setups.
* **[Feather](https://github.com/feather-wallet/feather)** – free, open-source Monero wallet for Linux, Tails, macOS, and Windows, focused on privacy and usability.

---

### Backup & Sync

* **[Syncthing](https://github.com/syncthing/syncthing)** – decentralized, encrypted file synchronization between your devices without a central server, keeping data under your control.
* **[Restic](https://github.com/restic/restic)** – fast, secure, deduplicating backup tool with built-in encryption, suitable for backing up to local disks, servers, or cloud storage.

---

### Metadata & File Hygiene

* **[Metadata Cleaner](https://gitlab.com/rmnvgr/metadata-cleaner)** – GUI tool for removing metadata (EXIF, author info, etc.) from documents and images before sharing.
* **[MAT2](https://0xacab.org/jvoisin/mat2)** – command-line metadata anonymization toolkit that strips identifying information from many file formats.

---

### Tools

* **[Rectangle](https://github.com/rxhanson/Rectangle)** – open-source window manager for macOS that lets you snap and arrange windows via keyboard shortcuts, improving productivity on large screens.
* **[AlDente](https://github.com/AppHouseKitchen/AlDente-Charge-Limiter)** – battery charge limiter for MacBooks, allowing you to cap maximum charge level to prolong battery health, useful for always-plugged-in laptops.
* **[AppCleaner](https://freemacsoft.net/appcleaner/)** – lightweight macOS utility that helps you fully remove apps by also deleting their related files (caches, preferences, support files), keeping the system cleaner and reducing leftovers after uninstalls.

---

### Development

* **[Atom](https://github.com/atom/atom)** – hackable, open-source text editor with a large ecosystem of community packages and built-in Git integration.
* **[VSCodium](https://github.com/VSCodium/vscodium)** – telemetry-free, open-source build of VS Code, providing the same editor experience without proprietary branding or tracking.

---

### Notes

* **[Logseq](https://logseq.com/)** – open-source, privacy-first outliner and knowledge management tool based on local Markdown/Org-mode files and bidirectional links.
* **[Draw.io](https://github.com/jgraph/drawio)** – free diagramming tool for flowcharts, architectures, and other visuals, available as a web app and desktop app.
* **[LibreOffice](https://www.libreoffice.org/)** – full-featured open-source office suite (Writer, Calc, Impress, etc.) for creating and editing documents, spreadsheets, and presentations.
