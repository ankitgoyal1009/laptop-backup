Things I did for first time setup of my new laptop

- install browser of your choice(firefox and brave in my case)
- login to the browser account so all your passwords and bookmarks will sync
- install any communication tool like slack
- take backup of your old laptop, read the main file
- install iTerm2
- install ohMyZsh "https://ohmyz.sh/#install"
- paste all your zsh_history, zshrc files etc.
- install brew from https://brew.sh/
- if you find "xcode-select: note: No developer tools were found, requesting install." error whiel cloning any repo or installing ohMyZsh, install xcode using `sudo xcode-select --install`
- If you copy zshrc from older laptop make sure to recheck all the paths correctly like I had `export ZSH="/Users/OLD_USER/.oh-my-zsh"` and I was getting ` cannot mkdir /Users/OLD_USER/.oh-my-zsh: Permission denied` error while installing ohMyZsh
- If you have local changes in ohMyZsh then you need to follow https://stackoverflow.com/questions/70368969/error-trying-to-update-oh-my-zsh-i-have-already-removed-yarn-and-continue

Installing existing ssh
- check if you have open SSH or not -> ssh -V(if this command works then you have open SSH)
- To create an SSH key pair:
-   cd ~
-   ssh-keygen -t ed25519 -b 4096 -C "{username@emaildomain.com}" -f {ssh-key-name}
- To add existing key into ssh
-   ssh-add ~/{ssh-key-name}



