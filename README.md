# docker-mailserver-armhf

Docker-mailserver for Raspberry Pi / armhf devices.

Just some little changes I put together which were provided by [@HolyGuacamole](https://github.com/HolyGuacamole) in this [issue](https://github.com/tomav/docker-mailserver/issues/348)

You will have to build this yourself.

```
docker build -t tvial/docker-mailserver:2.1 .
```

Afterwards you can follow the installation instructions written in the main repository. (You will have to change **tvial/docker-mailserver:latest** to **tvial/docker-mailserver:2.1** where it appears in commands in guide otherwise you will get errors)

Also since filebeat is being installed from a different location, you may need to edit the Dockerfile with the most recent link as I cannot keep up with the newest release.

```
https://beats-nightlies.s3.amazonaws.com/jenkins/filebeat/1291-ee07419cd283d5d5f5ebf6081adfd0915100ffcb/filebeat-linux-arm
```
To the newest one listed in https://beats-nightlies.s3.amazonaws.com/index.html?prefix=jenkins/filebeat/
```
https://beats-nightlies.s3.amazonaws.com/jenkins/filebeat/XXXX-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/filebeat-linux-arm
```

Every bit of feedback is appreciated as I know very little about docker. Maybe if someone can they could incorporate it with the main repository but for now this will have to do.

All credits still go to original creator [@tomav](https://github.com/tomav) and contributors
