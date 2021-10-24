### To add templates into your Zabbix distribution:
1. Read notes
0. Download the desired.xml
0. From Zabbix Web GUI: "Configuration"->"Templates" and click "Import"
0. Select the downloaded.xml and click on "Import" button
0. Enjoy your brand new template!

### **NOTES** for Template Cisco WLC

The value mapping AP MAC -> NAME ("Administration"->"General"->"Value mapping"->"Create value map"):

AP MAC: It's the corresponding AP "RADIO" MAC Address;

NAME: You can chose anithing suits to you, i've have hostnames like AP1, AP2, ecc

### NOTE: The MAC must be in "UPPERCASE" and without the colons ":"

EXAMPLE:

NAME: AP MAC -> NAME

Mappings: 78 BA F9 B2 7C 8C => AP1

The regular expression ("Administration"->"General"->"Regular expressions"->"New regular expressions")

Expression: Virtual Interface

Expression type: Result is FALSE

CaseSensitive: FALSE (unticked)

EXAMPLE:

NAME: WLCs uplink interfaces

Expression type: Result is FALSE

Expression: Virtual Interface

CaseSensitive: FALSE (unticked)

### The MIB's file

copy mib file to MIB' directory