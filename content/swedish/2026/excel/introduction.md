---
title: Introduktion
weight: 20
---

## Celler

Kalkylprogram använder sig av rutnät där rutorna kallas för celler. I cellerna
skriver du in tal eller annan typ av data. En cell kan också innehålla en
beräkning som i sin tur refererar till en eller flera andra celler med data och
cellen kommer då visa resultatet av denna beräkning. 

Rutnätet delas upp i **kolumner** (anges med bokstäver) och **rader** (anges med
siffror).

[wp-siffra]: https://sv.wikipedia.org/wiki/Siffra

### Rader

Rader numreras med siffror och anger vart en cell befinner sig vertikalt. I
exemplet nedan har alla celler på rad 3 markerats.

{{< figure src="/images/2024/excel/row-3.png" title="Rad 3 i rutnätet." >}}

### Kolumner

Kolumner numreras med bokstäver och anger var en cell befinner sig horisontellt.
I exemplet nedan har alla celler i kolumn C markerats.

{{< figure 
    src="/images/2024/excel/column-c.png"
    title="Kolumn C i rutnätet."
>}}

## Referenser

För att referera till en specifik cell anges först rad direkt följd av kolumn.
På detta sätt refererar `C3` till cellen på rad `C` och kolumn `3` i rutnätet.

{{< figure 
    src="/images/2024/excel/cell-position-example.png"
    title="I rutnätet befinner sig cell C3 i kolumn C, rad 3."
>}}

## Omfång

För att beteckna ett antal närliggande celler används __omfång__ (range). Ett
omfång utgör en rektangel av celler i rutnätet. Ett omfång definieras genom att
ange cellerna i två motstående hörn i rektangeln separerade av tecknet `:`
(kolon). I exemplet nedan har omfånget `A1:C3` markerats.

{{< figure 
    src="/images/2024/excel/range-example.png" 
    title="Omfånget A1:C3."
>}}

## Starta Excel på dator i datorsal

Om du är i en av Uppsala universitets datasalar med Windows bör det finnas en
version av Excel installerad. Du kan då starta den som vanligt, efter att ha
loggat in med ditt studentkonto. Sök efter **Excel** i aktivitetsfältet (1) och
klicka på **Excel** (2).

![](/images/2025/excel/taskbar-excel.png?width=555px)

## Starta Excel i din webbläsare

Du kan även använda ett Microsoft Live-konto för att använda Excel i din
webbläsare. Notera att denna version saknar stöd för trendlinjer. Logga in här
[här](https://office.live.com/start/Excel.aspx) med ditt Microsoft Live-konto om
du vill använda Excel i din webbläsare. 

1. Logga in [här](https://office.live.com/start/Excel.aspx) med ditt Microsoft Live-konto.
2. I menyn till vänster klickar du på **skapa**. 
3. Under **Vad vill du skapa?** klickar du på **Mer...**.
4. Välj **Arbetsbok** för att skapa ett nytt kalkylark.
5. Välj **Tom arbetsbok**. 

## Tomt kalkylark

Efter att du startat Excel bör du se något liknande detta: 

{{< figure
src="/images/2024/excel/start.png" title="Excel vid start." >}}

Du kan nu börja skriva in siffror! Spara genom att klicka på **File** (Arkiv),
längst upp till vänster.

## Inmatning

Excel har många smarta funktioner för att mata in siffror effektivt. Du kan
testa detta genom att skriva några tal (*Enter* tar dig till nästa rad), markera
dessa samt klicka och dra musen neråt från det nedre högra hörnet för att skapa
en talserie baserad på de markerade talen.

{{< figure 
    src="/images/2024/excel/quicknum.gif" 
    title="Snabb inmatning av serier." 
>}}

## Formler

I Excel är **formler** ett sätt att utföra beräkningar. Du kan mata in en formel
i en cell på två olika sätt. 

Alternativ 1: 

1. Klicka på cellen där du vill mata in en formel. 
2. Klicka på \\(f_x\\)  som du hittar strax ovanför rutnätet, till vänster. 
3. Skriv sedan in din formel. 

Alternativ 2: 

1. Klicka på cellen där du vill mata in en formel. 
2. Skriv `=` följt av formeln du vill mata in. 

Klicka på en tom cell och testa att mata in formeln `3 + 5` i rutan. När du
tryckt på enter visas resultatet `8` i cellen. 

{{< figure 
    src="/images/2026/excel/3-plus-five.gif" 
    title="Beräkning av 3 + 5 med hjälp av en formel." 
>}}


## Funktioner

Förutom vanliga matematiska beräkningar (`+`, `-`, `*`, `/`) kan formler använda
sig av funktioner. En funktion i Excel beter sig på samma sätt sätt som en
matematisk funktion. En funktion tar noll eller flera **argument** (indata) och
beräknar ett **resultat** (utdata). Excel har ett stort antal inbyggda
funktioner.

Genom att använda formler och funktioner kan du enkelt och snabbt utföra
komplicerade beräkningar. 

### Manuell inmatning

För att demonstrera manuell inmatning använder vi funktionen `SUM`. Som namnet
anger beräknar denna funktion summan av ett antal värden.

Innan du fortsätter, se till att du har några värden i omfånget `A1:B11`.

{{< figure 
    src="/images/2026/excel/1-to-11.png" 
    width="400"
    title="Exempel på värden." 
>}}

För att Excel ska förstå att du vill få resultatet av en funktion i en ruta
måste du börja formeln med tecknet `=` (likhetstecken), följt av namnet på
funktionen samt eventuella argument vilka anges inom parenteser separerade med
`,` (kommatecken).

1. Klicka på cellen `A12`.
2. Skriv in formel:
    - Om du använder Excel på engelska skriver du in `=SUM(A1:B11)`.
    - Om du använder Excel på svenska skriver du in `=SUMMA(A1:B11)`.
3. Tryck på **Enter**.


{{< figure 
    src="/images/2024/excel/sum.png"
    title="Beräkna summa av alla värden i omfånget A1:B11." 
>}}

I detta exempel är alltså funktionens namn `SUM` (engelska), eller `SUMMA`
(svenska), medan argumentet är `A1:B11`. Efter att du tryckt på **Enter** visas
summan av alla tal i omfånget `A1:B11` i cellen `A12`. I detta exempel är summan
`77`.

Testa att ändra några värden i omfånget `A1:B11` och notera hur summan i rutan
`A12` automatiskt uppdateras.

{{< figure 
    src="/images/2026/excel/a1b11-sum-example.gif"
>}}


### Grafisk inmatning

Ett alternativ till manuell inmatning av funktioner är grafisk inmatning. Notera
att denna metod endast är tillgänglig i någorlunda moderna versioner av Excel.

1. Klicka först på en cell. 
2. Klicka därefter på *Insert* -> *Function*
3. Välj funktionen du vill använda
4. Markera därefter omfånget som funktionen ska appliceras på
5. Avsluta med att trycka på *Enter*.

{{< figure 
    src="/images/2024/excel/stddev.gif" 
    title="Standardavvikelse." 
>}}

### Avancerade formler

Du kan även skriva in mer komplicerade funktioner och formler.

+ Aritmetik görs med samma symboler som de flesta datorprogram, dvs `+ - * / ^`,
  där `^` används för potenser.
+ Parenteser gäller enligt reglerna för vanlig matematik.
+ Funktioner (som SUM, vilken beskrevs ovan) kan läggas in och kombineras
  godtyckligt.
+ Du kan använda celler som variabler: se följande exempel.

{{< figure 
    src="/images/2024/excel/advfunc.png"
    title="Notera att formeln syns i rutan över kalkylbladet." 
>}}

I figuren ovan har `=SUM(B1:B11) + A11 * 3 + LOG(16,2)` skrivits in i rutan C12.

Vi lägger alltså ihop summan av cellerna B1 till B11, värdet i A11 multiplicerat
med 3 och logaritmen av 16 i bas 2.

Därmed får vi resultatet av \\(11 + 11 \cdot 3 + 4\\) vilket mycket riktigt blir
48.

## Grafer

En av de viktigaste användningsområdena för kalkylark är att generera grafer.
Genom att skriva in ett antal värden (siffrorna i exemplet nedan genererade med
[random.org](https://www.random.org)) kan vi markera dessa och välja vilken
grafisk presentation (graf) vi vill ha.

{{< figure 
    src="/images/2024/excel/chart.gif" 
    title="Enklare graf." 
>}}

### Redigering

Klicka på grafen och välj *Chart*, högst upp. Du kan nu byta typ av graf och
ställa in exempelvis titel och hur etiketter representeras.

### Trendlinjer och regressionsanalys

Målet med [regressionsanalys][reg-analys] är att, utifrån observerade data,
skapa en funktion som beskriver den. Ett sätt att illustrera detta i Excel är
med hjälp av **trendlinjer**.

- En trendlinje visar tendenser på hur dina datavärden förändras (till exempel
  hur ett mätvärde förändras över tid). 
- [\\(R^2\\)-värdet][R2] (determinationskoefficienten) mäter hur väl trendlinjen
  passar till de faktiska datapunkterna och anges som ett tal mellan noll och
  ett.
  - Noll (0.0): Ingen linjär anpassning alls. Trendlinjen förklarar ingenting av
    variationen i datapunkterna. 
  - Högt värde (t.ex. över 0,8): Starkt samband och hög tillförlitlighet.
  - Lågt värde (t.ex. under 0,3): Svagt samband; spridningen på datapunkterna är
    stor i förhållande till linjen
  
[reg-analys]: https://sv.wikipedia.org/wiki/Regressionsanalys

{{% notice style="warning" title="Funkar inte i online-versionen av Excel" %}}

Trendlinjer går, i dagsläget, inte att skriva in direkt i online-versionen av
Excel. För detta krävs den nedladdade versionen.

{{% /notice %}}

När du klickat på en lämplig graf dyker verktygen **chart tools** upp i övre
raden. Klicka på **layout* för att nå alternativet **trendline**.

{{< figure 
    src="/images/2024/excel/trendline-1.PNG"
    title="Menyalternativet trendlinje syns längst upp till höger."
>}}

Valet **more options** låter dig ställa in avancerade alternativ för trendlinjer.
Det låter dig exempelvis ställa in hur trendlinjen ska beräknas, visa
[\\(R^2\\)-värdet][R2], byta format, etc. Du kan även nå detta fönster genom att
högerklicka på redan befintliga trendlinjer och välja **format trendline**.

[R2]: https://en.wikipedia.org/wiki/Coefficient_of_determination

{{< figure 
    src="/images/2024/excel/trendline-2.PNG"
    title="Inställningar för trendlinjer." >}}

Tänk på att det viktigaste med grafer är att göra de så tydliga som möjligt.
Genom att använda färger och andra inställningar kan du förtydliga linjerna och
deras förhållande till datan de representerar.

{{< figure 
    src="/images/2024/excel/trendline-3.PNG"
    title="Exempel på trendlinjer." >}}

Trendlinjer går även att skapa med andra typer av grafer.

{{< figure 
    src="/images/2024/excel/chart-alt.PNG"
    title="Exempel på formatering." 
>}}

I exemplet ovan är \\(R^2\\)-värdet mycket lågt (0.0533). Eftersom
exempelfiguren använder slumpmässiga tal är det låga värdet rimligt.
