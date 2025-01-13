# mctk
Mecha Toolkit for Linux Wayland Clients

# Running Examples

This guide provides step-by-step instructions to set up and run the MCTK examples on a Debian/Ubuntu-based system.

## Prerequisites

1. **Wayland Compositor**:
   - Install `sway` (a Wayland compositor):
     ```bash
     sudo apt install sway
     ```

2. **Wayland Development Library**:
   - Install `libwayland-dev`:
     ```bash
     sudo apt install libwayland-dev
     ```

3. **Dependencies**:
   - Ensure `pkg-config` is installed:
     ```bash
     sudo apt install pkg-config
     ```

4. **Rust**:
   - Install the latest Rust toolchain if not already installed:
     ```bash
     curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
     ```

---

## Steps to Run the Examples

1. **Start the Wayland Compositor**:
   - Open a terminal and run:
     ```bash
     sway
     ```

2. **Set Up the Example Environment**:
   - Open another terminal (while `sway` is running) and set the `WAYLAND_DISPLAY` environment variable:
     ```bash
     export WAYLAND_DISPLAY=wayland-1
     ```

3. **Run an Example**:
   - Navigate to the example directory you want to run (e.g., `examples/hello-world`) and use `cargo run`:
     ```bash
     cd examples/hello-world
     cargo run
     ```

---
