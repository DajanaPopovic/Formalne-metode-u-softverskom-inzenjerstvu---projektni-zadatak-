# Klasifikacija Covertype skupa podataka pomoću neuronskih mreža

Ovaj projekat predstavlja rješenje za **Projektni zadatak br. 2** u okviru predmeta *Formalne metode u softverskom inženjerstvu*. Cilj zadatka je treniranje i 
optimizacija arhitekture vještačke neuronske mreže nad Covertype skupom podataka.



Formalne metode u softverskom inženjerstvu– Projektni zadatak br. 2:


(50%) Istrenirati neuronsku mrežu nad Covertype skupom podataka. Potrebno je definisati
proizvoljnu arhitekturu neuronske mreže. Obratiti pažnju na broj ulaznih i izlaznih neurona u
prvom i posljednjem sloju neuornske mreže. Koristiti adekvatnu funkciju greške. Trenirati
neuronsku mežu proizvoljan broj epoha sa proizvoljnom veličinom batch-a. Pronaći
preciznost i odziv nad testnim skupom podataka prije i poslije treninga.

(25%) Definisati validacioni skup podataka. Implementirati early stopping u toku treninga
tako da se trening prekine kada greška nad validacionim skupom počne da raste. Tolerisati 2
epohe rasta greške, a nakon toga prekinuti trening ukoliko se greška poveća i u trećoj
uzastopnoj epohi.

(25%) Pretražiti prostor hiperparametara. Potrebno je varirati bar 2 vrijednosti počtenog
faktora obučavavanja. Pored faktora obučavanja proizvoljno odabrati bar još dva prametra
koji utiču na arhitekturu mreže i varirati date parametre sa bar 2 vrijednosti. Odabrati model
koji daje najbolju preciznost na validacionom skupu. Napomena: Ukoliko samo
implementirate ovu tačku bez prethodne, trenirati sve mreže isti broj epoha.


## Opis zadatka i implementacija

Projekat je podijeljen u tri ključne cjeline:
1. **Treniranje neuronske mreže (50%):** Definisana je prilagođena arhitektura mreže, određen adekvatan broj ulaznih i izlaznih neurona, te izračunata preciznost (*precision*) i odziv (*recall*) nad testnim skupom prije i poslije treninga.
2. **Early Stopping mehanizam (25%):** Implementirana je logika za rani prekid treninga. Ukoliko greška na validacionom skupu raste tri uzastopne epohe (tolerancija od 2 epohe), trening se automatski obustavlja kako bi se spriječilo preprilagođavanje (*overfitting*).
3. **Pretraga hiperparametara (25%):** Izvršeno je variranje početnog faktora obučavanja (*learning rate*), kao i još dva strukturna parametra arhitekture (npr. broj skrivenih slojeva i veličina batch-a). Odabran je model sa najboljom preciznošću na validacionom skupu.

## Korištene biblioteke i instalacija

Projekat je implementiran u jeziku Python unutar Jupyter Notebook okruženja. Korištene su sljedeće biblioteke:
numpy, scikit-learn, tensorflow

Da biste pokrenuli projekat lokalno, instalirajte potrebne zavisnosti:

```bash
pip install -r requirements.txt
```

