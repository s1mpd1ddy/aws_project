# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.163.0/containers/python-3/.devcontainer/base.Dockerfile

# [Choice] Python version: 3, 3.9, 3.8, 3.7, 3.6
ARG VARIANT="3.9"
FROM mcr.microsoft.com/vscode/devcontainers/python:0-${VARIANT} as deploy

WORKDIR /workspace

COPY Pipfile Pipfile.lock /workspace/
RUN pipenv sync --dev
