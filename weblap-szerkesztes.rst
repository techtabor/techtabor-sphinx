A weblap szerkesztése
==========================================

Telepítés első alkalommal
-------------------------

Ezt a dokumentációt a Sphinx nevű programmal generáljuk. Maga a forráskód Danka Miki szerverén él. Ahhoz tehát, hogy szerkeszteni tudd a dokumentációt, két dologra van szükséged: a sphinxre, és hozzáférésre a forráskódhoz.

Az alábbi intstrukciók Unix alapú rendszerekre vonatkoznak (Linuxra és Macre). Windowson a legegyszerűbben úgy követheted ugyanezt, ha letöltöd a GitBash nevű programot - de azzal is valószínűleg néhány problémába fogsz ütközni.

Sphinx
~~~~~~

A Sphinxet csak akkor kell telepítened, ha a saját gépeden is szeretnéd tudni generálni a dokumentációt. Ha csak szerkeszteni szeretnéd, akkor nincs rá szükséged: a szerver maga legenerálja azt.

#. Telepítsd a `Sphinx programot <http://sphinx-doc.org/latest/install.html>`_
#. Telepítsd a `Sphinx stílust <https://github.com/snide/sphinx_rtd_theme>`_

Forráskód
~~~~~~~~~

A forrás `a Githubon <https://github.com/techtabor/techtabor-sphinx>`_ található. Kérj hozzáférést a repositoryhoz.

Szerkesztés és feltöltés
------------------------

Generálás
~~~~~~~~~
A lokális dokumentáció-generáláshoz:

1. Futtasd: ``make html``
2. Az eredmény a következő mappában lesz elérhető: ``_build/html/index.html``

Feltöltés
~~~~~~~~~

Amikor a ``git commit`` paranccsal elmentesz valamit, majd a ``git push`` paranccsal feltöltöd azt, a Netlify automatikusan legenerálja és publikálja a weboldalt.

A weboldal a `techtabor.miklosdanka.com <https://techtabor.miklosdanka.com>`_ oldalon érhető el ezen szöveg írásakor (2018-09-24).

