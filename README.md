
A collection of ansible roles for managing my personal archlinux install.

# dependencies:

- community.general collection: `ansible-galaxy collection install community.general`
- kewlfft.aur : `ansible-galaxy collection install kewlfft.aur`

# roles:

- base: Bootstraps the machine and adds a passwordless *ansible* user.
- pacman: Configures *pacman*, *aur* and adds *chaotic aur*, *flatpak* and other packaging utilities.
- dev: Installs and configures dev packages and utilities. 
- utils: Sets up *drivers*, *docker*, *virt-manager* and other utilities. 

