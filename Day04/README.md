📒 README — Day 04: Cybersecurity & Ethical Hacking
🗓️ Date: Day 04
🎯 Focus: TCP/UDP, Networking Concepts, Nmap Flags, and ifconfig
✅ Topics Covered
1. 🌐 TCP vs UDP
Feature	TCP	UDP
Full form	Transmission Control Protocol	User Datagram Protocol
Connection	Connection-oriented	Connectionless
Reliability	Reliable (guaranteed delivery)	Unreliable (no guarantee)
Speed	Slower (due to handshaking)	Faster (no overhead)
Use Cases	Web, Email, FTP	Streaming, DNS, VoIP
Packet Order	Maintains order	No guarantee of order
Acknowledgment	Yes	No

2. 📡 ifconfig
Command used to view and configure network interfaces.

Run:

bash
Copy
Edit
ifconfig
Key fields:

inet: IP address

ether: MAC address

tx/rx: Transmit/receive packets

3. 🕵️ Nmap Scanning
Nmap is a powerful tool for network discovery and security auditing.

Commonly used flags:
bash
Copy
Edit
nmap -Pn -A -sV -O -oN output.txt --script vuln -vv -p- <target>
Flag	Purpose
-Pn	Skip ping (assume host is up)
-A	Aggressive scan: OS detection, version, script
-sV	Service version detection
-O	OS detection
-oN	Output normal format to file (output.txt)
--script	Run a script (e.g., vuln for vulnerabilities)
-vv	Very verbose output
-p-	Scan all 65535 ports

Example:

bash
Copy
Edit
nmap -Pn -A -sV -O --script vuln -vv -p- 192.168.1.1
🧠 Key Takeaways
TCP = Reliable but slow, UDP = Fast but unreliable.

Use ifconfig to identify your machine’s IP and network state.

Mastering nmap is essential for vulnerability assessments.
