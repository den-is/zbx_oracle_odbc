###Zabbix template for Oracle databases monitoring via ODBC.

This is kinda fork of Orabbix probes.

Please report any problems, suggest items, fork, etc.

#####Currently supports 
* 57 items
* 15 triggers
* 11 graphs

#####Requirements:
* Oracle client software
* unixODBC configured with proper driver(s) and DSN(s)

#####Installation
* Import template. "Template Oracle ODBC"
* add to oracle host 3 macroses with known values:
  - {$DSN} - your DSN for oracle database You have configured in odbc.ini
  - {$ORA_USER} - database user
  - {$ORA_PASS} - database password

