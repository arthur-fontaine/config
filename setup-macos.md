## Initial Settings

1. Switch to qwerty
2. Disable natural scrolling
3. Update the Mac

## Applications

1. Download [Raycast](https://www.raycast.com/)
2. Download [Arc](https://arc.net/download)
3. Download 1Password
    1. [The macOS app](https://1password.com/fr/downloads/mac)
    2. [The extension](https://chromewebstore.google.com/detail/1password-%E2%80%93-gestionnaire/aeblfdkhhhdcdjpifhhbdiojplfjncoa)
4. Download [Ghostty](https://ghostty.org/download)
5. In the CLI, tap `git` to install Git (macOS will automatically open a popup to install the developer tools)
6. Download [VSCode](https://code.visualstudio.com/download)

## Others

1. Download [Input Mono font](https://input.djr.com/download/)
2. Download [Jetbrains Mono font](https://www.jetbrains.com/lp/mono/)

## Configs

1. Enable `sudo` with TouchID
    1. ```bash
       sudo cp /etc/pam.d/sudo_local.template /etc/pam.d/sudo_local
       ```
    2. ```bash
       sudo pico /etc/pam.d/sudo_local
       ```
    3. Uncomment the line
