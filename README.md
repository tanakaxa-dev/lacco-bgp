# BGP Status

Sat Jun 15 18:59:11 JST 2019
## tanakaxa-ix AS:64513

```

PLAY [ix] **********************************************************************

TASK [collect] *****************************************************************
ok: [tanakaxa-ix]

TASK [show clock] **************************************************************
ok: [tanakaxa-ix] => {
    "msg": [
        "Saturday, 15 June 2019 18:59:10 +09 00"
    ]
}

TASK [show ip bgp] *************************************************************
ok: [tanakaxa-ix] => {
    "msg": [
        "BGP table version is 112, local router ID is 172.18.19.1",
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
ok: [tanakaxa-cis]

TASK [show clock] **************************************************************
ok: [tanakaxa-cis] => {
    "msg": [
        "18:59:04.727 JST Sat Jun 15 2019"
    ]
}

TASK [show ip bgp] *************************************************************
ok: [tanakaxa-cis] => {
    "msg": [
        "BGP table version is 130, local router ID is 172.18.19.5",
        "Status codes: s suppressed, d damped, h history, * valid, > best, i - internal, ",
        "              r RIB-failure, S Stale, m multipath, b backup-path, f RT-Filter, ",
        "              x best-external, a additional-path, c RIB-compressed, ",
        "              t secondary path, ",
        "Origin codes: i - IGP, e - EGP, ? - incomplete",
        "RPKI validation codes: V valid, I invalid, N Not found",
        "",
        "     Network          Next Hop            Metric LocPrf Weight Path",
        " *>   10.128.0.0/29    172.18.20.1                            0 64515 64512 i",
        " *>   10.128.1.0/24    172.18.20.1                            0 64515 64512 64520 i",
        " *>   172.18.19.4/30   0.0.0.0                  0         32768 i",
        " *>   172.18.19.8/30   172.18.19.45            11         32768 ?",
        " *>   172.18.19.32/28  0.0.0.0                  0         32768 ?",
        " *>   172.18.20.0/30   0.0.0.0                  0         32768 i",
        " *>   172.18.20.4/30   172.18.20.1                            0 64515 64512 i",
        " *>   172.18.20.16/28  172.18.20.1              0             0 64515 i",
        " *>   172.18.21.0/30   172.18.20.1                            0 64515 64516 i",
        " *>   172.18.21.4/30   172.18.20.1                            0 64515 64516 i",
        " *>   192.168.211.0/30 0.0.0.0                  0         32768 i"
    ]
}

PLAY RECAP *********************************************************************
tanakaxa-cis               : ok=3    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

```

