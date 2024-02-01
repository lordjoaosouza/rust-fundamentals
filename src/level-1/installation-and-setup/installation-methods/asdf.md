### Installing with asdf (Linux and macOS only)

You will need to have `git` and `curl` installed on your machine to clone the **asdf** repository.

- Clone the **asdf** repository to your home directory:
    ```bash
    git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0
    ```
- Add the following line to your shell configuration file:
    - If you're using `bash` on **Linux (includes WSL)**:
      ```bash
      echo '. "$HOME/.asdf/asdf.sh"' >> ~/.bashrc
      ```
    - Or if you're using `bash` on **macOS**:
      ```bash
      echo '. "$HOME/.asdf/asdf.sh"' >> ~/.bash_profile
      ```
    - If you're using `zsh` on both:
      ```zsh
      echo '. "$HOME/.asdf/asdf.sh"' >> ~/.zshrc
      ```
    - You can install with other shell (e.g. `fish`) or with packages manager (e.g. `homebrew` and `pacman`), please
      refer to the [**asdf** documentation](https://asdf-vm.com/guide/getting-started.html).
- Restart your shell so that the configuration changes take effect.
- Verify that **asdf** is properly installed:
    ```bash
    asdf --version
    ```
  You should see the version number of **asdf** printed to the console.
- Update **asdf**:
    ```bash
    asdf update
    ```
- Install the [**asdf Rust** plugin](https://github.com/asdf-community/asdf-rust):
    ```bash
    asdf plugin add rust
    ```
- List all available versions of **Rust**:
    ```bash
    asdf list all rust
    ```
  You should see a list of all available versions of **Rust** printed to the console.
- Install the latest stable version of **Rust**:
  ```bash
  asdf install rust <last version on the list>
  ```
    - For example:
      ```bash
      asdf install rust 1.75.0
      ```
- Set the version you installed to your machine (you can choose if you want to set the version globally or locally):
    - Globally:
      ```bash
      asdf global rust <version>
      ```
        - For example:
          ```bash
          asdf global rust 1.75.0
          ```
    - Locally (inside some project's directory), that's useful if you want to use different versions of Rust in
      different projects:
      ```bash
      asdf local rust <version>
      ```
        - For example:
          ```bash
          asdf local rust 1.75.0
          ```
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
- As you installed with **asdf** you can see where these binaries are located:
    ```bash
    which rustc
    which cargo
    which rustup
    ```
  You should see the path where **asdf** installed these binaries printed to the console.

So now you have **Rust** installed on your machine, let's move on to the next section to learn more about the [**Rust**
toolchain]().
