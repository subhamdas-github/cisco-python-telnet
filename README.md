# cisco-python-telnet

```R1> enable```

```R1# conf t```

```R1(config)# int g0/0```

```R1(config-if)# ip address <your machine's ip address> <your machine's subnet mask>```

```R1(config-if)# no shut```

try in terminal: ```telnet <your machine ip address>```
  [Error : Unable to connect to remote host: Connection refused]

```R1(config-if)# exit```

```R1(config)# username <your username> password <your password>```

```R1(config)# line vty 0 4```

```R1(config-line)# login local```

```R1(config-line)# transport input all```

```R1(config-line)# end```

  
try in terminal : ```telnet <your machine ip address>```

It's working now !!!

  
  
```R1# debug telnet```
  
```R1# sh line```

```R1# sh ip int brief```

```R1# sh ip prot```

```R1# sh ip ospf int brief```
