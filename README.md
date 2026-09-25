# cyber-journey
Percorso personale di studio verso Cyber Defence e Ethical Hacking
Risorse principali: serie Free CCNA di NetworkChuck, Wireshark, Packet Tracer, TryHackMe.

## Log settimanale - giorno 1: wireshark

**22/09** — Primo utilizzo di Wireshark: ho catturato una query DNS reale sulla mia rete di casa, riconosciuto i layer OSI in un pacchetto (Ethernet II, IPv6 link-local, UDP porta 53, DNS), capito la differenza tra indirizzo MAC locale e IP end-to-end. Visto anche una richiesta HTTP in chiaro con tutti gli header (Host, User-Agent, Accept-Language) e capito perché HTTPS esiste.

## Log settimanale - giorno 2: packet tracer + routing
**24/09** — Prima rete completa in Packet Tracer: 2 PC + switch, ping riuscito. Errore iniziale: avevo piazzato un router al posto dello switch (le interfacce di un router sono spente di default e serve configurazione via CLI, uno switch invece funziona subito). Poi ho rifatto l'esercizio con il router configurato correttamente, mettendo i due PC su due subnet diverse (192.168.1.0/24 e 192.168.2.0/24) e collegandoli tramite routing reale, con comandi CLI (`interface`, `ip address`, `no shutdown`). Ping riuscito anche in quel caso.

## Come farò pratica con Packet Tracer
- Uso i laboratori guidati (.pka) forniti dal corso NetAcad, che si autovalutano.
- Ogni volta che NetworkChuck mostra una topologia di rete, provo a ricostruirla da solo prima di vedere come la fa lui.
- Aumento la complessità man mano che avanza la teoria: VLAN, DHCP, subnet multiple.
- Ricostruisco a memoria l'ultima rete complessa vista, senza guardare appunti — dove mi blocco è la mia lista di ripasso.

- ## Log settimanale - giorno 3: pratica con Packet Tracer
**24/09** — Confronto pratico Hub vs Switch in Packet Tracer: ho collegato più PC prima tramite un hub, poi tramite uno switch, e testato l'invio di messaggi/ping tra loro. Con l'hub, il traffico veniva ripetuto su tutte le porte indipendentemente dal destinatario (dispositivo di Layer 1, nessuna intelligenza sull'indirizzamento). Con lo switch, il traffico veniva inoltrato solo alla porta del vero destinatario, perché impara e associa gli indirizzi MAC alle porte (Layer 2). Ho anche configurato una connessione wireless tra un laptop e un router wireless, verificando la connettività.
