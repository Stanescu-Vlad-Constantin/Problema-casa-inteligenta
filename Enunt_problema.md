# Problema-casa-inteligenta
In proiectarea unei case inteligente e nevoie de un soft pentru management energetic si obtinerea a diferite statistici ale dispozitivelor din casa.
Cerinţa
Avand acces la o lista cu aparatele instalate, se doreste procesarea acesteia in functie de comanda primita ulterior.

Date de intrare
Pe prima linie citita de la tastatura (stream-ul stdin) se află un numar n, numarul de aparate instalate. Pe urmatoarele n linii se afla aparatele in formatul:

nume_aparat categorie_aparat camera_montaj consum_energetic

nume_aparat - este un nume format dintr-un singur cuvânt (fără whitespaces) de maxim 50 de caractere. Se garanteaza ca numele aparatului este unic. (ex: LG837dds, bec_phillips_E27)

categorie_aparat este o secvență de caractere fără whitespace care descrie tipul de aparat, de maxim 50 de caractere. (ex: frigider, bec, masina_spalat)

camera_montaj este un sir de caractere de maxim 50 caracter ce reprezinta camera in care e instalat aparatul respectiv. (ex: bucatarie, sufragerie)

consum_energetic numar intreg pe 16b ce reprezinta consumul in watti al aparatului.



Se citeste apoi un sir de caractere ce reprezinta cerinta dorita. Cerintele pot fi: "nr_categorii" "best_room", "sort_consum", "consum_total_timp","consum_max_timp".

In cazul cerintelor "consum_total_timp" si "consum_max_timp" se vor citi tot din stream-ul stdin linii pana la caracterul EOF. Aceste linii vor avea formatul:

nume_aparat nr_ore_pornit

nume_aparat - numele aparatului care se porneste. Sir de maxim 50 de caracter

nr_ore_pornit - numarul de ore cat aparatul a stat pornit. Numar intreg pe 16b.

Toate liniile se termină cu newline, mai puțin ultima, care se termină cu EOF.

Subiectul 1 - 6p
Daca cerinta dorita este "nr_categorii" se va afisa numarul de categorii de aparate diferite instalate.

Subiectul 2 - 6p
Daca cerinta dorita este "best_room" se va afisa numele camerei cu cele mai multe dispozitive. In caz de egalitate, se afiseaza prima alfabetic.

Subiectul 3 - 6p
Daca cerinta dorita este "sort_consum" se vor afisa toate aparatele sortate crescator dupa consum si in cazul consumului egal, alfabetic dupa numele aparatului.

Subiectul 4 - 6p
Daca cerinta dorita este "consum_total_timp" se vor citit orele cat au stat aparatele pornite si apoi se va afisa numarul de Watt-ora consumati.

Subiectul 5 – 6p
Daca cerinta dorita este "consum_max_timp" se vor citit orele cat au stat aparatele pornite si apoi se va afisa care aparat a consumat cel mai mult in total.

