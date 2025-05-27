DDos Attack Sequence Diagram 
This diagram show the sequence of ineruption on a companys web server. This shows how the attackers take control of the servers web flow.

'''Mermiad 
sequenceDiagram 
  Participant Attacker 
  Participant BotNet
  Participant Webserver 
  Participant Firewall 

  '''

  Attacker->>>BotNet: Sends attack command 
  BotNet->>>Webserver: Floods with requests
  Webserver->>>Firewall: casue High traffic in servers 
  Firewall->>>webserver: analyzing traffic flow 
  Firewall->>>BotNet: Block IPs address 
  BotNet->>>Webserver: looking for IP address
  Firewall->>>Firewall: filter out attackers flow 
  Firewall->>>Attacker: Report 
