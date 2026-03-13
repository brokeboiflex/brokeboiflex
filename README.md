# Hey, I'm Marcel

Full-stack engineer and cognition researcher based in Poland.

I like building things that sit at uncomfortable intersections — browser extensions that need persistent state, native bindings for obscure NLP tools, middleware that untangles nested data, security audits for misconfigured backends. If it's fiddly and nobody wants to deal with it, I'm probably interested.

Most of my 85+ repos are private client and research work, but here's what I've put out in the open:

---

### Hermit

An AI agent runtime that gives every agent its own full virtual machine — not a container, not a sandbox, an actual QEMU-backed OS with its own kernel, filesystem, and network stack. Agents get persistent semantic memory (SQLite + FTS5), an encrypted vault for secrets, configurable network allowlists, and the ability to snapshot their entire state — RAM, disk, running processes — mid-execution into transferable artifacts. You can fork a snapshot and spin up a variant in seconds.

Orchestration happens through MCP tools and A2A agent cards, so agents can discover and talk to each other. There's a web dashboard for managing everything, a host MCP server for IDE integration, and Nix-based reproducible builds so environments are deterministic.

The long-term vision is the Hermit Network — a decentralized marketplace on Solana where agent blueprints and shells are published, shared, and governed on-chain via IPFS.

Built with Python, FastAPI, WebSocket, QEMU, SQLite, Solana, IPFS, MCP, and A2A.

[**hermit-images**](https://github.com/brokeboiflex/hermit-images) — Pre-built base images for Hermit. More coming soon.

---

### SFS — Simple File Storage

A three-package npm ecosystem that handles file uploads end to end. I built it because wiring up file uploads across the stack is tedious boilerplate that everyone rewrites from scratch.

[**sfs-node**](https://github.com/brokeboiflex/sfs-node) is the core — disk space checks, MIME type detection, UUID-based naming, and a clean API for storing and retrieving files. [**sfs-express**](https://github.com/brokeboiflex/sfs-express) wraps it into Express middleware so adding file upload support to a server is a one-liner. [**sfs-frontend**](https://github.com/brokeboiflex/sfs-frontend) is the React client that handles the upload UX and talks to the backend.

All three are published on npm and designed to work together or independently.

---

**[zustand-chrome-storage](https://github.com/brokeboiflex/zustand-chrome-storage)** solved my own headache with Chrome extension state — turns out other people had the same one. **[firebuster](https://github.com/brokeboiflex/firebuster)** came from finding too many wide-open Firebase instances. **[nodeusz](https://github.com/brokeboiflex/nodeusz)** bridges Polish morphological analysis into the JS ecosystem via C++ N-API because nobody else was going to do it.

I've also built a [JSX router](https://github.com/brokeboiflex/jar-preact) for Preact (and [React](https://github.com/brokeboiflex/jar-react)), [Strapi middleware](https://github.com/brokeboiflex/strapi-middleware-resolveNestedObjects) for painless nested object mutations, and a [Cloudflare Worker](https://github.com/brokeboiflex/woocommercemiddleware) for WooCommerce.

When I'm not shipping code I'm reading papers on cognitive enhancement and running experiments — the ORCID on my profile isn't decorative.

`TypeScript` `JavaScript` `Python` `C++` `Rust` `React` `Node.js` `Cloudflare Workers` `QEMU` `Solana` `FastAPI`
