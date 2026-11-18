# AI Models & Open-Source Notices

Brightcraft runs on-device AI models and open-source Swift packages under their respective open-source licenses.

## On-Device AI Models & Runtimes

| Component | Source | Role |
| --- | --- | --- |
| **Apple Foundation Models** | Apple Inc. (iOS / iPadOS system framework) | Built-in Free-tier local text & structured generation on Apple Intelligence-capable hardware |
| **LiquidAI LFM2.5-VL 450M** (`Q8_0` GGUF + `mmproj`) | [LiquidAI / Hugging Face](https://huggingface.co/LiquidAI/LFM2.5-VL-450M-GGUF) | Universal Free-tier edge multimodal vision + language model via `llama.cpp` |
| **LiquidAI LFM3-VL 2B** (`QAD-Q4_0` GGUF + `mmproj`) | [LiquidAI / Hugging Face](https://huggingface.co/LiquidAI/LFM3-VL-2B-GGUF) | Pro-tier multimodal reasoning model with `<think>` step-by-step analysis via `llama.cpp` |
| **llama.cpp & libmtmd** | [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) (MIT License) | Local Metal-accelerated GGUF + multimodal projector inference runtime |

## Open-Source Swift Packages

- **archon-swift** (`ArchonCore`, `ArchonAgent`, `ArchonSearch`, `ArchonContext`, `ArchonConnect`, `ArchonMemory`, `ArchonSandbox`) — [github.com/VM451/archon-swift](https://github.com/VM451/archon-swift)
- **GRDB.swift** — [github.com/groue/GRDB.swift](https://github.com/groue/GRDB.swift) (MIT License)
- **mcp-swift-sdk** — [github.com/modelcontextprotocol/swift-sdk](https://github.com/modelcontextprotocol/swift-sdk) (MIT License)
- **ProximaKit** — [github.com/vivekptnk/ProximaKit](https://github.com/vivekptnk/ProximaKit)
- **EventSource** — [github.com/mattt/EventSource](https://github.com/mattt/EventSource) (MIT License)
- **yyjson** — [github.com/ibireme/yyjson](https://github.com/ibireme/yyjson) (MIT License)
- **swift-collections / swift-crypto / swift-log / swift-nio / swift-numerics / swift-asn1 / swift-atomics / swift-system** — Apple Inc. (Apache License 2.0)
- **swift-huggingface / swift-transformers / swift-jinja** — Hugging Face (Apache License 2.0)
- **mlx-swift / mlx-swift-lm** — MLX Contributors (MIT License; transitive dependency)

## Responsible AI Notice

On-device model outputs are generated probabilistically on local hardware and should be reviewed carefully before making business, financial, or legal commitments.
