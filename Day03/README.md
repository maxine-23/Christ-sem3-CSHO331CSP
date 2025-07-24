# Linux Commands, GitHub Usage & Windows Security Notes

## 1. Basic Linux Commands with Examples

Linux commands are used to interact with the operating system through the terminal. Here are some commonly used commands:

| Command | Description                           | Example                          |
| ------- | ------------------------------------- | -------------------------------- |
| `ls`    | Lists files and directories           | `ls /home/user`                  |
| `cd`    | Changes directory                     | `cd Documents`                   |
| `pwd`   | Prints current directory              | `pwd`                            |
| `mkdir` | Creates a new directory               | `mkdir my_folder`                |
| `rm`    | Removes files or directories          | `rm file.txt` or `rm -r folder/` |
| `cp`    | Copies files/directories              | `cp source.txt destination.txt`  |
| `mv`    | Moves or renames files                | `mv oldname.txt newname.txt`     |
| `touch` | Creates a new empty file              | `touch file.txt`                 |
| `cat`   | Displays file contents                | `cat file.txt`                   |
| `clear` | Clears the terminal screen            | `clear`                          |
| `sudo`  | Executes command with root privileges | `sudo apt update`                |

---

## 2. Cloning Projects using GitHub

GitHub is a platform used for version control and collaboration. It allows users to host and review code, manage projects, and collaborate on software development.

### Steps to Clone a Project:

1. Go to the GitHub repository page.
2. Click the green **"Code"** button.
3. Copy the **HTTPS** or **SSH** link.
4. Open terminal and run the following command:
   ```bash
   git clone https://github.com/username/repository.git
   ```
5. Navigate into the cloned project directory:
   ```bash
   cd repository
   ```

### Example:

```bash
git clone https://github.com/torvalds/linux.git
cd linux
```

This will download the complete project to your local machine for development or testing.

---

## 3. Advantage of Paying for Microsoft Windows 11 Upgrade

Upgrading to a licensed version of Windows 11 offers several benefits, especially in terms of cybersecurity:

### Security Advantages:

- **Regular Security Updates**: Paid versions receive ongoing updates and patches to protect against malware and vulnerabilities.
- **Windows Defender**: Enhanced version of built-in antivirus and firewall tools.
- **BitLocker Encryption**: Full-disk encryption feature available in Pro and Enterprise editions.
- **Secure Boot**: Ensures only trusted software runs during system startup.
- **Virtualization-based Security (VBS)**: Isolates sensitive processes from the OS.

### Other Benefits:

- Access to **Windows Sandbox**, **Hyper-V**, and other advanced tools.
- Better **customer support** from Microsoft.
- Compatibility with enterprise-level apps and security features.

---

## 4. Conclusion

Today’s session covered essential Linux commands for navigating and managing files, demonstrated how to clone repositories from GitHub for collaborative development, and highlighted the cybersecurity benefits of upgrading to a paid version of Windows 11.

