# Formats

When we create a regular Linux program, we generate an ELF file, which is read by the OS.

Without an OS, we can use the following formats:

-   boot sector, of which MBR is an important type.

-   El Torito for CDs: <https://en.wikipedia.org/wiki/El_Torito_%28CD-ROM_standard%29>

-   multiboot

-   hybrid boot sector / El Torito. It is possible to generate images that can be burnt either to USBs or optic disks.

    The Linux kernel 4.2 for example does that by default upon `make isoimage`.

-   PXE: <https://en.wikipedia.org/wiki/Preboot_Execution_Environment> and its implementation <https://en.wikipedia.org/wiki/IPXE>

    Boot from the network. TODO how does it work exactly? I suppose there is a server, and then the BIOS can download the boot sector from it.
