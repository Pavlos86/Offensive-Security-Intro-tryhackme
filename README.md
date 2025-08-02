# Offensive-Security-Intro-tryhackme
Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

Your First Hack
We will use a command-line application called "Gobuster" to brute-force FakeBank's website to find hidden directories and pages. Gobuster will take a list of potential page or directory names and try accessing a website with each of them; if the page exists, it tells you.

Step 1. Open A Terminal

Step 2. Use Gobuster To Find Hidden Website Pages
gobuster -u http://fakebank.thm -w wordlist.txt dir
