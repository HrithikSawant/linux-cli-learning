```bash
# by default sort is in ascending alphabetical manner 
sort animal.txt
alpaca	Intermediate Perl	2012	Schwartz, Randal
donkey	Cisco IOS in a Nutshell	2005	Boney, James
horse	Linux in a Nutshell	2009	Siever, Ellen
oryx	Writing Word Macros	1999	Roman, Steven
python	Programming Python	2010	Lutz, Mark
robin	MySQL High Availability	2014	Bell, Charles
snail	SSH, The Secure Shell	2005	Barrett, Daniel

# decending order (-r option)
sort -r animal.txt
snail	SSH, The Secure Shell	2005	Barrett, Daniel
robin	MySQL High Availability	2014	Bell, Charles
python	Programming Python	2010	Lutz, Mark
oryx	Writing Word Macros	1999	Roman, Steven
horse	Linux in a Nutshell	2009	Siever, Ellen
donkey	Cisco IOS in a Nutshell	2005	Boney, James
alpaca	Intermediate Perl	2012	Schwartz, Randal

# sort numerical (-n option) ascending
cut -f3 animals.txt | sort -n
1999
2005
2005
2009
2010
2012
2014

# sort numerical decending
cut -f3 animals.txt | sort -nr
2014
2012
2010
2009
2005
2005
1999

# maximum and minumum values
cut -f3 animals.txt | sort -nr | head -n1
2014

cut -f3 animals.txt | sort -n | head -n1
1999
```
