# MLIR-AIR docs (Xilinx/mlir-air)

Mirror of the published MLIR-AIR documentation pages from
[Xilinx/mlir-air](https://github.com/Xilinx/mlir-air) `docs/` (publishes
https://xilinx.github.io/mlir-air/dev/). MLIR-AIR is AMD's spatial-compile
MLIR framework for mapping AI workloads onto AMD NPUs and Versal AI Engine
arrays.

**Sync:** `sync-knowledge.sh` pulls the upstream clone (`~/amd-oss/mlir-air`)
and refreshes this folder; the repo's GitHub Action then refreshes Context7.

Position vs the other docs: DESCENT.md §7 — MLIR-AIE is the shared substrate
of the AMD NPU stack; MLIR-AIR is NOT it (IRON bypasses AIR entirely, zero
`air.*` imports). MLIR-AIR's role is the spatial-compile / AIE-array mapping
layer. Loom (docs/hrx-loom/) is the runtime kernel JIT; FastFlowLM
(docs/fastflowlm/) is the NPU-native inference runtime.
