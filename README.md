# Zabbix template for Oracle databases monitoring via ODBC

This template monitors Oracle database health, performance, security audit, etc.

This is kinda fork of [Orabbix](http://www.smartmarmot.com/product/orabbix/) probes.

Please report any problems, suggest items, fork and so on.

### Currently supports
* 57 items
* 15 triggers
* 11 graphs

### Requirements
* Zabbix 2.0+
* Oracle client software
* unixODBC configured with proper driver(s) and DSN(s)

### Installation
* Import template. "Template Oracle ODBC"
* Add to oracle host 3 macroses with known values:
  - **{$DSN}** - your DSN for oracle database You have configured in odbc.ini
  - **{$ORA_USER}** - database user
  - **{$ORA_PASS}** - database password

### Known issues
* **Audit** item returns "empty" result. *Disabled by default*.
* **Locks** item returns "empty" result. *Disabled by default*.
* **Tablespaces** item returns "empty" result. *Disabled by default*.
* **Users Locked** item returns "empty" result. Fixed for now with SQL by itself. *Enabled by default*.
