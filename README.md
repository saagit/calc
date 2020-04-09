# calc
A trivial Perl script to use as a command line based calculator.

I implemented this ages ago because I really like to have calculations
I make in bash's history for easy recall and editing.  I used Perl
because its arithmetic syntax most resembled C by it is interpreted.

Note you'll frequently need to quote the expressions.

Some examples:
```
$ calc
usage: calc [-x|-o|+FORMAT] expression
$ calc '2<<24'
33554432
$ calc -x '2<<24'
0x2000000
$ calc -o '2<<24'
0200000000
$ calc '+%08X' 29
0000001D
$ calc pi*12
37.699112
$ calc '(818 + 61) * 54'
47466
$ calc 'cos(pi/2)'
0.000000
$ calc 'sin(pi/2)'
1
$ calc -x '(1<<16)|(3<<5)'
0x10060
$ calc 'time()'
1586393625
$ calc 'time()/365.25/24/60/60'
50.269782
```
