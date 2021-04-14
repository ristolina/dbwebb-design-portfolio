---
Title: Laddningstid
Description: This is our load times page.
---
Laddningstid av hemsidor inom betalbranschen
=======================

Denna rapport är en analys av hastigheten på hemsidor inom betalbranschen. Analysen innebär både en teknisk analys av färgschema samt en subjektiv bedömning av färgerna och upplevelsen de förmedlar.

Urval
-----------------------

Jag har valt tre olika hemsidor för företag verksamma inom kortbetalningsbranschen. Anledningen till att jag valt den branschen är att jag själv arbetar inom samma bransch.

Metod
-----------------------
Jag har använt både [Google Pagespeed](https://developers.google.com/speed/pagespeed/insights) och Firefox Developer Tools för att utvärdera hastigheten på hemsidorna.

Resultat
-----------------------

Data för mätningarna finns [här](https://docs.google.com/spreadsheets/d/1gMml0anmxsHhgE7dv-hi4ZxWVKGhVhTKbvUAvCD0guQ/edit?usp=sharing).

## Hemsida 1 - [Bambora](www.bambora.com)
![Bambora](%base_url%/image/Bambora.png){.snapshot}
<table>
<tr>
<th>Laddninstid</th>
<th>Antal Requests</th>
<th>Storlek</th>
<th>Pagespeed Mobile</th>
<th>Pagespeed Desktop</th>
<tr>
<td>1.44</td>
<td>60</td>
<td>2.12</td>
<td>36</td>
<td>81</td>
</tr>
</table>
### Sammanfattning
Hemsidan för Desktop laddas relativt snabbt. Det finns såklart lite förbättringar som kan göras, till exemepel att snabba upp den initiala svarstiden på webbservern och optimera laddningen av det största content-elementet (bilden).
För mobilsidan så är det främst 'Time to interactive' som behöver förbättras eftersom det tar nästan 10 sekunder innan man kan använda sidan.


## Hemsida 2 - [Nets](www.nets.eu)
![Nets](%base_url%/image/Nets.png){.snapshot}
<table>
<tr>
<th>Laddninstid</th>
<th>Antal Requests</th>
<th>Storlek</th>
<th>Pagespeed Mobile</th>
<th>Pagespeed Desktop</th>
<tr>
<td>2.32</td>
<td>109</td>
<td>9.72</td>
<td>2</td>
<td>34</td>
</tr>
</table>
### Sammanfattning
Hemsidan känns ganska långsam vid första laddning. Enligt pagespeed så finns det flera punkter att förbättra. På Desktop-sidan är det främst utritningen av sidan och 'Time to interactive' som är de största hastighetsbovarna.
Samma gäller för mobilsidan men då är det 'Time to interactive' som tar längst tid, nästan 30 sekunder.

## Hemsida 3 - [Verifone](https://www.verifone.com)
![Verifone](%base_url%/image/Verifone.png){.snapshot}
<table>
<tr>
<th>Laddninstid</th>
<th>Antal Requests</th>
<th>Storlek</th>
<th>Pagespeed Mobile</th>
<th>Pagespeed Desktop</th>
<tr>
<td>3.12</td>
<td>31</td>
<td>2.11</td>
<td>63</td>
<td>91</td>
</tr>
</table>
### Sammanfattning
Hemsidan känns snabb vid första laddning och enligt pagespeed finns det inte så mycket att förbättra. På Desktop-sidan är det i princip bara tiden för det största elementen/bilden som behöver snabbas upp. För mobilsidan så är det förutom sammas som desktopsidan även 'Time to interactive' som behöver förbättras.

Analys
-----------------------
Gemensamt för samtliga sidor är att utritningen av det största element kan förbättras. Jag ser även 'Time to interactive' som en viktigt punkt för användarupplevelsen.

Andra gemensamma förbättringspunkter är att den initiala svarstiden på webbservern kan förbättras samt att ta bort resurser som blockerar renderingen av sidan.
Samtliga sidor har även javascript som inte används och därför kan tas bort.

Rangordning av sidorna:
1. Verifone
2. Bambora
3. Nets

Verifone känns helt klart som att den laddar den viktga informationen snabbast. Men Bambora kommer på en stark andraplats. I pagespeeds betyg skiljer det en del mellan Verifone och Bambora men när jag går in på sidorna så tycker jag inte någon av dem känns långsam.

Den totala laddningstiden tycker jag borde hålla sig under 2 sekunder för att det ska kännas snabbt. Enligt snittvärdena på mina mätningar så är det bara Bambora som klarar 2 sekunders-gränsen. Men det absolut viktigaste tycker jag är att sidan går att använda snabbt och att de element som tar lång tid att ladda in inte stör sidan (t.ex. att den hoppar och rycker).

Övrigt
-----------------------

Författare: Kristoffer Pettersson
