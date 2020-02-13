# nMap_Merger
<br>Requires python3
<br>
<br>Merge multiple nMap xml files into one XML which is human-browsable via Browser
(thanks to https://github.com/honze-net/nmap-bootstrap-xsl/)

<pre>usage: nMapMerge.py [-h] [-f FILE] [-d DIR] [-q]
<br>optional arguments:
<br>    -h, --help            show this help message and exit
<br>    -f FILE, --file FILE  parse FILE
<br>    --d DIR, --dir DIR     Parse all xml in directory
<br>    --q, --quiet           don't print status messages to stdout</pre>
<br>    -t, --target          target file to generate, default: nmapMerged.xml
<br>nMapMerge.py -f nMap_out.xml
<br>nMapMerge.py -d /root/nMap/
