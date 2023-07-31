---
title: Markdown intro
---

## Introduktion

*Markdown* är ett sätt att kunna lägga in grundläggande struktur och formatering i dokument, trots att man sparar dokumentet som ren text (plain text). Ren text är det mest portabla och kompatibla sättet att lagra text. 

*Markdown* fokuserar främst på __läsbarhet__ och __enkelhet__. Det använder en minimal syntax som är enkel att lära sig och texten förblir läsbar även om man öppnar den i ett program som inte tolkar Markdown.

I nedanstående avsnitt går vi igenom steg för steg med exempel hur man formaterar text med markdownsyntax. Vi inriktar oss på användning i *Trello* men det mesta gäller generellt.

* Rubriker
* Kursiv och fet stil
* Genomstruken text
* Punktlistor
* Numrerade listor
* Citat
* Avgränsare
* Emoji
* Länkar
* Infoga bilder
* Kodavsnitt

---
## Rubriker

En rad som inleds med ```#```-tecken följt av ett mellanslag är en rubrik. Antalet ```#``` anger rubrikens nivå, vilket ger dokumentet struktur. Lämna alltid en tom rad efter rubriken.

*Exempel*

# Rubriknivå 1

## Rubriknivå 2

### Rubriknivå 3

*Syntax*

    # Rubriknivå 1

    ## Rubriknivå 2

    ### Rubriknivå 3

---
## Kursiv och fet stil

Markdown använder asterisk (```*```) eller understrykning (```_```) som indikering för emfas. 

*Exempel*

För *kursiv* stil, omge text med *enkel asterisk*.
För **fet** stil, omge text med **dubbla asterisk**.
Det fungerar _likadant_ med __understrykning__.

*Syntax*

    För *kursiv* stil, omge text med *enkel asterisk*.
    För **fet** stil, omge text med **dubbla asterisk**.
    Det fungerar _likadant_ med __understrykningstecken__.

---
## Genomstruken text

Detta funkar i bl.a. Trello, men är inte standard i alla dialekter av Markdown.

*Exempel*

För ~~genomstruken text~~, omge texten med dubbla tilde-tecken.

*Syntax*

    För ~~genomstruken text~~, omge texten med dubbla tilde-tecken.


---
## Punktlistor

*Exempel på enkel punktlista*

* Inled en rad med en asterisk och mellanslag.
+ Det går lika bra med plus-tecken.
- Det går också bra med minus-tecken.
* Lämna alltid __en tom rad före och efter listan__. 

*Syntax*

    * Inled en rad med en asterisk och mellanslag.
    + Det går lika bra med plus-tecken.
    - Det går också bra med minus-tecken.
    * Lämna alltid __en tom rad före och efter listan__. 


*Exempel på punktlista med flera nivåer*

* Detta är första huvudpunkten.
  * Detta är en underpunkt till den första.
* Detta är andra huvudpunkten.
  + Underpunkt skapas med 2 inlednande mellanslag före punkt-tecknet.
    - Skapa en nivå till med ytterligare 2 mellanslag.
* Använd helst olika punkt-tecken på varje nivå för bättre läsbarhet.

*Syntax*

    * Detta är första huvudpunkten.
      * Detta är en underpunkt till den första.
    * Detta är andra huvudpunkten.
      + Underpunkt skapas med 2 inlednande mellanslag före punkt-tecknet.
        - Skapa en nivå till med ytterligare 2 mellanslag.
    * Använd helst olika punkt-tecken på varje nivå för bättre läsbarhet.

---
## Numrerade listor

*Exempel på numrerad lista*

1. Punkt nummer ett.
2. Andra punkten.
2.1. En underpunkt. Mellanslag behövs inte här.
2.2.1. Vilken nivå hamnar den här på?
3. Tredje punkten.

*Syntax*

    1. Punkt nummer ett.
    2. Andra punkten.
    2.1. En underpunkt. Mellanslag behövs inte här.
    2.2.1. Vilken nivå hamnar den här på?
    3. Tredje punkten.

---
## Citat

*Exempel*

>Detta är ett blockcitat. Det ser man på den speciella stilen. 
Syntax är samma som i epost med ett inledande >-tecken.
Det går bra att bryta rader. En tom rad avslutar citatet.

*Syntax*

    >Detta är ett blockcitat. Det ser man på den speciella stilen. 
    Syntax är samma som i epost med ett inledande >-tecken.
    Det går bra att bryta rader. En tom rad avslutar citatet.

---
## Avgränsare

Mellan varje stycke i den här instruktionen finns det en avgränsande linje. En sådan skapar man genom att skriva 3 asterisk (```***```) eller 3 minus (```---```) på en egen rad

*Syntax*

    ---

---
## Emoji

Alla standard emoji kan infogas i text genom att skriva dess *namn* omgivet av kolon (```:```).

*Exempel*

:star: :poop: :thumbsup:

*Syntax*

    :star: :poop: :thumbsup:

---
## Länkar

Man kan skapa en klickbar länk på följande sätt. Hakparenteser ```[ ]``` omger den text som ska visas, direkt följt av vanliga parenteser ```( )``` som omger URL:en.

*Exempel*

En klickbar länk till [Daring Fireball](https://daringfireball.net/projects/markdown/syntax), som är ursprunget till Markdown.

*Syntax*

    En klickbar länk till [Daring Fireball](https://daringfireball.net/projects/markdown/syntax), som är ursprunget till Markdown.

---
## Infoga bilder

Man infogar en bild genom att ange en __länk till bildfilen__ med ett __inledande utropstecken__.

*Exempel*

![beskrivning](http://folkets-lexikon.csc.kth.se/folkets/grafik/logotype.png)

*Syntax*

    ![beskrivning](http://folkets-lexikon.csc.kth.se/folkets/grafik/logotype.png)


I Trello kan man dessutom infoga en bild som ligger som *bilaga* i Trello. Denna metod finns beskriven på ett eget kort: [Trello: Infoga bild i beskrivning](https://trello.com/c/gks1cLcR)

---
## Kodavsnitt

Ibland vill man visa text med en ```fast teckenbredd```. Det är användbart för att visa källkod, syntax eller bara skilja ut tydligt från löptext. Man kan göra detta på två sätt.

### Alternativ 1 - trippla bakåtcitat

Inled och avsluta med 3 bakåtcitattecken (\```) efter varandra. Detta fungerar både för enstaka ord i en mening eller för ett helt stycke på flera rader.

*Exempel*

I detta exempel omges ordet ```kommando``` med trippla bakåtcitattecken.

```
void example() {
    cout << "Källkod på flera rader." << endl;
}
```

*Syntax*

    I detta exempel omges ordet ```kommando``` med trippla bakåtcitattecken.

    ```
    void example() {
        cout << "Källkod på flera rader." << endl;
    }
    ```

### Alternativ 2 - inledande mellanslag

Som alternativ till trippla bakåtcitattecken kan man istället __inleda varje rad med 4 mellanslag__. Avsluta bara med en tom rad.

*Exempel*

    Exempel på text med fastteckenbredd.
    På flera rader, som alla inledes med 4 mellanslag.
    Detta används till alla syntax-exempel i den här texten.
    Avsluta med en tom rad.

*Syntax*

        Exempel på text med fastteckenbredd.
        På flera rader, som alla inledes med 4 mellanslag.
        Detta används till alla syntax-exempel i den här texten.
        Avsluta med en tom rad.

---

