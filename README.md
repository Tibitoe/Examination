# Examination
Repo för examination V41
Instruktioner för att öppna sidan:
1. Klona repot i VSCode.
2. Högerklicka på index.html till vänster, välj "Open with Live Server".
3. Klart!

Teknisk beskrivning:
1. Navigation:
Jag valde att använda Flex för header/navbar.
Den innehåller en h1 för och en ul med tre knappar för navigation.
Active class på respektive sida för att vilka sida man är på.
Hover effekt på knapparna.

Vid 500pixlars bredd döljs h1 och knapparna blir vertikala samt tar upp hela skärmens bredd.
Den döljs även vid skrollning men kommer tillbaks när man skrollar upp.
Detta behövde jag använda JavaScript för, inte skrivit scriptet själv utan kopierade in det.
All mobilanpassning ligger i en mediaquery.

2. Hem:
Hem-sidan gjorde jag med CSS Grid, endast en kolumn och antal rader är auto.
Hade lika gärna kunnat använda Flex här men det är responsivt och bra.
Valde att sätta en max-width på 800px och margin 0: auto för att få innehållet centrerat och inte för brett, samt för att den fina bakgrunden skulle synas.

3. Matsvampar:
Här gjorde jag ett galleri med svampar med CSS Grid.
Använde mig utav "grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));" för att smidigt kunna lägga till fler bilder.
Kolumnerna skapas automatiskt och är 300px breda och fyller på så många som får plats i containern, i det här fallet max 3 per kolumn sedan fyller den på en ny rad. Blir responsivt och bra. Minskade paddingen på containern med mediaquery på mobil
för att bättre utnyttja utrymmet.

4. Om:
Sidan innehåller bara en Article som är en Flexcontainer.

5. Footer:
Gjord med Flex.
Knappar med länk till sociala medier, öppnas i ny flik.
Justeras med mediaquery för mobil, flex-direction: column; text-align: center; så hamnar ikonerna under kontakttexten.

Tillgänglighet:
Fullt tillgänglig, lagt till aria-labels till alla länkar och alt-texter på alla bilder.
Testat sidan med Wave och hittar inga anmärkningar.
Använt h1 till h4 i korrekt ordning.
Haft kontrast i åtanke med bakgrund och text.

Webbläsarverktyg:
Har kontinuerligt använt inspektörläget (DevTools) i Firefox för att identifiera problem och göra justeringar.

Git:
Gjorde en branch av main som heter develop.
Commitat och pushat ändringar med hyfsat utförliga meddelanden allt eftersom.
När jag var klar med sidan så mergade jag den till main.