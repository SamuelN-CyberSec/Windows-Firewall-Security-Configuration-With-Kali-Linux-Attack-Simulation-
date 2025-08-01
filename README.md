# Windows-Firewall-Security-Configuration-With-Kali-Linux-Attack-Simulation-
This project demonstrates how to configure the built in windows firewall on windows 11 machine to secure it from unauthorized access using kali linux, I simulated an attack to test the effectiveness of the firewall rule.
# Objective
-Configure custom windows firewall inbound rule 
-Simulate real-world attacks from Kali Linux (port scanning,ping test,) 
-monitor and analyze windows 
-Document network setup and findings

###Tool Used 
- Windows 11**(Host Machine )
- Kali Linux**(Virtual Box guest Machine )
- VirtualBox** (Virtual environment)
-**Nmap**,ping
- **Windows Defender Firewall with Advanced Security **


Network Setup 
-**Windows 11 Host IP**: 192.168.56.1
-**Kali Linux IP **: 192.168.56.102
-**VirtualBox Adapter **: Host Only Network (Isolated:Lab)

##Firewall Rules Configured(Windows 11)
-**Allow HTTP/HTTPS (Port 80,443)**:Enabled
-**Block ICMP(Ping)**:Enabled**
-**Log dropped packet and successful Connection

## Attack Simulation From Kali Linux
##Nmap Scan bash nnmap -sS 192.168.56.1 Result: Ignored State (due to firewall)
##Ping Test: ping 192.168.56.1 Result timed out (ICMP blocked by firewall)

Lesson Learned
*The built in Windows Firewall is effective when configured properly 
*Even simple rule set can defend against basic reconnaissance and intrusion attempts
*Logging is critical for Auditing and incident response

##Screenshots
*Firewall Inbound Rules
*Kali nmap result

f<img width="769" alt="Windows Defende Firewall Inbound Rule" src="https://github.com/user-attachments/assets/1fc21bec-399a-4f5a-bc05-6d98571dd71a" />
<img width="708" alt="kali Linux Communication to Windows 1" src="https://github.com/user-attachments/assets/6c576217-7cdf-4779-852e-f32da02017e7" />
irewall logs 
 
Future improvement
*Adding IDS tool (snort) to the enviromment 
