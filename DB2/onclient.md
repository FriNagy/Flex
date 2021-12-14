# Einrichten DB2 on Client

nach der Installation auf Client in DB2 cmd Fenster wechesln
da muss der Server im Catalog aufgenommen werden

zB:  `db2 catalog tcpip4 node db2inst remote 192.168.14.14 server 50000`

muss auch das Datenbank im Catalog

mit: `db2 catalog database FLEX01 at node db2inst`

erst danach können wir 

mit: `Connect to FLEX01 USER FlexUser USING FlexPwd`

zu Datenbank verbinden und haben vollen zugriff


```
:expdat
echo export %1 %2
db2 -z c:\df\exprot.txt export to %expdir%%2.dbx OF DEL modified by nochardel coldelx7F timestampformat=\"yyyymmdd hh:mm.ss\" decplusblank striplzeros Select * from %1.%2
rem @if errorlevel 2 ( @echo "FAILED to export..." && @pause ... && @goto :EOF )
GOTO :EOF
```
