# Networking Basics #1

## **Description**
This project introduces you to the basics of networking, helping you understand key concepts such as:
- `localhost` and `127.0.0.1`
- `0.0.0.0`
- The `/etc/hosts` file
- How to display active network interfaces on your machine.

You will also learn to use tools such as `ifconfig`, `telnet`, and `nc`.

---

## **Learning Objectives**
By the end of this project, you should be able to answer the following questions without using Google:

### **General**
1. What is `localhost` or `127.0.0.1`?
2. What is `0.0.0.0`?
3. What is the purpose of the `/etc/hosts` file?
4. How can you display your machine's active network interfaces?

---

## **Resources**
- [What is localhost](https://en.wikipedia.org/wiki/Localhost)
- [What is 0.0.0.0](https://en.wikipedia.org/wiki/0.0.0.0)
- [What is the hosts file](https://en.wikipedia.org/wiki/Hosts_(file))
- [Netcat examples](https://www.digitalocean.com/community/tutorials/how-to-use-netcat-to-establish-and-test-tcp-and-udp-connections)
- Commands to explore:
  - `ifconfig`
  - `telnet`
  - `nc`
  - `cut`

---

## **Requirements**
- Allowed editors: `vi`, `vim`, or `emacs`.
- Tested on **Ubuntu 20.04 LTS**.
- All files must end with a new line.
- A `README.md` file at the root of the project is mandatory.
- All Bash scripts must:
  - Be executable.
  - Pass Shellcheck (version 0.7.0) without any errors.
  - Have the first line exactly as `#!/usr/bin/env bash`.
  - Include a comment on the second line explaining what the script does.

---

## **Tasks**

### **0. Change your home IP**
**File:** `0-change_your_home_IP`

Write a Bash script that configures an Ubuntu server with the following requirements:
- `localhost` resolves to `127.0.0.2`.
- `facebook.com` resolves to `8.8.8.8`.

#### **Example Execution:**
Before running the script:
```bash
ping localhost
# localhost resolves to 127.0.0.1
ping facebook.com
# facebook.com resolves to its default IP
