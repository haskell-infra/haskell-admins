# Haskell Infrastructure Admins

The infrastructure team is ultimately responsible for maintaining Haskell.org services. It is not required you be a member of any existing group (for example, the Haskell.org committee) to join. The infrastructure team deals solely with technical aspects of Haskell.org infrastructure, including sensitive matters like domain management, backups, administrative email, security response, service allocation, and domain or URL routing. 

### Service details

Here are some of the services the infra team maintains.

* www.haskell.org - the primary website
* wiki.haskell.org - Our MediaWiki instance, hosting tons of content.
* hackage.haskell.org - The primary Hackage instance for Haskell.org; this setup is proxied in the front by Fastly, to provide low-latency downloads and caching for Hackage
* mail.haskell.org - Serving a variety of haskell-related mailing lists
* hoogle.haskell.org - the Haskell API search engine
* planet.haskell.org - Our Planet Venus instance, which powers the Haskell.org community RSS feeds.
* downloads.haskell.org - A downloads server hosting tons of static content, proxied by Fastly.
* archives.haskell.org - archives of decommissioned sites and services related to the open-source Haskell community.
* gitlab.haskell.org - The GHC git repositories and issue tracking system.
* status.haskell.org - A service providing status updates on haskell.org infrastructure issues (provided by status.io).

### How the Haskell Admins make decisions

The infra team does not seek to be a decision-making body, except in matters of particular technical detail (i.e. the specifics of a postfix configuration). Decisions that affect end-users are typically made by actual decision-making bodies, and the infra team simply aims to implement, assist, and manage their follow-through and continued maintenance. As a small group with a technical focus, our day to day operations are managed informally based on a division of labor, trust, and deference to other bodies in the case of dispute. Depending on the service in question, policy decisions may be made by the haskell.org committee, the hackage admin team, the ghc development team, hoogle maintainers, etc. Ultimately, since the haskell.org committee controls the domain, it tends to have final say -- but there may be various levels of intermediate delegation and shared responsibility along the way.

### How to contribute

Maintaining infrastructure is a task of serious responsibility, and little thanks (if we do our job right, you don't notice). We are always looking for more skilled volunteers to help out, and onboard people by building up from smaller tasks to a broader overview of the full scope of our infrastructure and more responsibility for various ongoing oversight. If you're interested in helping out, either in general, or with a specific issue that you'd like to see resolved, please contact us using the information below!

Strictly speaking, you do not even need to be a member of the infrastructure team to manage a Haskell.org service - many smaller, independent services are operated by people not on the infrastructure team, many on the same machines we tend to manage. You may certainly run a service with us on your own machine too (and we may provide you a DNS entry, for example). However, the infrastructure team generally carefully overlooks most changes made across the infrastructure to all core services and machines, and we prefer to automate in-house work where applicable. Most questions about the infrastructure are also handled by the team directly.

### The team and how to contact them

Status is available for haskell services at http://status.haskell.org and http://auto-status.haskell.org

The current core team is:

*  Gershom Bazerman (co-lead) (@gershomb)
*  Davean Scies (co-lead) (@davean)
*  Herbert Valerio Riedel (@hvr)
*  Rick Elrod (@relrod)

You can contact the current team at any time with an email to admin@haskell.org, or hit them up on IRC (#haskell-infrastructure on https://libera.chat/).

### Infrastructure providers
Haskell.org uses many service providers for its infrastructure.

* [Packet.com](https://www.packet.com/) provides compute, storage, and networking resources, powering almost all of Haskell.org in several regions around the world. 
* [Fastly](https://www.fastly.com/) provides low latency access for all of Haskell.org's downloads and highest traffic services, including the primary Hackage server, and Haskell Platform/GHC downloads.
* [CloudFlare](https://www.cloudflare.com/) provides DNS management, Anti-DDoS, and high-grade frontend SSL and caching for most of Haskell.org
Status.io powers https://status.haskell.org, and lets us easily tell you when we broke something.
* [DreamHost](https://www.dreamhost.com/) supports Haskell.org by providing free and unlimited object storage and bandwidth via DreamObjects, which we use to stash logs, perform backups, and generally host all kinds of long-term content that we might need.

