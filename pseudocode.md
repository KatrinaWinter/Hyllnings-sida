##Sten, Sax, Påse

###Version 1

START
    Sätt Spelarens  poäng till 0
    Sätt Datorns  poäng till 0 
    MEDAN Spelaren poäng <3 och Datorn poäng <3 
        generera tatorns val slumpmäsigt från sten, sax eller påse
        Input minLängd från Spelaren 
        SKRIV UT Spelaren och Datorn val
        OM Spelaren och Datorn väljer samma skriv ut "oavgjort"
            ANNARS OM Spelaren väljer sten och Datorn väljer sax
                Eller Spelaren väljer sax och Datorn väljer påse
                ELLER Spelaren väljer påse och Datorn väljer sten
                SKRIV UT "Du vann rundan"
                Öka Spelaren poäng med 1
            ANNARS skriv "Datorn vann rundan"
                Öka Y poång med 1    
        Visa Ställningen "spelare: X Dator Y" 
    SLUT MEDAN
        OM spelarens poäng = 3 Skriv "Du vann spelet"
        ANNARS Skriv "Datorn vann spelet"            
SLUT

##  STEGEN

### Version 1   

START
    Sätt Spelare 1  poäng till 0
    Sätt Spelare 2  poäng till 0 
    För mål från 1 till 6 
        Spelare 1 
        GÖR 
            lägg till +1 på poäng för varje kast
            kastar tärningen
        SÅ LÄNGE kast ≠ mål → kasta igen 
        Spelare 2 
        GÖR 
            lägg till +1 på poäng för varje kast
            kastar tärningen
        SÅ LÄNGE kast ≠ mål → kasta igen 
        SKRIV UT Spelare 1: poäng = X 
        SKRIV UTSpelare 2: poäng = Y
    SLUTFÖR 
    OM Spelare1 poäng = Spelare2 poäng
        SKRIV UT "oavgjort"
    ANNARS OM Spelare1 poäng < Spelare2 poäng
        SKRIV UT "Spelare 1 vann spelet!"
    ANNARS
        SKRIV UT "Spelare 2 vann spelet!"
SLUT


## Knock out
### Version 1

START
    Input antal spelare 
    Sätt x spelares poäng till 0
    Be spelare i turordning lägga in ett knockout nr. mellan 6-9
    x spelare slutför varje runda i turårdning
        FÖR runda 1 - 10
            Spelare kastar två tärningar
            Summera tärningskastet 
            OM summan = knockout nr ges minuspoäng
                Tärningskast nr. - 10 = ny summa
                poäng = poäng + summan
            ANNARS poäng = poäng + summan
        SLUT FÖR skriv spelarns slutpoäng
    Gämför spelarns poäng   
    Spelare med > poäng vinner
    SKRIV UT "Spelare x är vinnaren!"   
SLUT

