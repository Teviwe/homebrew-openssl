# Homebrew OpenSSL 1.1 (Private Tap)

Private Homebrew tap that provides the legacy **OpenSSL 1.1** formula.

> ⚠️ OpenSSL 1.1 is deprecated and no longer maintained in Homebrew
> core.\
> This tap exists strictly for legacy compatibility purposes.

------------------------------------------------------------------------

## 📌 Overview

This repository hosts a private Homebrew tap for installing **OpenSSL
1.1**, which has been removed from the official Homebrew core
repository.

Use this only if you maintain legacy systems or CI pipelines that still
depend on OpenSSL 1.1.

If you are starting a new project, use OpenSSL 3.x instead.

------------------------------------------------------------------------

## 🔐 Prerequisites

Since this is a **private repository**, you must have SSH access
configured.

### 1. Generate SSH key (if you don't have one)

``` bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

### 2. Add SSH key to GitHub

-   Go to **GitHub → Settings → SSH and GPG keys**
-   Click **New SSH key**
-   Paste your public key

### 3. Verify access

``` bash
ssh -T git@github.com
```

------------------------------------------------------------------------

## 🚀 Installation

### 1️⃣ Tap the repository

``` bash
brew tap Teviwe/openssl git@github.com:Teviwe/homebrew-openssl.git
```

### 2️⃣ Install OpenSSL 1.1

``` bash
brew install openssl@1.1
```

------------------------------------------------------------------------

## 🔎 Verify Installation

``` bash
openssl version
```

Expected output:

    OpenSSL 1.1.x

------------------------------------------------------------------------

## 🧩 Optional Linking (Use Carefully)

If your build requires explicit linking:

``` bash
brew link --force --overwrite openssl@1.1
```

⚠️ This may override newer OpenSSL versions.

------------------------------------------------------------------------

## 🛑 Important Notes

-   OpenSSL 1.1 is End Of Life (EOL)
-   No security updates are guaranteed
-   Intended strictly for legacy compatibility
-   Migration to OpenSSL 3.x is strongly recommended

------------------------------------------------------------------------

## 🧯 Troubleshooting

If Homebrew cannot access the repository:

-   Verify SSH authentication:

    ``` bash
    ssh -T git@github.com
    ```

-   Ensure your GitHub account has access to the private repository

------------------------------------------------------------------------

## 📦 Maintenance

This tap is privately maintained and may not receive regular updates.
Use at your own risk.
