# Seznámení s typografií na webu

## Připojení stylů

Propojte HTML soubor se stylem typography.css prostřednictvím tagu ``link``.

    <link rel="stylesheet" href="…">

## Vložení externích písem

Na webu [Google fonts](https://fonts.google.com/) si vyberte vhodnou kombinaci písem (Antikva+Grotesk) – inspirace například na [Fontpair](https://fontpair.co/)

Stáhněte a rozbalte příslušné (ttf) soubory do složky assets/fonts. Je velmi vhodné stáhnout i varianty řezů – pro nadpisy tučný a normální; pro stať i kurzívní.

Vytvořte příslušné definice v souboru fonts.css

Všimněte si, že pokud použijete stejný název písma, sloučí se řezy z oddělených souborů…

    @font-face {
        font-family: 'PT Sans';
        font-style: normal;
        font-weight: 400;
        src: url("./fonts/PT_Sans-Web-Regular.ttf") format('truetype');
    }
    @font-face {
        font-family: 'PT Sans';
        font-style: normal;
        font-weight: 700;
        src: url("./fonts/PT_Sans-Web-Bold.ttf") format('truetype');
    }

## Definice písma pro nadpisy a stať

Vytvořte vlastní definice kaskády velikostí písem a řezů pro nadpisy a tag ``<p>``. 

Preferujte jednotky em.

Použijte (citlivě 😉) barvy pro písmo.

## Zvýrazňování

Pokuste se o vizuální odlišení tagů

* ``<strong>`` a ``<b>`` (strong je víc)
* ``<em>`` a ``<i>`` (nemají spolu významově nic společného)
* ``<small>`` může být méně výrazné i jinak než velikostí (rozhazuje to totiž linii řádku)
* Dejte najevo, že ``<q>`` a ``<cite>`` spolu logicky souvisí
* ``<abbr>`` udělejte míň hnusný ;-)

## Bloky pro ty, co se budou nudit

Pokuste se vizuálně formátovat bloky ``<blockquote>``, ``<address>``, ``<pre>``, ``<ul>`` tak, aby více vyniklo jejich odlišení od zbytku sazebních bloků. Použijte barvu na pozadí a cokoliv dalšího na co si troufnete…
