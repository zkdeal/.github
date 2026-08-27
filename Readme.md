# zkdeal

Application-specific validity rooms for bounded, multi-step workflows that settle to Ethereum as a single checkpoint.

zkdeal lets an application define its participants, permitted inputs, ordering policy, deadline, and close conditions inside a room-local EVM. One proof binds the batch before Ethereum accepts the result.

## Start here

- [Website](https://zkdeal.org)
- [Yellow paper](https://zkdeal.org/yellow-paper/)
- [Technology brief](https://zkdeal.org/zkdeal-vs-zk-l2-technology-brief.pdf)
- [Repository catalog](https://zkdeal.org/repositories/)
- [Hands-on tutorials](https://zkdeal.org/blog/)
- [Docker images](https://zkdeal.org/docker-images/)0
- [Docker Hub](https://hub.docker.com/u/zkdeal)

## Core repositories

- [Examples](https://github.com/zkdeal/zkdeal-examples)  auctions, shops, private card play, FIFO, and commitâ€“reveal ordering
- [Node](https://github.com/zkdeal/zkdeal-node)  execution, networking, proving, settlement, and recovery
- [Protocol](https://github.com/zkdeal/zkdeal-protocol)  Ethereum verification, accounting, and asset movement
- [Testing](https://github.com/zkdeal/zkdeal-testing)  local Ethereum, Blockscout, coordinator, and CUDA prover stack
- [Cloud deployment](https://github.com/zkdeal/zkdeal-cloud-deployer-infra)  Compose, Kubernetes, observability, backup, and failover

> **Project status:** zkdeal is not a general-purpose L2. There is no public testnet or external security review yet. Repository licenses vary; check each repository before use.
