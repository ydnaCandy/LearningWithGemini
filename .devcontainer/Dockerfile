FROM mcr.microsoft.com/devcontainers/javascript-node:22

# Python インストール
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    python3-venv \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# よく使う Python パッケージ
RUN pip3 install --break-system-packages \
    requests \
    numpy \
    pandas \
    matplotlib \
    ipython

# Gemini CLI のインストール
RUN npm install -g @google/gemini-cli
