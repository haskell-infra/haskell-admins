# Haskell Infrastructure Admins

The infrastructure team is ultimately responsible for maintaining Haskell.org services. It is not required you be a member of any existing group (for example, the Haskell.org committee) to join. The infrastructure team deals solely with technical aspects of Haskell.org infrastructure, including sensitive matters like domain management, backups, administrative email, security response, service allocation, and domain or URL routing.

Strictly speaking, you do not even need to be a member of the infrastructure team to manage a Haskell.org service - many smaller, independent services are operated by people not on the infrastructure team, many on the same machines we tend to manage. You may certainly run a service with us on your own machine too (and we may provide you a DNS entry, for example). However, the infrastructure team generally carefully overlooks most changes made across the infrastructure to all core services and machines, and we prefer to automate in-house work where applicable. Most questions about the infrastructure are also handled by the team directly.

Status is available for haskell services at http://status.haskell.org and http://auto-status.haskell.org

The current team is:

Gershom Bazerman (@gershomb)
Ricky Elrod (@relrod)
Herbert Valerio Riedel (@hvr)
Davean Scies (@davean)
You can contact the current team at any time with an email to admin@haskell.org, or hit them up on IRC (#haskell-infrastructure on freenode).

### Infrastructure providers
Haskell.org uses many service providers for its infrastructure.

Packet.com provides compute, storage, and networking resources, powering almost all of Haskell.org in several regions around the world. 
Fastly provides low latency access for all of Haskell.org's downloads and highest traffic services, including the primary Hackage server, and Haskell Platform/GHC downloads.
CloudFlare provides DNS management, Anti-DDoS, and high-grade frontend SSL and caching for most of Haskell.org
Status.io powers https://status.haskell.org, and lets us easily tell you when we broke something.
DreamHost supports Haskell.org by providing free and unlimited object storage and bandwidth via DreamObjects, which we use to stash logs, perform backups, and generally host all kinds of long-term content that we might need.

### Service details

Here are some of the services the infra team maintains.

www.haskell.org - the primary website
wiki.haskell.org - Our MediaWiki instance, hosting tons of content.
hackage.haskell.org - The primary Hackage instance for Haskell.org; this setup is proxied in the front by Fastly, to provide low-latency downloads and caching for Hackage
mail.haskell.org - Serving a variety of haskell-related mailing lists
planet.haskell.org - Our Planet Venus instance, which powers the Haskell.org community RSS feeds.
downloads.haskell.org - A downloads server hosting tons of static content, proxied by Fastly.
archives.haskell.org - archives of decommissioned sites and services related to the open-source Haskell community.
ghc.haskell.org & git.haskell.org - The GHC git repositories and Trac system.
community.haskell.org & projects.haskell.org - Our legacy community infrastructure
status.haskell.org - A service providing status updates on haskell.org infrastructure issues (provided by status.io).
