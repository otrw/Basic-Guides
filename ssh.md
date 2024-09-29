1. Connect to a VM:
```bash
ssh ubuntu-desktop
```

2. Copy a file to a VM:
```bash
scp /path/to/local/file ubuntu-server-1:/path/on/remote/server
```

3. Copy a file from a VM:
```bash
scp ubuntu-server-2:/path/on/remote/server /path/to/local/destination
```

4. Run a command on a VM without logging in:
```bash
ssh ubuntu-server-3 'ls -l /home'
```

5. Start an SSH session with X11 forwarding (for GUI applications):
```bash
ssh -X ubuntu-desktop
```

6. Use SSH as a SOCKS proxy (for accessing internal network resources):
```bash
ssh -D 8080 ubuntu-server-1
```
Then configure your browser to use SOCKS proxy localhost:8080

7. Keep SSH connection alive (useful for unstable connections):
```bash
ssh -o ServerAliveInterval=60 ubuntu-desktop
```

