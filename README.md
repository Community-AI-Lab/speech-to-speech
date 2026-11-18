# Community AI Lab — Speech-to-Speech

An open-source effort to adapt **Qwen3-Omni** for low-latency, **full-duplex speech-to-speech**: the assistant listens while speaking, handles interruptions, understands group conversations and produces a live transcript of the user's speech.

**[Proposed architecture and diagram](docs/architecture.md)**

## Proposed development work

- [Full-duplex model adaptation](https://github.com/Community-AI-Lab/speech-to-speech/issues/9): causal/streaming audio, natural turn-taking, interruptions, group conversation and live user transcription.
- [TensorFold audio inference](https://github.com/Community-AI-Lab/speech-to-speech/issues/10): real-time serving and bidirectional audio sessions, with MLX or other runtime options as appropriate.
- [Training and evaluation harness](https://github.com/Community-AI-Lab/speech-to-speech/issues/11): reproducible data preparation, model training, checkpoints and objective benchmarks.
- [Distributed training](https://github.com/Community-AI-Lab/speech-to-speech/issues/12): use the same training harness with multi-GPU coordination; investigate **[Hivemind](https://github.com/learning-at-home/hivemind)** as a candidate.
- [Audio datasets and consent](https://github.com/Community-AI-Lab/speech-to-speech/issues/4): data provenance, permissions and quality.

**Training and inference are separate.** Training and model-specific experiments live in this repository. [Platform ModelOps](https://github.com/Community-AI-Lab/platform/issues/7) governs approval, releases and publication of trained artifacts to the Hugging Face Hub. TensorFold (or another selected runtime) loads published models for real-time inference; Hugging Face Hub publication is not itself an inference API.

## First milestone

Verify a spoken request → validated tool call → actual tool result → spoken answer, with reproducible evaluation. Extend that baseline to continuous listening, interruptions and group speech.

## Contributing

See the [project issues](https://github.com/Community-AI-Lab/speech-to-speech/issues) and [contribution notes](CONTRIBUTING.md). Submit only code and audio you are authorised to share. Contributor credits and commercial rights are governed separately by the Community AI Lab Platform and approved agreements.
