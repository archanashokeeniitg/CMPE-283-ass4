# CMPE-283-ass4

Archana Shokeen (015237378)


# Nested Paging vs. Shadow Paging


# Steps Followed from Assignment 4 Documentation

For environment - Use kernel environment in Assignment 3

Boot test VM using assignment 3.


CPUID leaf function 0x4FFFFFFE-  record total exit count information 

Record total exit count for each type of exit handled by KVM

Shut down inner VM

Remove 'kvm-intel' module

`rmmod kvm-intel`

Reload kvm-intel module using the parameter ept = 0 

Boot same test VM. Record the number of exits and exit types

# Questions

## Sample Outputs :

Check .txt files above

## What did you learn from the count of exits? Was the count what you expected? If not, why not?

With ept, the exit count is less in comparison to the exit count without ept. This is expected because an exit occurs only when an EPT violation is raised in nested paging. In shadow paging, more exits occur such as page faults, CR0 execution, etc.

## What changed between the two runs(ept vs no-ept)?

In non-ept mode, the page table does not belong to the guest VM. In ept mode, two page tables are utilized to get the host physical address and the page table elongs to the guest VM.
