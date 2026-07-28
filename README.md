# Inesh Reddy Chappidi

LLM inference engineer. I make big models run fast and cheap on NVIDIA GPUs.

📍 SF Bay Area | 📧 ineshreddy249@gmail.com | [LinkedIn](https://linkedin.com/in/ineshreddy) | [GitHub](https://github.com/IneshReddy249)

---

## What I've Shipped

**Meta — AI Systems Co-Design Intern** *(Sep–Dec 2025)*  
- FP8 quantization on LLaMA-3.1-8B @ H100: **1.8× throughput**, `&lt;0.5%` ppl drop.  
- Disaggregated prefill-decode for DeepSeek-R1: **p99 TTFT −52%**, **95% decode GPU util** sustained.

**Tata Elxsi — ML Engineer** *(2020–2023)*  
- Two-stage serving (ANN + XGBoost) on AWS ECS/K8s: **2M+ inferences/day**.  
- **P95 latency 150ms → 100ms** via batching + Redis caching.

---

## Projects That Moved Numbers

**Llama-3.1-8B on H100** *(TensorRT-LLM)*  
- TTFT **48ms → 13ms**. Throughput **440 → 1,700+ tok/s**. GPU util **58% → 94%**.  
- Nsight showed CPU launch gaps. Swapped in DeepGEMM + FlashAttention-3.

**EAGLE3 Speculative Decoding** *(SGLang, H100)*  
- **1.34× speedup** at low concurrency. MTP + SpecV2: **1.28× at high batch** (980 → 1,255 tok/s).  
- Draft trees: 16-token vs 6-token trees cut MoE throughput **11.5%** despite **+21% accept rate** — routing overhead per rejected token is real.

**CUDA Kernels** *(Tensara)*  
- FP8 GEMM: **12ms, 32K GFLOPS**, top-10.  
- GELU: **#3 globally**, 44μs, 16.7K GFLOPS on B200. Register tiling, float4 loads, warp-shuffle.

---

## Open Source

- **vLLM-Omni** [PR #4760/#4761](https://github.com/vllm-project/vllm-omni) — one-line codec fix + FlashInfer autotune disable. **18 GiB saved**, serves on single 80GB H100 at 196K context.  
- **vLLM-Omni** [PR #5132](https://github.com/vllm-project/vllm-omni) — fixed flaky CI perf test. Added warm-up + median-of-N.

---

## Certs

- NVIDIA DLI — CUDA C/C++ *(2025)*

---

## Education

**M.S. Computer Science** — Florida Atlantic University *(Dec 2025)*
