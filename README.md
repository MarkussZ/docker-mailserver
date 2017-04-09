# docker-mailserver-armhf

Docker-mailserver for Raspberry Pi / armv7 devices.

Just some little changes I put together which were provided by [@HolyGuacamole](https://github.com/HolyGuacamole) in this [issue](https://github.com/tomav/docker-mailserver/issues/348)

You will have to build this yourself.

```
docker build -t tvial/docker-mailserver:2.1 .
```

Afterwards you can follow the installation instructions written in the main repository. (You will have to change **tvial/docker-mailserver:latest** to **tvial/docker-mailserver:2.1** where it appears in commands in guide otherwise you will get errors)


All credits still go to original creator [@tomav](https://github.com/tomav) and contributors
