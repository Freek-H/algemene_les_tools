Data Warehouse (Voorbeeld klanttevredenheidsonderzoek (KTO)):
- Bron
	- Telefonisch
	- Webchat
	- Website
	- Receptie
- Staging
	- Opgeschoond
	- Conformeren aan kwaliteit
- Integratie
	- Samenvoegen tot één model
- Rapportage
	- Businesstermen toevoegen
- De Bron, Staging en Integratie lagen bevatten kopiën van de data. Afhankelijk van de smaak geldt dit mogelijk ook nog de Rapportagelaag.

Data Vault 2.0
- Filosofie:
	- Data komt binnen as-is
	- Kwaliteitsverantwoordelijkheid ligt bij de bronnen
	- Maar één kopie van de data en daarmee één waarheid

- Hub tabellen
	- Informatie die niet veranderd
		- Bijv. voornaam, achternaam
	- Keys naar Satellieten
	- Keys naar Links
- Satelliet tabellen
	- Informatie die wel veranderd
		- Adres
		- Telefoonnummer
	- Gegegroepeerd op informatie die tegelijkertijd zal veranderen
		- Straatnaam, straatnummer, postcode, woonplaats
	- Keys naar Hub
- Link tabellen
	- Alle transacties
	- Keys naar Hubs

Normalisatie (https://nl.wikipedia.org/wiki/Databasenormalisatie)

Data Lake
- Key: Value
- Program Files\Discord\discord.exe: <binary>
- Gebruikers\Freek\Documenten\Verslag Nederlands.docx: <inhoud van het verslag>

Data Lakehouse
- Grofweg een Data Warehouse op je Data Lake
- Kern is het hangen van relevante Metadata aan de data in het Data Lake
	- Zoekbaar
	- Vindbaar