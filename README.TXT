This program was written as an assignment for “Using Databases with Python”
by University of Michigan and www.courser.org 
https://www.coursera.org/learn/python-databases/home/welcome


The program takes a text file which contains email addresses as an argument and counts up the number email messages per organization (we suggest that every organization has his uniq domain name).
It creates a database file and a table named “Counts.” The table has two columns: organization and count. 
Then the program reads the mailbox data and uses a regular expression to separate the domain names. It puts the domain names in the “org” column and adds “1” to the number in the “count” column when the same domain names occurs. 

An example of input file(mbox.txt): 

From stephen.marquard@uct.ac.za Sat Jan  5 09:14:16 2008
Return-Path: <postmaster@collab.sakaiproject.org>
Received: from murder (mail.umich.edu [141.211.14.90])
	 by frankenstein.mail.umich.edu (Cyrus v2.3.8) with LMTPA;
	 Sat, 05 Jan 2008 09:14:16 -0500
X-Sieve: CMU Sieve 2.3
Received: from murder ([unix socket])
	 by mail.umich.edu (Cyrus v2.2.12) with LMTPA;
	 Sat, 05 Jan 2008 09:14:16 -0500
Received: from holes.mr.itd.umich.edu (holes.mr.itd.umich.edu [141.211.14.79])
	by flawless.mail.umich.edu () with ESMTP id m05EEFR1013674;
	Sat, 5 Jan 2008 09:14:15 -0500 count up using a database with the following schema to maintain the counts.
……..

Output:

Enter file name: mbox.txt
Counts:
iupui.edu 536
umich.edu 491
indiana.edu 178
caret.cam.ac.uk 157
vt.edu 110
uct.ac.za 96
media.berkeley.edu 56
ufp.pt 28
gmail.com 25
et.gatech.edu 17