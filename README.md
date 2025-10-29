# Using-Wireshark---analyzing-web-browser-artifacts-email-header-analysis

### Name : Mohammed Ibrahim MN 
### Reg No : 212223100034

## AIM:
To use Wireshark to analyze web browser activities and inspect email headers from captured network traffic.

## DESIGN STEPS:
### Step 1:
Launch Wireshark and start capturing traffic on the appropriate network interface.

### Step 2:
Use filters like http, dns, or tcp.port == 80 to monitor web browser artifacts such as visited URLs, cookies, and user-agent strings.

### Step 3:
Apply filters like smtp, pop, or imap to locate and analyze email header details (e.g., sender, receiver, subject) from email communications.

## PROGRAM:
Wireshark Web and Email Traffic Filtering Steps

## OUTPUT:
# A. Capturing Traffic in Wireshark

1.Open Wireshark and start capturing on the active interface (Wi- Fi/Ethernet).

2.Perform activities like opening a website or sending an email through a client (e.g., Gmail via browser or Thunderbird).

3.Stop the capture once done.
![435752115-04f9e42a-15ca-4cc2-a81c-97b889bb176b](https://github.com/user-attachments/assets/6a654494-4cde-405f-a45b-9505ea0e6ea5)
Analyze DNS Queries: o Filter: dns

Reveal domains the browser tried to resolve.
![435752556-eb10207d-d377-448d-beef-9985f73ae7ff](https://github.com/user-attachments/assets/0650a35c-dd56-4231-9800-7b09045f2588)
Email Header Analysis

# Apply relevant filters:
 For POP3: tcp.port == 110

For SMTP: tcp.port == 25 or 587

 For IMAP: tcp.port == 143 or 993

# Locate email data:
 Look for SMTP packets to see sender/receiver email addresses.

 Use "Follow TCP Stream" to view the full email headers and body if unencrypted.

# Extract Email Header Fields:

 Analyze From, To, Subject, Date, Message-ID, and relay servers used in sending the email.
 ![435754056-0bd101fe-2793-4eb1-b064-3ccaffd3ee3d](https://github.com/user-attachments/assets/c0c6d519-cc46-4433-88af-c8f265a3d1a6)
![435754283-37843833-560e-4dfa-ad86-8f3a4d0f53b2](https://github.com/user-attachments/assets/3c7ffbef-51ed-495e-803b-1f137c32c5c2)
![435754706-32698667-c3a1-4720-a813-56f94cf3da69](https://github.com/user-attachments/assets/c3cb3788-34f7-45ba-a318-4a51b9be027a)


## RESULT:
Web browser artifacts and email headers were successfully analyzed using Wireshark.

