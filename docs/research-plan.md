# Speech-to-speech research plan

## Goal

A reproducible voice demo, with spoken input and spoken output, tested for naturalness and latency. Local inference first; managed hosted inference next if suitable.

## Track A: baseline and evaluation

- List candidate audio architectures and licences, covering both modular ASR → language model → TTS and direct speech-to-speech approaches.
- Define minimum hardware and latency targets.
- Build a tiny, reproducible demo with a fixed evaluation set; record first-audio and end-to-end response latency.

## Track B: data and training

- Document allowed datasets, rights, recording consent, provenance and usage limitations.
- Prepare data preprocessing and validation scripts.
- Test fine-tuning on an existing legally usable model before attempting pretraining.

## Track C: deployment

- Run locally with documented dependencies.
- Publish versioned weights to Hugging Face only after permissions are confirmed.
- Assess Hugging Face Inference Endpoints, streaming requirements, cold starts, cost and potential custom serving.
- Integrate the endpoint with the Community AI Lab platform for auth, metering and billing once ready.

## Initial acceptance test

From a clean checkout, an engineer can run one documented command or procedure that sends a short audio clip and receives spoken output. Record the model and dataset licences, GPU, RAM, duration, voice quality observations and latency.

No particular model, dataset, hosting provider or target hardware has been approved yet.
