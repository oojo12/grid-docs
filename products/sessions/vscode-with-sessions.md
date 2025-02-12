---
description: >-
  Visual studio code is a source-code editor made by Microsoft for Windows,
  Linux and macOS. Features include support for debugging, syntax highlighting
  etc.
---

# VSCode with Sessions

## Step 1: Create and add the SSH Key

Create an ssh key from the computer you'd like to connect from (skip this step if you already have a key)

```yaml
# make the ssh key (if you don't have one)
ssh-keygen -t ed25519 -C "your_email@example.com"

# add the keys to grid
grid ssh-keys add lit_key ~/.ssh/id_ed25519.pub
```

## Step 2: launch the session

```bash
grid session create --name fun-bear-259
```

## Step 3: login to the interactive session

```bash
grid session ssh fun-bear-259
```

## Step 4: Install remote ssh extension

![](<../../.gitbook/assets/image (93) (2) (2) (2) (2) (2) (2) (2) (2) (8) (3) (7).png>)

## Step 5: Click the remote tab and find your session

![](<../../.gitbook/assets/vscode (1).gif>)

## Step 6: Ready

Clicking on it will open VSCode in the remote IxNode. You can use VSCode with any of its features.

![](../../.gitbook/assets/vscode.gif)

{% hint style="info" %}
You can clone any Github repositories into a Session using the [HTTPS cloning method](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository#cloning-a-repository-using-the-command-line) (SSH will not work).
{% endhint %}
