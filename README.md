# TA-PassiveDNS
CIM compliant Technology Add-on for Gamelinux PassiveDNS (https://github.com/gamelinux/passivedns)


Captures data in the following format from /var/log/passivedns.log:

#timestamp||dns-client ||dns-server||RR class||Query||Query Type||Answer||TTL||Count
1322849924.408856||10.1.1.1||8.8.8.8||IN||upload.youtube.com.||A||74.125.43.117||46587||5
1322849924.408857||10.1.1.1||8.8.8.8||IN||upload.youtube.com.||A||74.125.43.116||420509||5
1322849924.408858||10.1.1.1||8.8.8.8||IN||www.adobe.com.||CNAME||www.wip4.adobe.com.||43200||8
1322849924.408859||10.1.1.1||8.8.8.8||IN||www.adobe.com.||A||193.104.215.61||43200||8
1322849924.408860||10.1.1.1||8.8.8.8||IN||i1.ytimg.com.||CNAME||ytimg.l.google.com.||43200||3
1322849924.408861||10.1.1.1||8.8.8.8||IN||clients1.google.com.||A||173.194.32.3||43200||2

Headers are not included in the passivedns.log file.

## Installation

1. Install the TA on your indexer and search head
2. Set up Splunk to monitor /var/log/passivedns.log using the following sourcetype: gamelinux:passivedns
3. Done
