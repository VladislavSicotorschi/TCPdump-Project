# TCPdump-Project
Analyze Network Traffic with TCPDump: Build a Logging Tool

Preparing enviroment:
1. Created VM using Oracle VirtualBox

2. Deployed Linux distribution Ubuntu image on VM

3. Installed Tcpdump on VM: ###sudo apt-get install tcpdump

4. Installed Wireshark on VM: ###sudo apt install wireshark -y

5. Installed Microso Visual Studio Code on VM: ###sudo snap install --classic code

Task 1 Testing tcpdump commands:

1. Ran command "tcpdump" to capture some packets (ctl+c to stop capture)
2. Ran command "tcpdump -c 10" to limit cature to 10 packets
3. Ran command "tcpdump -c 10 -#XXtttt" to capture 10 packets with detailed hex and ASCII output, including timestamps(tttt)

Task 2 Bulding logging tool script:

1. Ran command "sudo tcpdump -D" to list all available network interfaces for packet capture
2. Ran command "sudo tcpdump -i lo" to capture network traffic on the loopback interface (lo).
3. open new terminal and ran "ping localhost" to send ICMP echo requests to localhost to generate network traffic on the loopback interface(lo).(ctl+c to stop pings)
4. Ran command "sudo tcpdump -#XXtttt host coursera.org" to captured and displayed detailed output of network traffic involving coursera.org, including timestamps
