# Dotfiles
this repository is a personal dotfiles management remote git repository powered by [GNU stow](https://github.com/aspiers/stow)

---

### This repository includes dotfiles / config files :
- <a href="https://github.com/neovim/neovim" ><img src="https://upload.wikimedia.org/wikipedia/commons/4/4f/Neovim-logo.svg" alt="Neovim" height="30" ></a>
- <a href="https://github.com/kovidgoyal/kitty"><img src = "https://upload.wikimedia.org/wikipedia/commons/2/2f/Kitty%28Terminal-emulator%29.png" alt = "Kitty" height="30"></a>
- <a href = "https://www.zsh.org/"><img src="[https://upload.wikimedia.org/wikipedia/commons/1/1f/Z_Shell_Logo_Color_Horizontal.svg](https://www.google.com/url?sa=i&url=https%3A%2F%2Fgithub.com%2FZsh-art%2Flogo&psig=AOvVaw3rnwHRcCEinHmPm15g3Qur&ust=1735152690911000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCPDlzs-JwYoDFQAAAAAdAAAAABAE)" alt="Zsh" height="30"></a>
- [FastFetch](https://github.com/fastfetch-cli/fastfetch).
- [Rofi](https://github.com/davatorium/rofi).
- More to come

---

## Installation :

### dependencies to install **Stow**:

- Using [Brew](https://brew.sh/) for windows and mac:
```brew install stow```

- Using Pacman for Arch Users :
```sudo pacman -S stow```

- Using apt on Ubuntu :
```sudo apt install stow```


To install the following dotfiles, clone the into your home directory
```git clone --depth 1 https://github.com/TheFatCatDev/dotfiles ${XDG_DATA_HOME}```

---

## Setting up symlinks :
After completing the above process, just *cd* into the **dotfiles** repository:
```cd ~/dotfiles```

and start stow:
```stow .```

---

### How [stow](https://github.com/aspiers/stow) Works:
Stow is a symlink farm manager program which takes distinct sets of software and/or data located in separate directories on the filesystem, and makes them all appear to be installed in a single directory tree.

Originally Stow was born to address the need to administer, upgrade, install, and remove files in independent software packages without confusing them with other files sharing the same file system space. For instance, many years ago it used to be common to compile programs such as Perl and Emacs from source and install them in `/usr/local`. By using Stow, `/usr/local/bin` could contain symlinks to files within `/usr/local/stow/emacs/bin`, `/usr/local/stow/perl/bin` etc., and likewise recursively for any other subdirectories such as `.../share`, `.../man`, and so on.
