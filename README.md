## How to Install
* Place `ac-mode` in `/bin`

* Make the program executable

```
sudo chmod 755 /bin/ac-mode
```

* Add this section to `rc.local`

```
# AC MODE
if [ -x /bin/ac-mode ]; then
    ( sleep 20; setsid nohup /bin/ac-mode >> /var/log/ac-mode.log 2>&1 ) &
fi
```

* Restart system
