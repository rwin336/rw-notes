# Problem Description

Ubuntu Xenial (16.04) VM running on VMWare was seeing high CPU usage on the khugepaged process.

Entire VM becomes useless.

# Platform
Ubuntu Xenial 16.04

# Reference
* http://unix.stackexchange.com/questions/161858/arch-linux-becomes-unresponsive-from-khugepaged
* https://bugzilla.redhat.com/show_bug.cgi?id=879801
* https://www.kernel.org/doc/Documentation/vm/transhuge.txt

# Workaround Procedure

1. echo never > /sys/kernel/mm/transparent_hugepage/defrag
2. echo 0 > /sys/kernel/mm/transparent_hugepage/khugepaged/defrag
