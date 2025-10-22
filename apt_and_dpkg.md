# Package Management — apt & dpkg (Debian/Ubuntu/Kali)

## apt (recommended high-level)
- `sudo apt update` — refresh package lists
- `sudo apt upgrade` — upgrade installed packages
- `sudo apt install package-name` — install package
- `sudo apt remove package-name` — remove package
- `sudo apt purge package-name` — remove including config files
- `apt-cache search term` — search packages

## dpkg (low-level)
- `dpkg -i package.deb` — install .deb file
- `dpkg -l | grep package` — list installed packages
- `dpkg -r package` — remove package (no deps handling)

## Tips
- Use `apt` for normal installs; `dpkg` for local .deb files.
- If dependency errors: `sudo apt -f install` can fix broken deps.
