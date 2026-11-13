# Z1 PCB – releases

Windows 10/11 installers of [Z1 PCB](https://github.com/JoeApo108/z1pcb) (G-code for the Makera Z1 from Gerber and
Excellon files). The user interface is in Slovak.

**Download:** [latest release](https://github.com/JoeApo108/z1pcb-releases/releases/latest) → `Z1PCB-x.y.z-setup.exe`.
On first start Windows shows "Windows protected your PC": click **More info → Run anyway**.

Each release has a `.sig` file next to the installer: an ed25519 signature over the installer's name, version, size
and SHA-256. The app installs an update only if the signature is valid. Public key:

    c73020442ce697f8af26bba7d18d0b7d0ac48cba3a7829fcf31889b64c8f593c

Manual check of a downloaded file: its SHA-256 (`Get-FileHash Z1PCB-x.y.z-setup.exe`) must equal `sha256` in the `.sig`.
