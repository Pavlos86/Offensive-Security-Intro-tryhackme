# Offensive-Security-Intro-tryhackme
Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

# Your First Hack
We will use a command-line application called "Gobuster" to brute-force FakeBank's website to find hidden directories and pages. Gobuster will take a list of potential page or directory names and try accessing a website with each of them; if the page exists, it tells you.

# Step 1. Open A Terminal

# Step 2. Use Gobuster To Find Hidden Website Pages
gobuster -u http://fakebank.thm -w wordlist.txt dir

To execute this command without errors, you must be in the same directory where wordlist.txt is located.

If wordlist.txt is somewhere else, you need to use the full path, like: gobuster dir -u http://fakebank.thm -w ~/Documents/wordlist.txt

In the command above, -u is used to state the website we're scanning, -w takes a list of words to iterate through to find hidden pages.

You will see that Gobuster scans the website with each word in the list, finding pages that exist on the site. Gobuster will have told you the pages in the list of page/directory names (indicated by Status: 200).

# Step 3. Hack The Bank

You should have found a secret bank transfer page that allows you to transfer money between bank accounts (/bank-transfer). Type the hidden page into the FakeBank website using the browser's address bar.

From this page, an attacker has authorized access and can steal money from any bank account. As an ethical hacker, you would (with permission) find vulnerabilities in their application and report them to the bank to fix them before a hacker exploits them.

Your mission is to transfer $2000 from bank account 2276 to your account (account number 8881). If your transfer was successful, you should now be able to see your new balance reflected on your account page.

Go there now and confirm you got the money! (You may need to hit Refresh for the changes to appear)


