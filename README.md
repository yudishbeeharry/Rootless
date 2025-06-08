# Rootless
[In Progress] A collection of research, tools, and techniques for modifying Android systems without root access.

Purpose:
To access the functionality of Xposed modules and perform dynamic instrumentation with Frida without having to go through the hassle of rooting, hiding root status, or bypassing integrity checks like Play Integrity.

Limitations:
Since this method doesn't involve rooting the device, Magisk and Zygisk modules are not compatible. This also means any modifications requiring system access (UID 0) are not feasible.

Note: This approach is currently theoretical and has not been fully tested.

For dynamic instrumentation in a rootless environment:
Step 1: Install Shizuku from https://github.com/RikkaApps/Shizuku and establish a USB debugging session with the Shizuku app to grant necessary permissions.
Step 2: Install LSPatch, a non-root Xposed framework. Since the original project is no longer maintained, the fork by JingMatrix can be used instead: https://github.com/JingMatrix/LSPatch.
Step 3: Install Mujde from https://github.com/mon231/com.rel.mujde and load your Frida JavaScript instrumentation scripts into the app for runtime patching and analysis.
