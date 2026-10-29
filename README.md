## JK

Infrastructure engineer working on Solana validator operations and Linux networking. Rust.

I ran a Solana testnet validator on bare metal for 117 days (6,904 blocks, 12 skipped) and built the tooling around it. Now building shred tooling and writing up what the node taught us.

- Field notes: [vyralabs.fun/logs](https://vyralabs.fun/logs)

### Shred tooling

Read the shreds reaching a validator, verify them, rebuild the blocks.

| Project | What it does |
|---|---|
| [shredcore](https://github.com/vyralabshq/shred-core) | Rust libraed packets, get back verified slots and transactions |
| [shredtap](https://github.com/jkrishnad/shred-tap) | Live shred decoder and dashboard. Rebuilds FEC sets, checks Merkle proofs and leader signatures, turns shreds into blocks |
| [shredwire](https://github.com/jkrishnad/shred-wire) | Verifies every shred off the wire and streams each transaction over gRPC the moment its batch completes |

### Validator tooling

Built for the validator I operated at [@vyralabshq](https://github.com/vyralabshq).

| Project | What it does |
|---|---|
| [preflight](https://github.com/vyralabshq/preflight) | Read only preflight check for validator hosts. 40 checks, tells you what is wrong before you start the node|
| [driftwatch](https://github.com/vyralabshq/driftwatch) | eBPF profiler for disk I/O on Solana validator nodes |
| [agave-tap](https://github.com/vyralabshq/agave-tap) | Reads Agave nverts them to InfluxDB line protocol, roughly 100 measurements asecond |
| [vyralabs](https://github.com/vyralabshq/vyralabs) | The Vyra Labs

### Systems work

| Project | What it is |
|---|---|
| [sol-indexer](https://github.com/vyralabshq/sol-indexer) | Solana istone Geyser gRPC stream |
| [gossip-explorer](https://github.com/jkrishnad/gossip-explorer) | Minimal Rust spy node that explores the Solana gossip network |
| [mini-validator](https://github.com/jkrishnad/mini-validator) | Simipeline in Rust, built to see how the stages fit together |
| [banking-jitter-harness](https://github.com/jkrishnad/banking-jitter-harness) | Measures Agave banking-stage timing against the Votor slot budget |
| [Event-Ingestion](https://github.com/jkrishnad/Event-Ingestion) | Hy ingestion service |
| [matching-engine](https://github.com/jkrishnad/matching-engine) | Real time order matching engine |
| [Token-Program](https://github.com/jkrishnad/Token-Program) | Reimprogram |
| [QUIC-Implementation](https://github.com/jkrishnad/QUIC-Implementation) | QUIC client and server, written to understand the transport Solana uses |
| [SMTP](https://github.com/jkrishnad/SMTP) | SMTP server in Rust |

### eBPF and XDP

| Project | What it is |
|---|---|
| [xdp-with-aya](https://github.com/jkrishnad/xdp-with-aya) | XDP pac
| [packet-counter](https://github.com/jkrishnad/packet-counter) | eBPF packet counter |
| [xdp-log](https://github.com/jkrishnad/xdp-log) | XDP logging progr

Wrote a series on how eBPF programs are actually built: [Aya project a.xyz/blogs/deep-dive-into-aya-project-structure), [writing eBPFprograms](https://jkrishna.xyz/blogs/learning-ebpf-chapter-2), [anatomy of eBPF programs](https://jkrishna.xyz/blogs/learning-ebpf-chapter-3).

### Open source

Merged contributions in:

| Project | What it is |
|---|---|
| [solana-foundation/surfpool](https://github.com/solana-foundation/surfpool) | Local Solana development environment |
| [otter-sec/anchor](https://github.com/otter-sec/anchor) | The Ancho
| [boa-dev/boa](https://github.com/boa-dev/boa) | JavaScript engine written in Rust |
| [gillsdk/gill](https://github.com/gillsdk/gill) | Solana JavaScript
| [samui-build/samui-wallet](https://github.com/samui-build/samui-wallet) | Open source Solana wallet |
| [blueshift-gg/Scilla](https://github.com/blueshift-gg/Scilla) | Sol
| [solana-rpc/superbank](https://github.com/solana-rpc/superbank) | Solana ledger RPC stack |
