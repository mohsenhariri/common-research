# Git and GitHub

## Setting Up SSH Key Pair

To set up an SSH key pair (public and private) for your machine and GitHub account, follow [this guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

## GitHub Configuration

### Mini-course

For a quick overview, check out this [mini-course](https://www.youtube.com/playlist?list=PLWKjhJtqVAbkFiqHnNaxpOPhh9tSWMXIF).

### Reference

Refer to the [Git documentation](https://git-scm.com/book/en/v2) for more detailed information.

## Repository Setup

1. **Watch the Repository**: Add the research repo to your watch list by clicking the watch button in the upper right corner of the repo page.

    ![watch-list](image.png)

2. **Fork the Repository**: Fork the repo by clicking the fork button in the upper right corner of the repo page.

    ![fork](image-1.png)

3. **Clone the Repository**: Clone the repo to your local machine or HPC.

    Example:
    ```bash
    git clone git@github.com:mohsenhariri/common-research.git
    ```

    **Notes**:
    * Ensure your SSH key is set up in your GitHub account to clone the repo.
    * The preferred way to clone the repo is using SSH, not HTTPS.

4. **Create a New Branch**: Create a new branch for your work.

    ```bash
    git checkout -b new-branch-name
    ```

5. **Make Changes and Push**: Make your changes and push them to your forked repo.

    ```bash
    git add .
    git commit -m "your message"
    git push origin new-branch-name
    ```

6. **Create a Pull Request**: Create a pull request from your forked repo to the original repo.
