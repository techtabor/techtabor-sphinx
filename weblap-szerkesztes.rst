A weblap szerkesztése
==========================================

Telepítés első alkalommal
-------------------------

Ezt a dokumentációt a Sphinx nevű programmal generáljuk. Maga a forráskód Danka Miki szerverén él. Ahhoz tehát, hogy szerkeszteni tudd a dokumentációt, két dologra van szükséged: a sphinxre, és hozzáférésre a forráskódhoz.

Az alábbi intstrukciók Unix alapú rendszerekre vonatkoznak (Linuxra és Macre). Windowson a legegyszerűbben úgy követheted ugyanezt, ha letöltöd a GitBash nevű programot - de azzal is valószínűleg néhány problémába fogsz ütközni.

Sphinx
~~~~~~

A Sphinxet csak akkor kell telepítened, ha a saját gépeden is szeretnéd tudni generálni a dokumentációt. Ha csak szerkeszteni szeretnéd, akkor nincs rá szükséged: a szerver maga legenerálja azt.

#. Telepítsd a Sphinx programot: `link <http://sphinx-doc.org/latest/install.html>`_
#. Telepítsd a Sphinx stílust: `link <https://github.com/snide/sphinx_rtd_theme>`_

Forráskód
~~~~~~~~~

#. Ha nincs még pubic keyed a ``~/.ssh`` mappában, akkor generálj egyet az ``ssh-keygen -t rsa`` utasítással. (Bővebben `itt <https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2>`_ olvashatsz róla)
#. Küldd el a public keyed (``<valami>.pub``) Danka Mikinek, és várd meg amíg válaszol
#. A ``.ssh/config`` fájlba írd be a következő részt::

    Host miki-git
      User git
      Hostname 5.101.107.150
      Port 22022
      IdentityFile ~/.ssh/<a te private key fajlod>

#. Ezek után letöltheted a repositoryt: ``git clone miki-git:techtabor``

Szerkesztés és feltöltés
------------------------

Generálás
~~~~~~~~~
A lokális dokumentáció-generáláshoz:

1. Futtasd: ``make html``
2. Az eredmény a következő mappában lesz elérhető: ``_build/html/index.html``

Feltöltés
~~~~~~~~~

Amikor a ``git commit`` paranccsal elmentesz valamit, majd a ``git push`` paranccsal feltöltöd azt, egy "git hook" automatikusan legenerálja és publikálja a weboldalt.

A weboldal a `www.miklosdanka.com/techtabor <http://www.miklosdanka.com/techtabor>`_ oldalon érhető el ezen szöveg írásakor (2016-09-03).

