# zkdeal

Application-specific validity rooms for bounded, multi-step workflows that settle to Ethereum as a single checkpoint.

zkdeal lets an application define its participants, permitted inputs, ordering policy, deadline, and close conditions inside a room-local EVM. One proof binds the batch before Ethereum accepts the result.

## Start here

- [Website](https://zkdeal.org)
- [Yellow paper](https://zkdeal.org/yellow-paper/)
- [Protocol brief PDF](https://zkdeal.org/zkdeal-vs-zk-l2-technology-brief.pdf)
- [Repository catalog](https://zkdeal.org/repositories/)
- [Hands-on tutorials](https://zkdeal.org/blog/)
- [Docker images](https://zkdeal.org/docker-images/)
- [Docker Hub](https://hub.docker.com/u/zkdeal)

## Motivational examples

Architecture becomes useful when it answers a concrete question. These seven
small runs start with the question, keep the command and result together, and
link the code to the boundary it exercises. Open an Asciinema recording to
pause the terminal and copy its text; use the transcript for scanning or the
VHS tape to reproduce the presentation. “Motivates” names the repository
boundary illuminated by the example; a full-stack recording may run linked
owner repositories rather than that deployment repository itself.

| Question | Motivates | Recording sources |
| --- | --- | --- |
| Is this the exact native CUDA prover, with no CPU fallback? | [`zkdeal-prover`](https://github.com/zkdeal/zkdeal-prover) | [Prover Asciinema](https://zkdeal.org/blog/run-the-supplied-zkdeal-docker-stack/#terminal-recording) · [prover transcript](https://zkdeal.org/blog/terminal/vii-docker-prover-smoke.txt) · [prover VHS tape](https://zkdeal.org/blog/terminal/vii-docker-prover-smoke.tape) |
| What full-stack baseline should a deployment preserve? | [`zkdeal-cloud-deployer-infra`](https://github.com/zkdeal/zkdeal-cloud-deployer-infra) (the run uses `zkdeal-testing`) | [Full-stack Asciinema](https://zkdeal.org/blog/specialized-validity-systems-and-stage-aligned-room-profiles/#terminal-recording) · [full-stack transcript](https://zkdeal.org/blog/terminal/vi-profile-and-fallback-checks.txt) · [full-stack VHS tape](https://zkdeal.org/blog/terminal/vi-profile-and-fallback-checks.tape) |
| What is the smallest useful room application? | [`zkdeal-examples`](https://github.com/zkdeal/zkdeal-examples) | [Minimal-app Asciinema](https://zkdeal.org/blog/zkdeal-vs-shared-l2-proof-stacks/#terminal-recording) · [minimal-app transcript](https://zkdeal.org/blog/terminal/v-room-node-boundary.txt) · [minimal-app VHS tape](https://zkdeal.org/blog/terminal/v-room-node-boundary.tape) |
| Does one actor's custody and accounting balance in the focused Foundry model? | [`zkdeal-protocol`](https://github.com/zkdeal/zkdeal-protocol) | [Liquidity Asciinema](https://zkdeal.org/blog/three-ways-capital-returns-to-ethereum-l1/#terminal-recording) · [liquidity transcript](https://zkdeal.org/blog/terminal/iv-capital-return-contract-tests.txt) · [liquidity VHS tape](https://zkdeal.org/blog/terminal/iv-capital-return-contract-tests.tape) |
| What changes when an app chooses FIFO instead of priority ordering? | [`zkdeal-node`](https://github.com/zkdeal/zkdeal-node) | [Ordering Asciinema](https://zkdeal.org/blog/prove-the-market-rule-you-choose/#terminal-recording) · [ordering transcript](https://zkdeal.org/blog/terminal/iii-market-rule-mev.txt) · [ordering VHS tape](https://zkdeal.org/blog/terminal/iii-market-rule-mev.tape) |
| How do one-shot and continuing rooms differ after a checkpoint? | [`zkdeal-coordinator`](https://github.com/zkdeal/zkdeal-coordinator) | [Lifecycle Asciinema](https://zkdeal.org/blog/one-checkpoint-clear-to-eight-hour-market/#terminal-recording) · [lifecycle transcript](https://zkdeal.org/blog/terminal/ii-room-lifecycle-gates.txt) · [lifecycle VHS tape](https://zkdeal.org/blog/terminal/ii-room-lifecycle-gates.tape) |
| How do I know an accepted checkpoint is final and visible in Blockscout? | [`zkdeal-testing`](https://github.com/zkdeal/zkdeal-testing) | [Evidence Asciinema](https://zkdeal.org/blog/more-than-a-transaction-less-than-a-chain/#terminal-recording) · [evidence transcript](https://zkdeal.org/blog/terminal/i-public-checkout-and-gates.txt) · [evidence VHS tape](https://zkdeal.org/blog/terminal/i-public-checkout-and-gates.tape) |

## Core repositories

- [Examples](https://github.com/zkdeal/zkdeal-examples)  auctions, shops, private card play, FIFO, and commit reveal ordering
- [Node](https://github.com/zkdeal/zkdeal-node)  execution, networking, proving, settlement, and recovery
- [Protocol](https://github.com/zkdeal/zkdeal-protocol)  Ethereum verification, accounting, and asset movement
- [Testing](https://github.com/zkdeal/zkdeal-testing)  local Ethereum, Blockscout, coordinator, and CUDA prover stack
- [Cloud deployment](https://github.com/zkdeal/zkdeal-cloud-deployer-infra)  Compose, Kubernetes, observability, backup, and failover

> **Project status:** zkdeal is not a general-purpose L2. There is no public testnet or external security review yet. Repository licenses vary; check each repository before use.
