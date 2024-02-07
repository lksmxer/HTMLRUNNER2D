Ez egy egyszerű HTML játék, ahol egy dinoszaurusz karakter ugrál át akadályokon. A játékot a szóköz billentyű vagy egy gombkattintás vezérli. A játék akkor ér véget, amikor a dinoszaurusz összeütközik egy akadállyal. Minden játék után egy kérdést tesznek fel, és ha a válasz helyes, a pontszám egyel nő. Ha a válasz helytelen, a pontszám nullára csökken. A legmagasabb pontszámot a böngésző helyi tárolójában tárolják.


Bagyarázat a JavaScript kódhoz:

A dino, obstacle és scoreElement a dinoszaurusz, akadály és pontszám megjelenítő elemekre utalnak.

Az onkeyup eseményfigyelő a testen aktiválja az jump funkciót, amikor a szóköz (key code 32) lenyomva van.

Az jump funkció hozzáad egy "jump" osztályt a dinoszauruszhoz, ami elindít egy CSS animációt, amelynek hatására a dinoszaurusz úgy tűnik, mintha ugrana. 600 millimásodperc után az "jump" osztályt eltávolítják.

A resetGame funkció visszaállítja a játékot úgy, hogy leállítja az akadály animációját, véletlenszerűen beállítja a magasságát, és beállít egy ütközésdetektáló intervallumot, amely minden 10 millimásodpercben ellenőrzi, hogy a dinoszaurusz és az akadály összeütköznek-e.

A gameOver funkció leállítja az akadály animációját, törli az ütközésdetektáló intervallumot, és véletlenszerűen feltesz egy kérdést egy előre meghatározott listáról. Ha a válasz helyes, a pontszám egyel nő és a játék visszaáll. Ha a válasz helytelen, a pontszám nullára csökken és a játék visszaáll.

A játék a resetGame funkció hívásával indul.

Készítette:
  Simák Balázs és
  Erdővölgyi Bendegúz
