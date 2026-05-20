# Network-Simulation

Aufbau eines sicheren, segmentierten Unternehmensnetzwerks mit Cisco Packet Tracer.

## Technologien
- VLAN · DHCP · ACL · SSH v2 · Sticky MAC · DNS

## Netzwerktopologie
- 1 Router (Router-on-a-Stick)
- 1 Core-Switch
- 4 Abteilungs-Switches (IT, HR, Gast, Server)
- 1 DNS-Server

## Was umgesetzt wurde
- VLAN-Segmentierung – 4 isolierte Broadcast-Domänen
- DHCP – automatische IP-Vergabe pro VLAN
- ACL – Gäste haben nur Zugriff auf DNS-Server
- Sticky MAC – Port Security auf allen Access-Switches
- SSH v2 – verschlüsselter Remote-Zugriff, Telnet deaktiviert

## Testergebnisse
- VLAN-übergreifender Ping erfolgreich
- Gast → IT: 100% Paketverlust (ACL greift korrekt)

## Datei
- `netzwerk.pkt` – Cisco Packet Tracer Projektdatei
