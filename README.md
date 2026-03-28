/* Author : George Botrs Azer Date : 2026-3-28 Description:A Simple Write up for Intro Poc Scripting */

Task2,Example - The starting point :
1-What is the target's platform and version number?

-Answer:
Webmin 1.580

2-What is the associated CVE for this platform?

-Answer:
CVE-2012-2982

3-Which file does the vulnerability exist in?

-Answer:
file/show.cgi

4-What program/command would be the most effective to use in this exploit?

-Answer:
System Shell


#Task3,Translating Metasploit module code :

1-What's the original disclosure date of this exploit?

-Answer:
September 6 2012

2-What HTTP response code do we expect after the initial POST request?

-Answer:
302

3-What HTTP response code do we expect after the initial POST request?

-Answer:
Session ID, authentication

4-In the check function, what is it doing to the cookies?

-Answer:
format

5-In the second request of the check function, what method is piped into the command?

-Answer:
rand_text_alphanumeric


#Task4,Converting Ruby to Python :

1-Which HTTP response header allows us to send an authenticated POST request?

-Answer:
set-cookie


2-Which is the correct method for formatting cookies in this example?

r.headers().replace().split().strip()

r.headers().split().strip()

a = r.cookies()
b = a.strip()

-Answer:
any

3-What data type does the payload need to be?

-Answer:
string

4-Why do we need to use "bash -c exec" instead of just "bash -i"

Answer:
replaces current shell process

5-What is the purpose of "<&1" in the payload function?

-Answer:
redirects socket output stream to bash input stream


#Task5,Final exploit and test :

1-Run the program and listen for the shell. What is the /root/root.txt flag?

-Answer:
THM{ur_So_1337!@#$}


