# Terminus Flatpak

This is a flatpak build configuration based on several electron flatpak apps.

There are a few issues that could not be solved:
* Serial connections don't work because they are blocked by flatpak sandboxing.
* Even though Terminus can access host executables with --filesystem=host argument, it has limited usage as a sandboxed app because it can't access libraries installed on host.
