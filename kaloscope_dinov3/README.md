# Vendored DINOv3 inference code

Copied from the sibling kaloscope-dinov3 repository: dinov3 hub, models, layers,
utils. The required backbone factory and deterministic image transforms were
extracted into architecture.py and preprocessing.py. Absolute imports use the private
kaloscope_dinov3 namespace to avoid other ComfyUI extensions' dinov3 packages.
No fine-tuning model, training scope controls, datasets, data augmentation,
optimizers, losses or training entry points are included. Loading is offline
(pretrained=False). Core model/layer definitions retain the original architecture
implementation to preserve checkpoint compatibility.

The original copyright headers and DINOv3 License Agreement (LICENSE.md) apply
to these files. Other plugin code retains its existing license.
