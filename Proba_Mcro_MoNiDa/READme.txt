Salutări bine v-am găsit, aici și READme0ul promis.

Pentru acest program am creat 3 fișiere diferite:

- index.html - punctul de start al programului și așezarea elementelor în pagină
- style.css - stilizarea elementelor alese pentru aplicație
- joc.js - partea de logică din spatele programului

1. joc.js

- în acest fișier am început cu myfunc(), o funcție care determină statusul jocului: dacă a câștigat vreun jucător sau este remiză. 
Această funcție este apelată de fiecare dată când este apăsată (completată) o căsuță nouă. Avem 9 variabile diferite (b1-b9) pentru căsuțe, cu
ajutorul cărora verificăm fiecare variantă posibilă de câștig pentru ambii jucători. În cazul în care avem o variantă de câștig
sau remiză, va fi afișat un mesaj corespunzător iar restul căsuțelor vor fi dezactivate până la resetarea jocului.
În cazul în care nu s-au completat căsuțele încă, le spunem jucătorilor să continue jocul.

- urmează cele 9 funcții corespunzătoare celor 9 căsuțe (casuta_N ()), care verifică ce valoare ar trebui să aibă căsuța, în funție de variabila flag.
Această variabilă ține evidența jucătorilor, dacă este rândul jucătorului X sau 0. După completare, căsuța rămâne 
dezactivată, și schimbăm rândul jucătorilor.

- într-un final, avem și funcția de reset a jocului - reset_game(), care este apelată odată cu apăsarea butonului de reset. Căsuțele își resetează 
valorile și sunt active din nou.

2. html.index

- în acest fișier am amplasat elementele aplicației: titlu, subtitluri, instrucțiuni, matricea 3x3, și butonul de reset.

- pentru fiecare căsuță N, va fi apelată funția corespunzatoare ei: cauta_N() și myfunc() pentru verificarea statusului.

- de asemenea, pentru butonul de reset vom apela functia reset_game().

3. style.css 

- am creat mai multe stiluri, în funcție de elementele pe care le avem în aplicație.

- avem h1, h2, și h3 pentru headerele de text

- avem #b1-#b9 pentru căsuțe

- #but pentru butonul de reset

- #print și #ins pentru textele de instrucțiuni și rândul jucătorului

- #main - pentru backgroundul aplicației



