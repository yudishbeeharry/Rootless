# Rootless
[In Progress] A collection of research, tools, and techniques for modifying Android systems without root access.

Purpose:
To access the functionality of Xposed modules and perform dynamic instrumentation with Frida without having to go through the hassle of rooting, hiding root status, or bypassing integrity checks like Play Integrity.

Limitations:
Since this method doesn't involve rooting the device, Magisk and Zygisk modules are not compatible. This also means any modifications requiring system access (UID 0) are not feasible.
