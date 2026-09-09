## JK

Infrastructure engineer working on Solana validator operations and Linux networking. Rust.

I run a testnet validator on bare metal and build the tooling around it.

- Validator dashboard: [vyralabs.fun/dashboard](https://vyralabs.fun/dashboard)

### Validator tooling

Built for a validator I actually operate, at [@vyralabshq](https://github.com/vyralabshq).

| Project | What it does |
|---|---|
| [driftwatch](https://github.com/vyralabshq/driftwatch) | eBPF profiler for disk I/O on Solana validator nodes |
| [agave-tap](https://github.com/vyralabshq/agave-tap) | Reads Agave datapoint log lines and converts them to InfluxDB line protocol, roughly 100 measurements a second |
| [preflight](https://github.com/vyralabshq/preflight) | Read only preflight check for validator hosts. Tells you what is wrong before you start the node |
| [vyralabs](https://github.com/vyralabshq/vyralabs) | The site and the public validator dashboard |

### Systems work

| Project | What it is |
|---|---|
| [Sol-Indexer](https://github.com/jkrishnad/Sol-Indexer) | Solana indexer built on the Yellowstone Geyser gRPC stream |
| [gossip-explorer](https://github.com/jkrishnad/gossip-explorer) | Explores the Solana gossip network |
| [mini-validator](https://github.com/jkrishnad/mini-validator) | Simplified Solana validator pipeline in Rust, built to see how the stages fit together |
| [banking-jitter-harness](https://github.com/jkrishnad/banking-jitter-harness) | Measures jitter in the banking stage |
| [Event-Ingestion](https://github.com/jkrishnad/Event-Ingestion) | High throughput, low latency ingestion service |
| [matching-engine](https://github.com/jkrishnad/matching-engine) | Real time order matching engine |
| [Token-Program](https://github.com/jkrishnad/Token-Program) | Reimplementation of the token program |
| [QUIC-Implementation](https://github.com/jkrishnad/QUIC-Implementation) | QUIC client and server, written to understand the transport Solana uses |
| [SMTP](https://github.com/jkrishnad/SMTP) | SMTP server in Rust |

### eBPF and XDP

| Project | What it is |
|---|---|
| [xdp-with-aya](https://github.com/jkrishnad/xdp-with-aya) | XDP packet filter using Aya |
| [packet-counter](https://github.com/jkrishnad/packet-counter) | eBPF packet counter |
| [xdp-log](https://github.com/jkrishnad/xdp-log) | XDP logging program |

Wrote a series on how eBPF programs are actually built: [Aya project structure](https://jkrishna.xyz/blogs/deep-dive-into-aya-project-structure), [writing eBPF programs](https://jkrishna.xyz/blogs/learning-ebpf-chapter-2), [anatomy of eBPF programs](https://jkrishna.xyz/blogs/learning-ebpf-chapter-3).

### Open source

Merged contributions in:

| Project | What it is |
|---|---|
| [solana-foundation/surfpool](https://github.com/solana-foundation/surfpool) | Local Solana development environment |
| [otter-sec/anchor](https://github.com/otter-sec/anchor) | The Anchor framework |
| [boa-dev/boa](https://github.com/boa-dev/boa) | JavaScript engine written in Rust |
| [gillsdk/gill](https://github.com/gillsdk/gill) | Solana JavaScript and TypeScript SDK |
| [samui-build/samui-wallet](https://github.com/samui-build/samui-wallet) | Open source Solana wallet |
| [blueshift-gg/Scilla](https://github.com/blueshift-gg/Scilla) | Solana tooling |
| [solana-rpc/superbank](https://github.com/solana-rpc/superbank) | Solana ledger RPC stack |
