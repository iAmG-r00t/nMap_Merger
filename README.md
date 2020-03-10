# What is this?
Ever needed to merge results of several nmap scans into one, cute and browseable page?
This tool does just that!

# What will I get as output?
Below is screenshots of what you will get.
(All credits go to https://github.com/honze-net/nmap-bootstrap-xsl)
![scanme screenshot 1](https://raw.githubusercontent.com/honze-net/nmap-bootstrap-xsl/master/scanme-screenshot1.png)
---
![scanme screenshot 2](https://raw.githubusercontent.com/honze-net/nmap-bootstrap-xsl/master/scanme-screenshot2.png)
---
![scanme screenshot 3](https://raw.githubusercontent.com/honze-net/nmap-bootstrap-xsl/master/scanme-screenshot3.png)

# Cool! Now, how to use it?
**NOTE: Nmap output must be in XML format (nmap -oX flag)**

and: it requires **python3**!

<pre>usage: nMapMerge.py [-h] [-f FILE] [-d DIR] [-q]
<br>optional arguments:
<br>    -h, --help            show this help message and exit
<br>    -f FILE, --file FILE  parse FILE
<br>    --d DIR, --dir DIR    parse all xml in directory
<br>    --q, --quiet          don't print status messages to stdout
<br>    -t, --target          target file to generate, default: nmapMerged.xml</pre>

# Examples
Merge all XML files from a directory *nmap_out* into a single file *singleReport.xml*
```
python3 nMapMerge.py -d nmap_out -t singleReport.xml
```
now, open that XML in your browser (Chrome might fail, but Firefox always works!)
