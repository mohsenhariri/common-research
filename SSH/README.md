# SSH

The ssh config file is used to store configurations for SSH connections. This file is located at `~/.ssh/config`. You can copy the contents of the `https://github.com/mohsenhariri/common-research/blob/main/SSH/config` to your own `~/.ssh/config` file.

## GitHub Configuration

To set up a SSH key pair for your machine and GitHub account follow [this link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).


## Set up SSH Key Pair for HPC
1. Generate a new SSH key pair:
    ```bash
    ssh-keygen -o -a 75 -t ed25519 -f ~/.ssh/keyname -C "email"
    ```
2. Ensure the SSH agent is running:
    ```bash
    eval "$(ssh-agent -s)"
    ```
3. Add the new key to the SSH agent:
    ```bash
    ssh-add ~/.ssh/keyname
    ```
4. Copy the SSH public key to the HPC server:
    ```bash
    ssh-copy-id -i ~/.ssh/keyname.pub username@remote_ip
    ```
    Or manually copy the public key:
    ```bash
    cat ~/.ssh/keyname.pub
    ```
    Then add the content to the server's `~/.ssh/authorized_keys` file.

5. (Apple Users Only) Store the passphrase in the Keychain:
    - For macOS 12.0 Monterey and later:
        ```bash
        ssh-add --apple-use-keychain ~/.ssh/keyname
        ```
    - For macOS versions older than 12.0 Monterey:
        ```bash
        ssh-add -K ~/.ssh/keyname
        ```
