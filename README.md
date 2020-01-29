# IRSSI

How to start irssi using docker.

```bash
    docker run -it --name mIRC -e TERM -u $(id -u):$(id -g) \
    --log-driver=none \
    -v $HOME/.irssi:/home/user/.irssi:ro \
    -v /etc/localtime:/etc/localtime:ro \
    irssi:alpine
```
