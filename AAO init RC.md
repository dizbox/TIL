AAO init.rc 내용 수정
```
service batteryd /vendor/bin/batteryd
    class last_start
    user root
    group system system wakelock
    disabled
    oneshot
    seclabel u:r:batteryd:s0

on property:sys.boot_completed=1
    start batteryd

#run batteryd in off-charge mode
on charger
    start batteryd
```