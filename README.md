<style>
r { color: Red }
o { color: Orange }
g { color: palegreen }
blu { color: lightskyblue }
cmd { color: #569CD6; }
arg { color: #9CDCFE; }
grey { background-color: #f6f8fa; }

</style>

# 🐳 Docker Cheatsheet

## <g>docker</g> <blu>images <o>-it 

## Basic Commands

### **Container Lifecycle**
- <g>docker</g> <blu>run</blu> &lt;image&gt; : Start a new container
    - `-d` (detached)
    - `-p HOST:CONTAINER` (ports)
    - `--name` (assign name)
    - `--rm` (auto-remove)
- **`docker exec -it <container> <cmd>`**: Run command in container
    - `-it` (interactive TTY)
    - `-e VAR=val` (env vars)


### **Container Lifecycle**

<details>
<summary><strong><g>docker</g> <blu>run</blu> &lt;image&gt;</strong> - Start a new container</summary>

- `-d` (detached mode)
- `-p` <span style="color: #CE9178;">HOST:CONTAINER</span> (port mapping)
- `--name` <span style="color: #CE9178;">&lt;name&gt;</span> (assign name)
- `-v` <span style="color: #CE9178;">HOST:CONTAINER</span> (volume mount)
- `-e` <span style="color: #CE9178;">VAR=val</span> (env variables)
- `--rm` (auto-remove after exit)

</details>

<details>
<summary><strong><span style="color: #4EC9B0;">docker run</span> <span style="color: #CE9178;">&lt;image&gt;</span></strong> - Start a new container</summary>

- `-d` (detached mode)
- `-p` <span style="color: #CE9178;">HOST:CONTAINER</span> (port mapping)
- `--name` <span style="color: #CE9178;">&lt;name&gt;</span> (assign name)
- `-v` <span style="color: #CE9178;">HOST:CONTAINER</span> (volume mount)
- `-e` <span style="color: #CE9178;">VAR=val</span> (env variables)
- `--rm` (auto-remove after exit)
</details>

<details>
<summary><strong><span style="color: #4EC9B0;">docker exec -it</span> <span style="color: #CE9178;">&lt;container&gt; &lt;cmd&gt;</span></strong> - Run command in container</summary>

- `-it` (interactive TTY)
- `-e` <span style="color: #CE9178;">VAR=val</span> (pass env vars)
- `--user` <span style="color: #CE9178;">&lt;user&gt;</span> (run as user)
</details>

<details>
<summary><strong><span style="color: #4EC9B0;">docker stop</span> <span style="color: #CE9178;">&lt;container&gt;</span></strong> - Stop a container</summary>

- `-t` <span style="color: #CE9178;">N</span> (timeout in seconds)
</details>

<details>
<summary><strong><code>docker run &lt;image&gt;</code></strong> - Start a new container</summary>

- `-d` (detached mode)
- `-p HOST:CONTAINER` (port mapping)
- `--name` (assign custom name)
- `-v HOST:CONTAINER` (volume mount)
- `-e VAR=val` (set env variable)
- `--rm` (auto-remove after exit)
</details>

<details>
<summary><strong><code>docker start &lt;container&gt;</code></strong> - Start a stopped container</summary>

- `-a` (attach to output)
- `-i` (interactive mode)
</details>

<details>
<summary><strong><code>docker stop &lt;container&gt;</code></strong> - Stop a running container</summary>

- `-t N` (timeout in seconds)
</details>

<details>
<summary><strong><code>docker restart &lt;container&gt;</code></strong> - Restart a container</summary>

- `-t N` (timeout before restart)
</details>

<details>
<summary><strong><code>docker rm &lt;container&gt;</code></strong> - Remove container</summary>

- `-f` (force remove running)
- `-v` (remove volumes)
</details>

<details>
<summary><strong><code>docker exec -it &lt;container&gt; &lt;cmd&gt;</code></strong> - Run command in container</summary>

- `-it` (interactive TTY)
- `-e VAR=val` (pass env vars)
- `--user` (run as specific user)
</details>

## 🤝 Feedback and Contributions

I would be very thankful if you contribute to make this list more complete
