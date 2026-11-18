# Salón Jasmín · design notes

Demo pre jasmin.esticode.sk. Metóda: refero-design, výskum ručne (bez Refero MCP), cez voľne dostupné styles.refero.design a weby salónov.
Dátum: 18. 11. 2026.

## Brief

Navrhujem jednostránkový web pre susedské kaderníctvo v Košiciach (Dargovských hrdinov) pre zákazníčky z okolia, primárne na iPhone.
Cieľ: zavolať a objednať sa, nájsť cestu, vidieť hodiny.
Tón: pokojný, upravený, ako ich interiér (drevené lamely, antracitové steny).
Riziko: generický "beauty" vzhľad zameniteľný s inými salónmi, a to, že Merci demo je tiež kaderníctvo.
Zapamätateľný prvok: obrovský názov ako hlavný vizuál a posuvník pred a po nad ich vlastnými fotkami z Facebooku.
Obmedzenia: jeden statický index.html, iba overené fakty, bez cien, bez mien recenzentov a citátov.

## Referencie

| # | Web | URL | Čo z neho beriem |
|---|-----|-----|------------------|
| 1 | Face Formula (Refero Styles) | https://styles.refero.design/style/78ac71e1-cd4c-4b4d-bac5-e7e6c65cd3fa | Primárny smer. Kondenzovaný serif ako masthead s názvom značky, takmer achromatická paleta, 1px linky namiesto kariet, 0 radius, drobné popisky v kapitálkach s 0.2em rozostupom, fotky nesú všetko teplo. |
| 2 | Iad-lab (Refero Styles) | https://styles.refero.design/style/7d66c966-6cee-4c82-b2e4-2bf1ca7b2ccd | Iba binárne tmavé pásy (bone na charcoal) pre úvod, hodiny a kontakt, s tenkými svetlými deliacimi linkami. |
| 3 | Serenity Hair Salon, Blaxland (Awwwards Nominee) | https://serenityhairblaxland.com.au/ · https://www.awwwards.com/sites/serenity-hair-salon-blaxland | Iba mobilný postup: tlačidlo objednania hneď pod úvodom, služby po kategóriách. Pastelové škvrny a script písmo zamietnuté. |

Pozorované, nepoužité: Il Colorista Salon (https://www.awwwards.com/sites/il-colorista-salon), WebGL, v prehliadači sa nevykreslil.

## Reference lock

- Primárny: Face Formula.
- Zachovať: obrovský serif wordmark, 1px linky, 0 radius, kapitálkové popisky, žiadne tiene ani gradienty na UI.
- Požičať: tmavé pásy z Iad-lab; poradie CTA zo Serenity.
- Odmietnuté: krémové plátno, olivová a terakota, italic zvýraznenie slov, karty s tieňom, pastelové blob tvary.

## Decision ledger

| Rozhodnutie | Zdroj | Rola | Prečo |
|---|---|---|---|
| Instrument Serif 400 na nadpisy | Face Formula (Libre Caslon Condensed) | iba display | kondenzovaný serif, latin-ext pre slovenčinu, iný ako Merci (EB Garamond) |
| Manrope 400 až 600 na UI | Face Formula (Circular, náhrada Manrope) | celé UI | neutrálny sans; 600 iba v tlačidlách kvôli čitateľnosti CTA |
| Charcoal #2B2E32 | farba stien v ich salóne (FB fotka interiéru) | text, tmavé pásy, tlačidlo | web vyzerá ako ich priestor |
| Dub #B07D4F | drevené lamely v ich salóne | iba dekor: lamelový pás, hviezdy, demo pruh, štítok "dnes" | nikdy ako plocha s textom tela |
| Mist #F1F2F3 | Face Formula Mist | pás cenníka, box hodnotenia | povrch bez tieňa |
| Plné tlačidlo "Objednať sa" | Serenity (poradie), brief | hlavné CTA | Face Formula má ghost linky, ale tu je cieľ telefonát |
| Spodná lišta s volaním na mobile | brief (iPhone, konverzia) | iba mobil, skrytá pri úvode a kontakte | CTA vždy na dosah palca |
| Posuvník pred a po | ich FB fotky sú koláže pred a po | obsah | pravdivý dôkaz kvality bez vymyslených citátov |

## Fotky

Všetky z https://www.facebook.com/p/Salón-Jasmín-100066542241533 (sekcia Fotky, verejne viditeľné bez prihlásenia).
Jedna koláž vyradená, lebo v pozadí bol rozpoznateľný iný človek.

## Neoverené

Otváracie hodiny podľa oma.sk. Cenník ukážkový, bez cien.
