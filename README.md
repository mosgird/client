# Mosgird desktop

The desktop client of the Mosgird protocol. The specification is in mosgird/protocols.

**Status:** not started. No code yet.

**License:** Mulan Permissive Software License, Version 2 (Mulan PSL v2). See [LICENSE.md](LICENSE.md).

## Specification

The protocol is specified in [mosgird/protocols](https://github.com/mosgird/protocols). This repository implements that specification. When the two disagree, the specification wins, and the difference is a bug to fix here or a change to propose there. Users and developers should read the specification before relying on any behavior of this software.

## What the client does

The protocol has no server and uses no domain names ([decision 0005](https://github.com/mosgird/protocols/blob/main/spec/decisions/0005-serverless-online-only-delivery.md), proposed). The client is therefore the whole system on the user's side. It holds the user's keys, encrypts and decrypts, delivers ciphertext directly to other devices while both are reachable, and keeps undelivered ciphertext until it is delivered. The transport, group protocol, and moderation design are still open in the specification. This client implements none of them until they are decided there.


## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Rules for AI tools and agents are in the protocol repository.
