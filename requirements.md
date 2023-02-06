# Requirements

## Tools

### Visual Studio Code

[![VSCode][vscode]][vscode-url]

- Code editor
- I am used to and it has helpful extensions to ease the work flow.

### Microsoft Edge

[![Edge][edge]][edge-url]

- Web Browser
- It comes built-in Windows 10 & 11.

### Git

[![Git][git]][git-url]

- Open source distributed version control system.
- I use it to track and monitor my projects and upload it to github.

### Node.js

[![Node][node.js]][node-url]

- JavaScript Runtime
- Use Node.js to execute JavaScript programs


### SSH key

To avoid entering a username and password everytime you interact with GitHub you can use what is called a key pair. Follow these steps to generate and use your own SSH key:

1. Open Git Bash
2. Create your key pair
   1. Run `ssh-keygen -t ed25519 -C "youremail@yourdomain.com"`. The `-t` argument specifies the key type and `-C` is a comment
   2. Give it a file name
   3. Leave the passphrase blank
   4. Leave the passphrase blank again
   5. Done! It will have created two files one ending with .pub which is the public key and the other is the private key
3. Start the ssh agent with `eval "$(ssh-agent -s)"`
4. Run `ssh-add <file name or path to file>`. Make sure to use the private key, do **NOT** use the file that ends with .pub
5. Adding public key to github
   1. Open GitHub in your browser
   2. Top right, select your profile photo and click Settings
   3. In the menu on the left, look for Access and select "SSH and GPG keys"
   4. Click New SSH Key
   5. Paste the contents of the public key (`<file name>.pub`) in to the key area
   6. Click Add SSH Key
   7. Done!

[vscode]: https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white
[vscode-url]: https://code.visualstudio.com/
[git]: https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white
[git-url]: https://git-scm.com/
[edge]: https://img.shields.io/badge/Microsoft_Edge-0078D7?style=for-the-badge&logo=Microsoft-edge&logoColor=white
[edge-url]: https://www.microsoft.com/edge
[node.js]: https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white
[node-url]: https://nodejs.org/
