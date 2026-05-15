# Homebrew OpenSSL 1.1 (Private Tap)

Private Homebrew tap that provides the legacy **OpenSSL 1.1** formula.

> OpenSSL 1.1 is deprecated and no longer maintained in Homebrew
> core.\
> This tap exists strictly for legacy compatibility purposes.

------------------------------------------------------------------------

## Overview

This repository hosts a private Homebrew tap for installing **OpenSSL
1.1**, which has been removed from the official Homebrew core
repository.

Use this only if you maintain legacy systems or CI pipelines that still
depend on OpenSSL 1.1.

If you are starting a new project, use OpenSSL 3.x instead.

------------------------------------------------------------------------

## Installation

### Tap the repository

``` bash
brew tap Teviwe/openssl https://github.com/Teviwe/homebrew-openssl.git
```

### Install OpenSSL 1.1

``` bash
brew install openssl@1.1
```

------------------------------------------------------------------------

## Verify Installation

``` bash
openssl version
```

Expected output:

    OpenSSL 1.1.x

------------------------------------------------------------------------

## Optional Linking (Use Carefully)

If your build requires explicit linking:

``` bash
brew link --force --overwrite openssl@1.1
```

This may override newer OpenSSL versions.

------------------------------------------------------------------------

## Important Notes

-   OpenSSL 1.1 is End Of Life (EOL)
-   No security updates are guaranteed
-   Intended strictly for legacy compatibility
-   Migration to OpenSSL 3.x is strongly recommended

------------------------------------------------------------------------

## Maintenance

This tap is privately maintained and may not receive regular updates.
Use at your own risk.
