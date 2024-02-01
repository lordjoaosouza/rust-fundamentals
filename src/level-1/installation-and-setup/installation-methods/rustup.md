### Installing with rustup (official Rust method)

- If you're using **Linux (includes WSL)** and **macOS** you can run (must have `curl` installed):
    ```bash
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
    ```
  And follow the instructions shown in the terminal.
- If you're using **Windows**, you can download the installer
  from [**Rust** website](https://www.rust-lang.org/tools/install?platform_override=win) or
  directly [here](https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe).

  After downloading the installer, run it and follow the instructions shown in the screen.
- Verify that **Rust** is properly installed:
    ```bash
    rustc --version
    ```
  You should see the version number of **Rust** printed to the console.
- Verify that **Cargo** is properly installed:
    ```bash
    cargo --version
    ```
  You should see the version number of **Cargo** printed to the console.
- Verify that **rustup** is properly installed:
    ```bash
    rustup --version
    ```
  You should see the version number of **rustup** printed to the console.

All these commands and links are available on the official [**Rust** website](https://www.rust-lang.org/tools/install).

So now you have **Rust** installed on your machine, let's move on to the next section to learn more about the [**Rust**
toolchain]().
