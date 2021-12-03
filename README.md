# CMPE-283-ass4

# Nested Paging vs. Shadow Paging

1.  test VM

## CPUID leaf function 0x4FFFFFFE-  record total exit count information 

## Shutdown your test (inner) VM.

Remove the ‘kvm-intel’ module from your running kernel:
◦rmmod kvm-intel


Reload the kvm-intel module with the parameter ept=0 

isable nested paging and force 
KVM to use shadow paging instead)

Booting the same test VM again,


sample of your print of exit count output from dmesg from “with ept” and “without ept”


learn from the count of exits? Was the count what you expected? If not, why not?



What changed between the two runs (ept vs no-ept)?
