### TTT
- Docker on Windows Host/Environment
- Visual Studio Code Dev Containers extension
- https://code.visualstudio.com/docs/devcontainers/containers
- https://www.docker.com/products/docker-desktop/
- https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers

Extensions
- https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens
- https://marketplace.visualstudio.com/items?itemName=KevinRose.vsc-python-indent
- https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff
- https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree

https://hub.docker.com/_/python

Boilerplate Dockerfile
```
FROM python:3

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "./your-daemon-or-script.py" ]
```
