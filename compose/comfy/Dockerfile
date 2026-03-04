FROM python:3

RUN pip install comfy-cli
RUN comfy --skip-prompt --no-enable-telemetry --workspace /ComfyUI install --cpu
RUN comfy set-default --launch-extras="--cpu --use-pytorch-cross-attention --listen 0.0.0.0" /ComfyUI

CMD [ "comfy", "launch" ]
