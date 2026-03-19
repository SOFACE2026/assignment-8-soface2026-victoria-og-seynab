Emne 1:
What is an IP address?

En IP-adresse er en unik tal-adresse, som fungerer som en computers ”post-adresse” på et netværk. 

Why do we need IP addresses?

Vi har brug for IP-adresser, fordi de fungerer som et unikt identifikationsnummer for hver enhed på et netværk. Vi vil kunne vide hvem der sender data, og hvor data skal leveres (modtager) med IP-adresser.

What is the relation between TCP and IP?

IP (Internet Protocol) er ligesom postvæsnet, som sørger for selve adresseringen og finder ruter, så pakkerne kan blive sendt fra én IP-adresse til en anden. Den kan ikke garanterer, at pakken når frem.

TCP (Transmission Control Protocol) er som et anbefalet brev, som kører ovenpå IP og sørger for, at data kan blive leveret fejlfrit, og i de rigtige rækkefølger, og den sørger også for at de ikke forsvinder undervejs.

What is a socket? Have you heard of different types of sockets?

En socket er et software-endepunkt, der gør det muligt for et program at sende eller modtage data over et netværk. Den består af en IP-adresse og et port-nummer. Der er en TCP type og en UDP type.

What is up with the address: 127.0.0.1?

Det er en "localhost" eller en loopback-adresse. Den får ens computer til at kunne sende data til sig selv. 



Emne 2:
What does a client-server architecture mean? 

En Klient-Server arkitektur er en distribueret struktur, der opdeler opgaver mellem to typer komponenter: server og klient. Ansvaret er skarpt opdelt her. Serveren er en ressource, der venter passivt på forespørgsler. Klienten er den aktive part, der tager initiativ til kommunikationen for at få adgang til data. Èn server kan typisk betjene flere klienter på samme tid. 

Give a concrete example of where you would encounter this in real life. 

En webbrowser (klienten) og en webserver (serveren), fx når man indtaster google.dk, så sendes browseren en http-anmodning over netværket, og serveren modtager admodningen, derefter finder de ønskede data og sender tilbage som svar.

How do you decide who is the server and who is the client?

Klienten er den enhed, der starter forbindelsen.
Serveren er den enhed, der lytter på en bestemt port og svarer på anmodningen.

Emne 3:
What is the difference between client-server architecture and the broker architecture?

I en Klient-Server arkitektur, kommunikerer klienten direkte med en kendt server for at anmode om en ressource, hvor klienten skal kende serverens præcise adresse (IP/port). 
Broker-arkitekturen indfører en mellemmand (en broker), hvor klienten ikke behøver at kende den endelige udbyders placering. Den sender bare sin anmodning til brokeren, som derefter videresender den til den rette modtager.

What are the benefits to the broker pattern? 

Klienter og servere er uafhængige af hinanden, hvor klienten kun skal kende en adresse (brokeren) i stedet for hundredvis af forskellige service-adresser. 

What could be potential downsides?

Hvis brokeren går ned, kan ingen dele af systemet kommunikere eller finde hinanden. Da brokeren er en mellemmand, så kan alle beskeder give lidt forsinkelse. 

Emne 4:
What does Peer-to-Peer mean? 

Peer-to-Peer er en decentraliseret arkitektur, hvor alle computere i netværket har samme rettigheder og ansvarsområder.

What are the main characteristics of this architecture? 

I modsætning til klient-server modellen, er der ingen central autoritet. Hver af dem fungerer som både klient og server og kommunikationen sker direkte mellem dem.

Have you encountered it anywhere online? 

Skype eller Bitcoin

Does Peer-to-Peer applications mean that there are no servers and only clients? 

Det betyder ikke nødvendigvis, at der slet ikke er servere. Mange P2P-applikationer bruger en "tracker" eller en "broker" (en server) til at hjælpe nodes med at finde hinanden, men selve dataoverførslen sker direkte mellem nodes.

What benefits could there be to using this pattern? 

Der er intet "single point of failure"; hvis én computer går offline, kører netværket videre.

What downsides could there be to this pattern? 

Hvis ingen peers har den specifikke fil, du leder efter, online samtidig, kan du ikke få fat i den.



