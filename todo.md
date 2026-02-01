zrób skill do obslugi https://api.serpdata.io/
przykładowy request to

curl --request GET \
	--url 'https://api.serpdata.io/v1/search?keyword=pomoc+drogowa+Krakow&hl=pl&gl=pl' \
	--header 'Authorization: Bearer nodeshub_1cf9b3291f87e7a06e98bbb95902c3a0-TLltoqELg9I'

forma odpowiedzi to:

{
  "data": {
    "search_engine": "google",
    "location": "pl",
    "language": "pl",
    "timestamp": "2026-02-01T08:18:23.096157Z",
    "search_url": null,
    "total_results_count": null,
    "results": {
      "query": "pomoc drogowa Krakow",
      "snippets": {
        "ads": [],
        "answer_box": [],
        "local_pack": [
          {
            "more_places_url": null,
            "places": [
              {
                "name": "Pomoc drogowa Kraków | Laweta | Holowanie Inspect Car Robert Krzyżek",
                "rank_inner": 1,
                "url": "https://autopomoc-krakow.pl/"
              },
              {
                "name": "Pomoc Drogowa Kraków Damian Frąc",
                "rank_inner": 2,
                "url": "https://pomoc-drogowakrakow.pl/"
              },
              {
                "name": "Laweta 24 Kraków",
                "rank_inner": 3,
                "url": "https://www.laweta24krakow.pl/"
              }
            ],
            "rank_absolute": 1,
            "title": "Local results"
          },
          {
            "more_places_url": null,
            "places": [
              {
                "name": "Euro Hol",
                "rank_inner": 4,
                "url": "https://eurohol.pl/"
              },
              {
                "name": "Pomoc Drogowa Jasek-Hol | Laweta | Holowanie | Kraków | Wieliczka",
                "rank_inner": 5,
                "url": "https://jasekhol.pl/"
              },
              {
                "name": "Pomoc Drogowa24H Laweta",
                "rank_inner": 6,
                "url": "http://www.hienka.com.pl/"
              }
            ],
            "rank_absolute": 4,
            "title": "Local results"
          }
        ],
        "people_also_ask": {
          "questions": [
            {
              "expanded": false,
              "rank_inner": 1,
              "text": "Ile kosztuje 1 km pomocy drogowej?"
            },
            {
              "expanded": false,
              "rank_inner": 2,
              "text": "Ile kosztuje laweta w Krakowie?"
            },
            {
              "expanded": false,
              "rank_inner": 3,
              "text": "Kiedy laweta jest za darmo?"
            },
            {
              "expanded": false,
              "rank_inner": 4,
              "text": "Czy laweta liczy kilometry w obie strony?"
            }
          ],
          "rank_absolute": 5
        },
        "perspectives": [],
        "related_searches": {
          "queries": [
            "Pomoc Drogowa Kraków 24h",
            "Pomoc drogowa - Kraków OLX",
            "Laweta Kraków",
            "Pomoc drogowa a4 kraków",
            "Pomoc drogowa Balice",
            "Holowanie Kraków",
            "Pomoc drogowa Wieliczka",
            "Pomoc drogowa Nowa Huta"
          ],
          "rank_absolute": 14
        }
      },
      "organic_results": [
        {
          "pos": 1,
          "global_pos": 2,
          "url": "https://krakhol.pl/",
          "domain": "krakhol.pl",
          "title": "Pomoc Drogowa Kraków | Krakhol",
          "description": "Pod numerem telefonu 536 536 789 otrzymasz fachową pomoc. Po upływie 15-20 minut od przyjęcia zgłoszenia nasz profesjonalista z odpowiednim sprzętem udzieli ...",
          "page": 1,
          "pos_internal": 1
        },
        {
          "pos": 2,
          "global_pos": 3,
          "url": "https://eurohol.pl/",
          "domain": "eurohol.pl",
          "title": "Euro Hol: Pomoc drogowa i holowanie 24h - Kraków",
          "description": "Potrzebna pomoc drogowa w Krakowie lub okolicy? Dzwoń 24h na 501323031. Oferujemy TANIE, profesjonalne holowanie pojazdów osobowych, dostawczych i TIR.",
          "page": 1,
          "pos_internal": 2
        },
        {
          "pos": 3,
          "global_pos": 6,
          "url": "https://autopomoc-krakow.pl/",
          "domain": "autopomoc-krakow.pl",
          "title": "Pomoc drogowa Kraków | Całodobowa Auto Pomoc",
          "description": "Całodobowa pomoc drogowa w Krakowie i okolicach * 607 996 268 - Szybki Dojazd w 20 min * Pomoc na autostrada A4 + Laweta Kraków oraz holowanie.",
          "page": 1,
          "pos_internal": 3
        },
        {
          "pos": 4,
          "global_pos": 7,
          "url": "https://www.pomoc-drogowakrakow.pl/",
          "domain": "www.pomoc-drogowakrakow.pl",
          "title": "Całodobowa Auto Pomoc Drogowa Kraków | Damian Frąc",
          "description": "Pomoc drogowa świadcząca usługi na terenie Krakowa i okolic. Szybka i skuteczna pomoc w przypadku awarii, wypadku lub zablokowania pojazdu.",
          "page": 1,
          "pos_internal": 4
        },
        {
          "pos": 5,
          "global_pos": 8,
          "url": "http://www.autopapiez.pl/",
          "domain": "www.autopapiez.pl",
          "title": "Pomoc Drogowa Kraków Podgórze - Auto Papież - pomoc ...",
          "description": "- pomoc drogowa 24h (za holowanie samochodu w granicach miasta Krakowa pobieramy opłatę zryczałtowaną, niezależnie od ilości kilometrów);. - powypadkowe naprawy ...",
          "page": 1,
          "pos_internal": 5
        },
        {
          "pos": 6,
          "global_pos": 9,
          "url": "https://www.facebook.com/Pomoc.Drogowa.Krakow.1/?locale=pl_PL",
          "domain": "www.facebook.com",
          "title": "Pomoc Drogowa Kraków, Sprint-Car",
          "description": "Kontakt: 514-190-999 E-mail: biuro@sprint-car24.com Nie trać czasu ani pieniędzy! Z nami szybko i bez stresu wrócisz do normalnego funkcjonowania. Twoje ...",
          "page": 1,
          "pos_internal": 6
        },
        {
          "pos": 7,
          "global_pos": 10,
          "url": "https://krakow-pomoc-drogowa.pl/",
          "domain": "krakow-pomoc-drogowa.pl",
          "title": "Pomoc Drogowa Kraków – Kraków i Okolice. Zadzwoń!",
          "description": "Działamy 24/7, zapewniając szybki czas reakcji i pełne wsparcie w każdej sytuacji. Holowanie pojazdów ciężarowych – awaria, kolizja, czy problem techniczny?",
          "page": 1,
          "pos_internal": 7
        },
        {
          "pos": 8,
          "global_pos": 11,
          "url": "https://ampomoc.pl/",
          "domain": "ampomoc.pl",
          "title": "Auto Pomoc Drogowa Kraków 24h - Całodobowy Mechanik",
          "description": "ZADZWOŃ 600 600 452 - WYJAZD DO 15 MIN! Cennik naszych usług. Usługa, Przykładowa cena. Załadunek i transport pojazdu osobowego na terenie Krakowa, 200-300 zł.",
          "page": 1,
          "pos_internal": 8
        },
        {
          "pos": 9,
          "global_pos": 12,
          "url": "https://popekhol.pl/",
          "domain": "popekhol.pl",
          "title": "POPEK HOL | Pomoc drogowa Kraków",
          "description": "Oferujemy szeroki zakres usług, w tym holowanie, złomowanie pojazdów, awaryjne odpalanie, naprawy powypadkowe i mechaniczne, wyciąganie pojazdów spoza drogi i ...",
          "page": 1,
          "pos_internal": 9
        },
        {
          "pos": 10,
          "global_pos": 13,
          "url": "https://pomocdrogowacentrum.pl/",
          "domain": "pomocdrogowacentrum.pl",
          "title": "Usługi pomocy drogowej - Pomoc drogowa Kraków - 574 112 ...",
          "description": "Przewóz uszkodzonych pojazdów✓, holowanie✓, transport maszyn✓, motocykli✓. Dowóz paliwa, drobne naprawy mechaniczne. Uruchomienie w przypadku utraty ...",
          "page": 1,
          "pos_internal": 10
        }
      ],
      "snippets_found": [
        "people_also_ask",
        "related_searches",
        "local_pack"
      ],
      "request": {
        "url": "https://www.google.com/search?q=pomoc drogowa Krakow&gl=pl&hl=pl&uule=w+CAIQICIGUG9sYW5k&pws=0&safe=disabled&num=10&nfpr=1",
        "final_url": "",
        "device": "desktop",
        "crawl_datetime": "2026-02-01T08:18:22",
        "http_code": 200
      },
      "success": true
    },
    "success": true
  },
  "totalResponseTime": 6258
}

Instrukcja jak budować skile: https://github.com/anthropics/skills

W wynikach chce otrzymać top 10 wyników z "organic_results"