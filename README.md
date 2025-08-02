# Offensive-Security-Intro-tryhackme
Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

Your First Hack
We will use a command-line application called "Gobuster" to brute-force FakeBank's website to find hidden directories and pages. Gobuster will take a list of potential page or directory names and try accessing a website with each of them; if the page exists, it tells you.

Step 1. Open A Terminal

A terminal, also known as the command line, allows us to interact with a computer without using a graphical user interface. On the machine, open the terminal by clicking on the Terminal icon on the right of the screen.

<img width="221" height="189" alt="image" src="https://github.com/user-attachments/assets/1a5d0cf8-90c4-4978-89d7-e975e3115e0e" />


Step 2. Use Gobuster To Find Hidden Website Pages

Most companies have an admin portal page, giving their staff access to basic admin controls for day-to-day operations. For a bank, an employee might need to transfer money to and from client accounts. Due to human error or negligence, there may be instances when these pages are not made private, allowing attackers to find hidden pages that show or give access to admin controls or sensitive data.

To begin, type the following command into the terminal to find potentially hidden pages on FakeBank's website using Gobuster (a command-line security application).
ubuntu@tryhackme:~/Desktop$ gobuster -u http://fakebank.thm -w wordlist.txt dir

=====================================================
Gobuster v2.0.1              OJ Reeves (@TheColonial)
=====================================================
[+] Mode         : dir

[+] Url/Domain   : http://fakebank.thm/

[+] Threads      : 10

[+] Wordlist     : wordlist.txt

[+] Status codes : 200,204,301,302,307,403

[+] Timeout      : 10s

=====================================================
2024/05/21 10:04:38 Starting gobuster
=====================================================
/images (Status: 301)
/bank-transfer (Status: 200)
=====================================================
2024/05/21 10:04:44 Finished
=====================================================
In the command above, -u is used to state the website we're scanning, -w takes a list of words to iterate through to find hidden pages.


