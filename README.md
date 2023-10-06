# Note/News:
I've been away from any open source work for a while. I also have had issues with my Github account for a while. However!, I know a lot of people like this plugin and have posted a lot of ideas/errors in the issues. 

#### I will be spending a good amount of time to update the plugin, instructions, deal with outstanding errors, and begin adding features that have been requested. 
If you have a specific issue that is important to you please add any kind of "reaction" to the first comment in that issue and/or a comment of your own(if you have something important to add). 
If I notice that an issue has a lot of activity, then I will try to prioritize that work first. 

As well, if you are a Twitter user. Feel free to [follow me](https://twitter.com/ELWillis10). My private messages are always open if you want to contact me for whatever reason. 

Thanks everyone for all the interest and nice comments over the years :)

--Ethan

# Zotero Scihub

This is an add-on for [Zotero](https://www.zotero.org/) and [Juris-M](https://juris-m.github.io/) that enables automatic download of PDFs for items with a DOI.

# Quick Start Guide

#### Install

- Download the latest release (.xpi file) from the [Releases Page](https://github.com/ethanwillis/zotero-scihub/releases)
  _Note_ If you're using Firefox as your browser, right click the xpi and select "Save As.."
- In Zotero click "Tools" in the top menu bar and then click "Addons"
- Go to the Extensions page and then click the gear icon in the top right.
- Select Install Add-on from file.
- Browse to where you downloaded the .xpi file and select it.
- Restart Zotero, by clicking "restart now" in the extensions list where the
  scihub plugin is now listed.

#### Usage

Once you have the plugin installed simply, right click any item in your collections.
There will now be a new context menu option titled "Update Scihub PDF." Once you
click this, a PDF of the file will be downloaded from Scihub and attached to your
item in Zotero.

For any new papers you add after this plugin is installed, the scihub pdf will be
automatically downloaded.

#### Configuration

Plugin is configured through the dedicated tab: 

<img width="782" alt="Screenshot 2021-08-21 at 22 14 04" src="https://user-images.githubusercontent.com/387791/130333778-8bfb0878-2122-49a9-bc23-c528eb9b6cbf.png">

#### DNS-over-HTTPS

In case of malfunctioning or unsafe local DNS server, Zotero (as it's built on Firefox) might be configured with [Trusted Recursive Resolver](https://wiki.mozilla.org/Trusted_Recursive_Resolver) or DNS-over-HTTPS, where you could set your own DNS server just for Zotero without modifying network settings.

_Preferences > Advanced > Config Editor_

1. set `network.trr.mode` to `2` or `3`, this enables DNS-over-HTTPS (2 enables it with fallback)
2. set `network.trr.uri` to `https://cloudflare-dns.com/dns-query`, this is the provider’s URL
3. set `network.trr.bootstrapAddress` to `1.1.1.1`, this is cloudflare’s normal DNS server (only) used to retrieve the IP of cloudfaire-dns.com
4. Restart zotero, wait for a DNS cache to clean up.

## Building

0. Pre-requisite is to have [node.js](nodejs.org) installed
1. Install dependencies `npm install`
2. Build `npm run build`

## [Contributing](./CONTRIBUTING.md)

## Disclaimer

Use this code at your own peril. No warranties are provided. Keep the laws of your locality in mind!

```
zotero-scihub
├─ .eslintignore
├─ .eslintrc.json
├─ .git
│  ├─ FETCH_HEAD
│  ├─ HEAD
│  ├─ branches
│  ├─ config
│  ├─ description
│  ├─ hooks
│  │  ├─ applypatch-msg.sample
│  │  ├─ commit-msg.sample
│  │  ├─ fsmonitor-watchman.sample
│  │  ├─ post-update.sample
│  │  ├─ pre-applypatch.sample
│  │  ├─ pre-commit.sample
│  │  ├─ pre-merge-commit.sample
│  │  ├─ pre-push.sample
│  │  ├─ pre-rebase.sample
│  │  ├─ pre-receive.sample
│  │  ├─ prepare-commit-msg.sample
│  │  ├─ push-to-checkout.sample
│  │  └─ update.sample
│  ├─ index
│  ├─ info
│  │  └─ exclude
│  ├─ logs
│  │  ├─ HEAD
│  │  └─ refs
│  │     ├─ heads
│  │     │  └─ master
│  │     └─ remotes
│  │        ├─ origin
│  │        │  └─ HEAD
│  │        └─ upstream
│  │           ├─ HEAD
│  │           ├─ dependabot
│  │           │  └─ npm_and_yarn
│  │           │     ├─ json5-1.0.2
│  │           │     ├─ jszip-3.10.1
│  │           │     └─ xmldom
│  │           │        └─ xmldom-0.8.5
│  │           └─ master
│  ├─ objects
│  │  ├─ 13
│  │  │  └─ 09e2f6e00522e3dd97da32f706391970930c7c
│  │  ├─ 30
│  │  │  └─ 529b927f8fad7a3ed119d412eacf0814c931a5
│  │  ├─ 36
│  │  │  └─ 5eb9a64fca70b7d54e4f89fccc47bef8168e7a
│  │  ├─ 55
│  │  │  └─ b3e10b336107f2433d6770c583b40647bbe6e9
│  │  ├─ 57
│  │  │  └─ 9e567c4507712ae51ded2c9c2bc70206838dfd
│  │  ├─ 5d
│  │  │  └─ 94e3c69d69bfe7136ff0f77b4ab4533d659c00
│  │  ├─ 61
│  │  │  └─ 5d7e48d2909c44db04f57479993ffc3dda1a86
│  │  ├─ 64
│  │  │  └─ ebe653a87af27d5b4f7bcb4fd36d519b3fa86a
│  │  ├─ 6a
│  │  │  └─ 77f13a539f6f9416884914653919cda3b38445
│  │  ├─ 72
│  │  │  └─ b035848e8ffec0bd5565e7c43dfdc08435b2bb
│  │  ├─ 7a
│  │  │  └─ c28cab612d9af77e9c53c250dcdf6c787988da
│  │  ├─ 8b
│  │  │  └─ 10cb56a7c9cde91774b4612ce568b1f0451844
│  │  ├─ a0
│  │  │  └─ 1cabb49868fb8826f501eca68ad183557a4f80
│  │  ├─ a3
│  │  │  └─ 164123fd3645d7abdf866bd26eb8c202aa64b1
│  │  ├─ a4
│  │  │  └─ f80b6934aea4b328cf8fc0c8068c2b4654923e
│  │  ├─ aa
│  │  │  └─ f63ac4e463b7e0f62a2da74aab3bd3753f420b
│  │  ├─ ae
│  │  │  └─ 40b9b59039f79a6c0bd59e5cd3eae55aa42c76
│  │  ├─ b5
│  │  │  └─ f0a52ecca61f477709fe1717524739ba5f8c0d
│  │  ├─ b6
│  │  │  └─ 844f585541154921b44589d3bbb19d192d3a91
│  │  ├─ c7
│  │  │  └─ e7f9b0212b94928211671c0ed8d20cf8e3328a
│  │  ├─ d4
│  │  │  └─ 68a827d4321228ee5e357ceeadc96d8ca2a706
│  │  ├─ e1
│  │  │  └─ ca60de9baf226480a36de6596fb761a9052c69
│  │  ├─ ed
│  │  │  └─ 0b25e7af9bcbac523a34b7f737bdb7ec6b594c
│  │  ├─ ee
│  │  │  └─ a51a9d0b014cf9d7619b425013e860dd2c6ee3
│  │  ├─ f1
│  │  │  └─ 44162a56169a85f6e9b4609a28c89cc2873809
│  │  ├─ f2
│  │  │  └─ a1c53a41e4a266eada140ce1f958f93895da7c
│  │  ├─ fb
│  │  │  └─ 4c260ffb711f07b59b1c3e3c320c9708aac94e
│  │  ├─ info
│  │  └─ pack
│  │     ├─ pack-e0cc1bdfbe109a5e1c1b79da9f5d0c3af7eaa581.idx
│  │     └─ pack-e0cc1bdfbe109a5e1c1b79da9f5d0c3af7eaa581.pack
│  ├─ packed-refs
│  └─ refs
│     ├─ heads
│     │  └─ master
│     ├─ remotes
│     │  ├─ origin
│     │  │  └─ HEAD
│     │  └─ upstream
│     │     ├─ HEAD
│     │     ├─ dependabot
│     │     │  └─ npm_and_yarn
│     │     │     ├─ json5-1.0.2
│     │     │     ├─ jszip-3.10.1
│     │     │     └─ xmldom
│     │     │        └─ xmldom-0.8.5
│     │     └─ master
│     └─ tags
│        ├─ 0.0.1
│        ├─ 0.0.2
│        ├─ 0.0.3
│        ├─ 0.0.4
│        ├─ 0.0.4-beta
│        ├─ 0.0.4-beta.1
│        ├─ 0.0.4p1
│        ├─ 0.0.5
│        ├─ 0.0.6
│        ├─ release
│        ├─ v1.0.1
│        ├─ v1.0.2
│        ├─ v1.0.3
│        ├─ v1.0.4
│        ├─ v1.0.5
│        ├─ v1.0.6
│        ├─ v1.0.7
│        ├─ v1.0.8
│        ├─ v1.0.9
│        ├─ v1.1.0
│        ├─ v1.1.1
│        ├─ v1.1.2
│        ├─ v1.1.3
│        ├─ v1.2.0
│        ├─ v1.3.0
│        ├─ v1.4.0
│        ├─ v1.4.2
│        └─ v1.4.4
├─ .github
│  ├─ ISSUE_TEMPLATE
│  │  ├─ bug_report.md
│  │  └─ feature_request.md
│  └─ workflows
│     └─ main.yml
├─ .gitignore
├─ .nycrc
├─ .tool-versions
├─ CONTRIBUTING.md
├─ LICENSE
├─ README.md
├─ chrome.manifest
├─ content
│  ├─ itemPane.ts
│  ├─ itemPane.xul
│  ├─ prefPane.ts
│  ├─ prefPane.xul
│  ├─ scihub.ts
│  ├─ toolsPane.ts
│  ├─ toolsPane.xul
│  ├─ urlUtil.ts
│  └─ zoteroUtil.ts
├─ locale
│  └─ en-US
│     ├─ itemPane.dtd
│     ├─ prefPane.dtd
│     └─ toolsPane.dtd
├─ package-lock.json
├─ package.json
├─ skin
│  └─ default
│     └─ sci-hub-logo.svg
├─ tests
│  ├─ scihub.test.ts
│  ├─ urlUtil.test.ts
│  ├─ zotero.mock.ts
│  ├─ zoteroItem.mock.ts
│  └─ zoteroUtil.test.ts
├─ tsconfig.json
└─ typings
   └─ zotero.d.ts

```