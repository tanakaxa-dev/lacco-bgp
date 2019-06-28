# BGP Status

Fri Jun 28 18:39:29 JST 2019
## tanakaxa-ix AS:64513

```

PLAY [ix] **********************************************************************

TASK [collect] *****************************************************************
ok: [tanakaxa-ix]

TASK [show clock] **************************************************************
ok: [tanakaxa-ix] => {
    "msg": [
        "Friday, 28 June 2019 18:39:26 +09 00"
    ]
}

TASK [show ip bgp] *************************************************************
ok: [tanakaxa-ix] => {
    "msg": [
        "BGP table version is 2, local router ID is 172.18.19.1",
        "Local AS number 64513",
        "Status codes: s - suppressed, * - valid, h - history",
        "              > - best, i - internal",
        "Origin codes: i - IGP, e - EGP, ? - incomplete",
        "",
        "   Network            Next Hop            Metric     LocPrf  Path",
        "   172.18.18.0/30     0.0.0.0                  0             i",
        "   172.18.18.4/30     0.0.0.0                  0             i",
        "*> 172.18.19.0/30     0.0.0.0                  0             i",
        "*> 172.18.19.16/28    0.0.0.0                  0             i",
        "",
        "Total number of prefixes 4"
    ]
}

PLAY RECAP *********************************************************************
tanakaxa-ix                : ok=3    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

```

## tanakaxa-cis AS:64514

```

PLAY [ios] *********************************************************************

TASK [collect] *****************************************************************
fatal: [tanakaxa-cis]: FAILED! => {"msg": "[Errno None] Unable to connect to port 22 on 172.18.19.46"}

PLAY RECAP *********************************************************************
tanakaxa-cis               : ok=0    changed=0    unreachable=0    failed=1    skipped=0    rescued=0    ignored=0   

```

