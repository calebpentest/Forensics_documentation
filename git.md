How to install git on fedora without any problem

1. **Install Git with sudo (correct way)**

```bash
sudo dnf install git
```

2. **If repos timeout or get stuck**

```bash
sudo dnf clean all
sudo dnf makecache --refresh
```

3. **Disable a slow or unnecessary repo (example: PyCharm Copr)**

```bash
sudo dnf config-manager --set-disabled phracek-PyCharm
```

4. **Re-enable a repo later if needed**

```bash
sudo dnf config-manager --set-enabled phracek-PyCharm
```

5. **Check Git version**

```bash
git --version
```

6. **Install GnuPG (correct package name)**

```bash
sudo dnf install gnupg
```

7. **Check if gpg is already installed**

```bash
gpg --version
```

8. **Skip unavailable packages during install**

```bash
sudo dnf install <package-name> --skip-unavailable
```

