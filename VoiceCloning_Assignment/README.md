
# Voice Cloning Project (OpenVoice)

This project provides a Google Colab–ready pipeline to perform voice cloning using **OpenVoice** (openvoice-cli) and to document the full experimental run required by your task.

## Deliverables this repo helps produce
- GitHub repo with code and notebook
- Error log document (`docs/error_log.md`)
- 30-second audio sample (original vs cloned) in `samples/`
- Brief report (`docs/report.md`) describing what worked, what failed, suggestions, and resource usage

## How to run (Colab)
1. Upload this folder `VoiceCloning_OpenVoice_v2.zip` to Colab and unzip (or paste notebook cells directly).
2. Run the notebook `notebooks/voice_cloning_colab.ipynb`. It will:
   - install dependencies (PyTorch + openvoice-cli)
   - download checkpoints (OpenVoiceV2) via git LFS from Hugging Face
   - allow you to upload a reference voice and an input narration (or reuse the same file)
   - automatically trim/pad to 30s and run cloning
   - save `samples/cloned_30s.wav` and `samples/original_30s.wav`

## Notes
- The notebook expects a GPU runtime in Colab (Runtime → Change runtime type → GPU).
- If you have large amounts of audio (recommended 30 min–3 hours), quality improves. The notebook supports using shorter samples (>=30s) for quick tests.
