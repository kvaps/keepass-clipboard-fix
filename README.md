Clipboard fix for Keepass2
==========================

Dirty solution to fix this bugs:

Sloves this bugs:
- https://sourceforge.net/p/keepass/bugs/1530/
- https://github.com/FreeRDP/Remmina/issues/900

Installation
------------

Just replace the content of keepass2 starting script:

```bash
file=`whereis -b keepass | awk '{print $2}'`
curl https://raw.githubusercontent.com/kvaps/keepass-clipboard-fix/master/keepass > $file
```
