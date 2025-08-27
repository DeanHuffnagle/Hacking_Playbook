### Connect Using RDP
```
xfreerdp3 /u:$TARGET_USER /p:$TARGET_PASS /v:$TARGET_IP
```

### Connect With File Transfer
```shell-session
xfreerdp3 /v:$TARGET_IP /d:Fileshare /u:$TARGET_USER /p:$TARGET_PASS /drive:linux,/home/dean/Transfer
```
