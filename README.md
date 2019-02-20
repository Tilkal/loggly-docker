loggly-docker
=============

Docker container for loggly (via rsyslog). Check out Loggly's [Docker logging documentation](https://www.loggly.com/docs/docker-syslog/) to learn more.

Usage:

```
docker run -p 5014:514/udp -e LOGGLY_AUTH_TOKEN=[Loggly Customer Token] -e LOGGLY_TAG=[Tag Describing Source] tilkal/loggly
echo netcat:"Host test log" | nc -u -w 1 127.0.0.1 5014
```
