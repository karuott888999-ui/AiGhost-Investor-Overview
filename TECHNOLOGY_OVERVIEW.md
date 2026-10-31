# AiGhost — Technology Overview

## 1. Product layer: Ghost

The existing repository describes Ghost as a privacy-first social messaging application. AiGhost's broader product direction adds a local-first intelligence layer and a user-controlled home-node concept. This public overview intentionally stays at product and architecture level; it does not expose implementation source, credentials, internal endpoints, or deployment instructions.

## 2. Local-first intelligence

The current self-development architecture specifies local inference as the preferred path and treats local memory as a durable store for selected system context. The design aims to keep inference on a user-controlled host where a compatible local model is configured.

This is an architecture and development track, not a blanket claim that all users' devices have adequate compute, that every feature operates offline, or that autonomous self-development is production-proven. Device compatibility, model availability, resource limits, permissions, and safe update controls must be validated per deployment.

## 3. Ghost Home Node

The repository documents a consent-gated node registry and bounded store-and-forward packet queue. The current pilot is intentionally narrow:

- only devices whose owners opt in may be enrolled;
- sender and recipient nodes must belong to the same AiGhost account;
- packet size, queue size, and expiry are bounded;
- node tokens are displayed once and only their hashes are persisted by the service;
- a node owner can revoke participation;
- the network does not silently scan, enrol, remotely control, or repurpose a device.

The documented pilot is not a public VPN, Tor exit, internet proxy, general file-sharing service, public carrier network, or promise of continuous availability. The device's node client must be running for it to participate. A signed Windows/macOS installer and fully automated cross-platform onboarding remain future work.

## 4. Neuroplasma Optical Fabric

Neuroplasma is a software research model for a possible hybrid optical/electronic fabric. Its software architecture distinguishes:

- **transport:** carrying a modulated signal through an optical path;
- **active processing:** controlled switching, modulation, wavelength conversion, or electronic/photonic processing at a node;
- **temporary optical buffering:** holding a signal in transit for a bounded delay;
- **persistent memory:** storing an addressable state in a suitable memory device.

A passive fibre or mirror does not inspect software headers, execute arbitrary code, or provide general-purpose RAM. A real system would require suitable active devices, control electronics, physical memory technologies, optical components, secure control, and laboratory validation.

### Current software demonstration

The engineering note dated 2026-10-30 records an isolated five-role software loopback: source, coordinator, wavelength-selective junction, mirror, and receptor. The model represents a forward 1550 nm channel and a return 1310 nm channel over a modelled 95 m combined path, with a simulated round-trip delay of approximately 465 ns.

**These values are outputs of a software model, not measurements of a physical AiGhost optical link.** No physical transceiver, fibre segment, optical NIC, live socket, or optical bridge was used in that demonstration.

### Security model in the prototype

The engineering note records tests for AES-256-GCM and ChaCha20-Poly1305 authenticated encryption, including rejection of invalid keys and tampered authenticated headers/ciphertext. Key provisioning, secure distribution, rotation, and recovery are not yet implemented. A passing encryption test is not equivalent to a production key-management system or independent security certification.

## 5. Research boundaries

Neuroplasma is a software prototype and research direction. Physical optical transport, optical switching, non-volatile optical memory, device packaging, power/thermal budgets, reliability, manufacturing, and cost remain open engineering topics. These should be evaluated with qualified optical and hardware specialists before any physical-performance claim is made.
