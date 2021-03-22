Alle Befehle in DB2 Befehlsfenster (Admin)

db2ic --- online DB2 Manual, Select Version 11.5

db2val --- Installation file validation for the DB2

D:\DB2\BIN>db2licm -l
```
Product name:                     "DB2 Community Edition"
License type:                     "Community"
Expiry date:                      "Permanent"
Product identifier:               "db2dec"
Version information:              "11.5"
Max amount of memory (GB):        "16"
Max number of cores:              "4"
```

dmctop  is a free text-based monitoring utility

Ausgeben auf Alt-Server:

db2look -d FDT01 -z dfroot  -e -i db2user1 -w db2pasw1 -o angete

mit -t einzelne Tabelle bestimmen -tw mit wildcard

export ... of del

Einlesen auf Neu-Server:
vorher in Skript login u/o schema anpassen

sql Skript in cmdline:
db2 -tvmf angete.sql

dann in db2:
import from .\myange of del  commitcount 900 replace  into dfroot.angeb

