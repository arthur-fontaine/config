## System Preferences

1. Switch to qwerty
2. Disable natural scrolling and 24-hour
3. Update the Mac

## Applications

1. Download [Brew](https://brew.sh/)
2. Download [Raycast](https://www.raycast.com/)
3. Download [Arc](https://arc.net/download)
4. Download 1Password
    1. [The macOS app](https://1password.com/fr/downloads/mac)
    2. [The extension](https://chromewebstore.google.com/detail/1password-%E2%80%93-gestionnaire/aeblfdkhhhdcdjpifhhbdiojplfjncoa)
    3. [The CLI](https://developer.1password.com/docs/cli/get-started/)
5. Download [Ghostty](https://ghostty.org/download)
6. Download [VSCode](https://code.visualstudio.com/download)
7. Download [Keka](https://d.keka.io/) and the [Keka helper](https://d.keka.io/helper) (once done, open Keka general settings and set Keka as the default extraction application)

## CLIs

1. In the CLI, tap `git` to install Git (macOS will automatically open a popup to install the developer tools)
2. Run `brew install antidote fzf gh httpie fx pyenv git-delta`
3. Install [Volta](https://volta.sh/)
    ```bash
    curl https://get.volta.sh | bash
    ```
4. Install [Golang](https://go.dev/dl/)
5. Install [`cps`](https://github.com/yongkangchen/cps)
    ```bash
    curl https://raw.githubusercontent.com/yongkangchen/cps/main/cps -o cps && chmod +x cps && sudo mv cps /usr/local/bin
    ```
6. Install [uv](https://docs.astral.sh/uv/)
   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

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
2. Download the [.config](https://download-directory.github.io/?url=https%3a%2f%2fgithub.com%2farthur-fontaine%2fconfig%2ftree%2fmain%2f.config) directory and put it at `~/.config`
3. Configure Git to use Delta
   ```bash
   cat <<EOF >> ~/.gitconfig
   [core]
       pager = delta
   
   [interactive]
       diffFilter = delta --color-only
   
   [delta]
       navigate = true  # use n and N to move between diff sections
       dark = true      # or light = true, or omit for auto-detection
   
   [merge]
       conflictstyle = zdiff3

   [push]
        autoSetupRemote = true
   EOF
   ```
4. If you have servers that you connect to with SSH, go in your `/etc/hosts` and name them. You will then be able to connect to your server with `ssh user@servername`.

## Shortcuts

### Raycast

#### Search Emoji & Symbols

| Shortcut | Description | How to? |
| --- | --- | --- |
| `Ctrl+Space` | Search Emoji & Symbols | Open Raycast parameters, go to Extensions and search `emoji`. Then, set the shortcut to `Ctrl+Space`. If you can't, you need to disable a specific parameter in System Preferences (check https://github.com/spring-projects/sts4/issues/517#issuecomment-668635598) |
