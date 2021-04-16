FROM python:3.8-slim

ENV PATH=/root/.local/bin:$PATH

# Install the required stack
RUN pip install --user jupyterlab \
    pandas \
    numpy \
    matplotlib \
    torch==1.8.1 \
    torchvision \
    torchaudio

EXPOSE 8888

CMD [ "/bin/bash", "-c", "jupyter-lab --notebook-dir=/ --ip 0.0.0.0 --no-browser --allow-root"]