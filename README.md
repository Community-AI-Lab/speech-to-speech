# Community AI Lab — Speech-to-Speech

This is the first model project for [Community AI Lab](https://github.com/Community-AI-Lab/platform).

## Goal

Build a voice AI demo that accepts speech and produces spoken replies. We want to study low latency, naturalness and the ability to run locally on suitable hardware, with optional hosted inference.

Nothing is trained or deployed yet. **Start by evaluating existing models** with suitable licences rather than immediately pretraining a new one.

## Work to do

1. Set measurable targets: streaming latency, quality and hardware.
2. Evaluate candidate open-weight speech architectures and their licences.
3. Decide on safe, properly licensed and consented audio data.
4. Build a reproducible baseline and evaluation suite.
5. Improve training, fine-tuning, inference speed and model quality.
6. Store model artefacts on Hugging Face and test a hosted Inference Endpoint. Confirm support for real-time audio, potentially through a custom serving container.
7. Connect the demo and usage metrics to the contributor platform.

## First milestone

A reproducible local demo: microphone/audio file in, spoken response out, with installation instructions and measured latency. Next, test hosted inference.

## Contribute

Pick an [open issue](../../issues) and describe what you'll deliver. See [CONTRIBUTING.md](CONTRIBUTING.md). Audio contributors must have permission for submitted recordings, and participants must not submit employer-owned confidential material.

The contributor credit and commercial revenue-sharing rules are still being designed. No payout or ownership rights are promised at this stage.
