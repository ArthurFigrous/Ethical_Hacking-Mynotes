📒 README — Day 03: Cybersecurity & Ethical Hacking
🗓️ Date: Day 03
🎯 Focus: Kali Linux Booting, Interface Tour, Reconnaissance & File Permissions
✅ Topics Covered
1. 🔧 Booting Kali Linux via VirtualBox
Verified VM settings (RAM: ≥2GB, 2 CPUs, NAT network).

Booted into Kali using default credentials (kali / kali).

Resolved login or display issues (if any).

2. 🧭 Kali Linux Interface Walkthrough
XFCE desktop interface basics.

Opened terminal, explored file system with:

bash
Copy
Edit
pwd        # show current directory
ls -la     # list files with permissions
cd         # change directory
3. 🌐 Networking Refresher
IP address check:

bash
Copy
Edit
ip a
Concepts: MAC address, DNS, Gateway.

Used:

bash
Copy
Edit
ping <target>
4. 🕵️ Introduction to Reconnaissance
Types: Passive vs Active.

Used tools:

nmap: Network scanning.

bash
Copy
Edit
nmap <IP_address>
nmap -sV <IP_address>
5. 🔐 Linux File Permissions
Permissions are represented in symbolic (rwx) and numeric (0–7) formats.

Number	Permission	rwx Representation
0	none	---
1	execute only	--x
2	write only	-w-
3	write & execute	-wx
4	read only	r--
5	read & execute	r-x
6	read & write	rw-
7	read, write, exec	rwx

Example:

bash
Copy
Edit
chmod 755 filename
# Means: rwxr-xr-x
🧠 Key Takeaways
Kali Linux is a hacker’s toolkit — get familiar with its layout.

Networking is the entry point to hacking; always know your IP.

Permissions are your gatekeepers — understand and use them well.

Let me know if you'd like this as a downloadable .md file or if you're maintaining a folder-based documentation structure.
