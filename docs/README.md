dokumentatsioon:


Meeskonnaliikmete nimed ja rollid: Tegin üksinda: Berit Ruut

Valitud serverivariant koos põhjendusega: Zone.ee kuna seal oli juba eelnevalt server püsti pandud.

Serverinfo (IP, OS, veebiserver): IP: 217.146.69.55, OS: ZoneOS, ruudus.eu.

SSH seadistuse staatus (võtmepaar, GitHub Secrets):
Lõin ühenduse SSH Zone-i: genereerisin privaat- ja avaliku võtme. Lisasin avaliku võtme Zone-i SSH seadistuse alla ning Github Secretite alla lisasin privaatvõtme. Veel, lisasin GitHubi secretite alla login credentialid. 

Probleemid, mis tekkisid, ja kuidas lahendasid:
GitHubist ei suutnud ühendada Zone-i serveriga. Alustasin sellega, et proovisin enda kohalikku arvutit ühendada SSH kaudu Zone-i serveriga. See töötas, seega olin kindel, et probleem polnud SSH võtmetes, vaid GitHubis seadistuses. Peale mõnda aega kaevamist, leidsin, et kui SSH private key-d lisada, siis peab juurde jätma ka selle osa, kus on -----BEGIN OPENSSH PRIVATE KEY----- ja -----END OPENSSH PRIVATE KEY-----. Kui panin need ka juurde sinna private key-le, siis hakkas asi tööle ning commititud failid tekkisid Zone-i serverisse.

Deploy testmise tulemus:
Nagu eelnvalt mainitud, tekkisid mu commititud failid ilusti Zone-i serverisse ning muudatused tekkisid automaatselt veebis nähtavale.

Kasutasin muudatuste tegemiseks Visual Studio Code-i.


