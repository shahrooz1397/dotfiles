# Hyprdots

**hyprdots** is a collection of dotfiles and configuration files aimed at setting up a personalized and efficient Linux environment. This repository includes configurations for various tools and applications, enhancing productivity and aesthetics.

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Configuration Details](#configuration-details)
5. [Contributions](#contributions)
6. [License](#license)
7. [Contact](#contact)

## Features

- **Application Configurations**: Custom settings for applications.
- **Custom Icons**: Personalized icon sets for a unique desktop experience.
- **Wallpapers**: A curated collection of wallpapers.
- **tmux Configuration**: Enhanced tmux settings for better terminal multiplexing.
- **zsh Configuration**: Optimized zsh settings for an improved shell experience.
- **Backup of Old Dotfiles**: Archive of previous configurations.

## Installation

To set up your environment using `hyprdots`, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/ahmad9059/hyprdots.git
    cd hyprdots
    ```

2. **Backup Existing Dotfiles**:
    Before copying new configurations, it's wise to back up your current dotfiles:
    ```bash
    mkdir -p ~/dotfiles_backup
    cp ~/.config ~/dotfiles_backup -r
    cp ~/.tmux.conf ~/dotfiles_backup
    cp ~/.zshrc ~/dotfiles_backup
    ```

3. **Copy New Configurations**:
    ```bash
    cp -r .config ~/
    cp .tmux.conf ~/
    cp .zshrc ~/
    ```

4. **Apply Desktop Theme**:
    Extract and apply the Vimix theme:
    ```bash
    tar -xf Vimix-1080p.tar.xz -C ~/.themes/
    ```

## Usage

After installation, you can start using the configured applications. Modify the configurations as per your preferences:

- **tmux**: Start tmux with custom settings using:
    ```bash
    tmux
    ```

- **zsh**: Ensure zsh is your default shell, then reload configurations:
    ```bash
    chsh -s $(which zsh)
    source ~/.zshrc
    ```

- **Desktop Environment**: Apply the new theme and icons through your desktop environment settings.

## Configuration Details

### .config

- Contains configurations for various applications like:
  - `nvim` (Neovim)
  - `i3` (i3 Window Manager)
  - `polybar` (Status Bar)

### .tmux.conf

- Custom tmux settings for improved usability and aesthetics.

### .zshrc

- Aliases, prompt customization, and plugin settings for zsh.

### Icons and Wallpapers

- Custom icons located in `.icons`.
- Wallpapers are in the `wallpapers` directory.

### old_dots

- Backup of previous dotfiles for reference and recovery.

## Contributions

Contributions are welcome! If you have improvements or additional configurations, feel free to fork this repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions, suggestions, or issues, please open an issue in this repository or contact the repository owner directly.

---

Enjoy your personalized Linux setup!
