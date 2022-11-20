```bash
# find all lines containing Nutshell
grep Nutshell animal.txt
horse	Linux in a Nutshell	2009	Siever, Ellen
donkey	Cisco IOS in a Nutshell	2005	Boney, Jame

# Exclude all lines containing Nutshell
grep -v Nutshell animal.txt
python	Programming Python	2010	Lutz, Mark
snail	SSH, The Secure Shell	2005	Barrett, Daniel
alpaca	Intermediate Perl	2012	Schwartz, Randal
robin	MySQL High Availability	2014	Bell, Charles
oryx	Writing Word Macros	1999	Roman, Steven

# print lines that containes the string Perl in files with names ending in .txt
grep Perl *.txt

```
