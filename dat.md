# dat info

A repo to collect and organize info about [dat][dat] in a way that makes sense to me.

[dat]: https://docs.datproject.org

## Anatomy of a dat

### Core modules

- [hypercore-protocol](https://github.com/mafintosh/hypercore-protocol) - A node duplex stream that implements the hypercore protocol
- [Hypercore](https://github.com/mafintosh/hypercore) - Append only logs using over the hypercore protocol
- [Hyperdrive](https://github.com/mafintosh/hyperdrive) - Versioned and syncable file archives built with hypercores
- [dat-node](https://github.com/datproject/dat-node) - A dat client as a library.  Used to manage a single dat from a library.
  - [dat-node@hyperdb](https://github.com/datproject/dat-node/blob/hyperdb/examples/download.js) - the dat-node with hyperdb baked in.
- [multidat](https://github.com/dat-land/multidat) - A lib for managing multiple dats from a library.

### Storage providers

- [random-access-storage/random-access-storage](https://github.com/random-access-storage/random-access-storage) - abstract random access api
- [random-access-file](https://github.com/random-access-storage/random-access-file)
- [mafintosh/random-access-memory](https://github.com/mafintosh/random-access-memory)

### Networking layers

- [mafintosh/signalhub](https://github.com/mafintosh/signalhub) -
Simple signalling server that can be used to coordinate handshaking with webrtc or other fun stuff.  Needed for discovery-channel to operate.
- [discovery-channel](https://github.com/maxogden/discovery-channel) - look for peers at a key, and announce your presence.
- [discovery-swarm](https://github.com/mafintosh/discovery-swarm) - Discover peers at a key, and node duplex stream with them.
- [mafintosh/discovery-server](https://github.com/mafintosh/discovery-server) - A tcp/utp server that auto announces itself using discovery-channel. Basically a server-only version of discovery-swarm
- [dat-swarm-defaults](https://github.com/datproject/dat-swarm-defaults) - Defaults for dns and dht servers
- [karissa/hyperdiscovery](https://github.com/karissa/hyperdiscovery) - Pass a hypercore or hyperdrive in, and it will join a swarm and repliacte.

### Dat tools

- [karissa/hyperhealth](https://github.com/karissa/hyperhealth) - monitor hyperfeed stats

### Viz

- [karissa/hypercore-stats-server](https://github.com/karissa/hypercore-stats-server)
- [mafintosh/hypercore-stats-ui](https://github.com/mafintosh/hypercore-stats-ui)
- [jimpick/vizceral-hypercore-stats](https://github.com/jimpick/vizceral-hypercore-stats)
  - using: https://github.com/Netflix/vizceral

### Roll your own dat

- https://github.com/mafintosh/dat-next-next/blob/master/index.js

## Apps

### End user Dat applications

- [dat-desktop][dat-desktop] - Desktop torrent client for dats
- [dat-cli][dat-cli] - a cli dat client
  - [dat-next](https://github.com/joehand/dat-next): next version of dat cli with hyperdb

[dat-desktop]: https://github.com/dat-land/dat-desktop
[dat-cli]: https://github.com/datproject/dat

### End user hypercore apps

- [hyperirc](https://github.com/mafintosh/hyperirc) - an irc client that stores logs into a hyperdrive
- [hyperirc-www](https://github.com/mafintosh/hyperirc-www) - a static webapp that displays hyperirc logs via webrtc
- [louiscenter/hypercast](https://github.com/louiscenter/hypercast) - a video streaming system.

## Beaker projects using dat

- [webdb](https://github.com/beakerbrowser/webdb) - a dat client with indexing and schema validation

## Orgs + Owners

Dat uses lots of orgs and people's github accounts to store code and projects.

### Dat Orgs, Owners and Purpose

- [datproject][datproject] - "A distributed data community": Core org
- [Dat Community/dat-land][dat-land] - "Community tools and projects built with Dat" "DAT'S HACKER COMMUNITY"
- [Dat Protocol Specification][datproto] - Dat protocol development org

[dat-land]: https://github.com/dat-land
[datproject]: https://github.com/datproject
[datproto]: https://github.com/datprotocol

### Auxiliary Orgs and Owners

- [random-access-storage][ras] - Random Access Storage projects and community
- [Home Prebuilders Association][hpa] - Organization for tools to prebuild native node modules for all versions of node and electron.
- [sodium friends][https://github.com/sodium-friends] - Javascript friends of libsodium
- [mafintosh/abstract-encoding](https://github.com/mafintosh/abstract-encoding) - abstract encoding family
- [mafintosh/abstract-chunk-store](https://github.com/mafintosh/abstract-chunk-store) - abstract chunk store
- [maxogden/abstract-blob-store](https://github.com/maxogden/abstract-blob-store) - abstract blob store

[ras]: https://github.com/random-access-storage
[hpa]: https://github.com/prebuild

### History

- [bnewbold/dat-early-days](https://github.com/bnewbold/dat-early-days) - collection of interesting Dat and beaker milestones as well as early rotonde links.
- [mafintosh/awesome-p2p](https://github.com/mafintosh/awesome-p2p) - a small collection of p2p links.
- [cblgh/decent-dat-intro](https://github.com/cblgh/decent-dat-intro) - a collection of beaker apps and a corresponding lecture.
