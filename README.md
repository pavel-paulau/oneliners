Capture full gdb output:

    gdb --ex 't a a bt full' /opt/couchbase/bin/memcached /tmp/core.memcached.27157  < /dev/null  > gdb.log

Disable vCPU:

    echo 0 > /sys/devices/system/cpu/cpuX/online

Drop buffers and OS cache:

    sync && echo 3 > /proc/sys/vm/drop_caches
