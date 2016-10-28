Git
==========================================


Kód hozzáadása a Slack Techbothoz
---------------------------------

#. Töltsd le és telepíts egy git klienst, pl.: `<https://git-for-windows.github.io/>`_
#. Nyisd meg a git klienst, és navigálj egy mappába, ahova majd a projektet letöltjük
#. Nyisd meg a repot: `<https://github.com/techtabor/techbot>`_
#. Nyomd meg a fork gombot. Ez generál egy másolatot a repositoryról a saját accountodra. Nevezzük ezt techbot-copy reponak
#. A techbot-copy repoban kattints a Clone gombra - ekkor előjön egy link: ezt másold ki
#. A git kliensben töltsd le a repositoryt: ``git clone <a másolt link>``
#. Menj bele a mappába: ``cd techbot``
#. Csinálj egy új branchet: ``git checkout -b feature/<branch neve>``
#. Most írd át azt a kódrészletet, amit szeretnél
#. Ha új fájlt készítettél, trackeld az új fájlt: ``git add .``
#. Mentsd el a kódot: ``git commit``
#. Töltsd fel a kódot: ``git push origin feature/<branch neve>``
#. Most csinálunk egy pull requestet az eredeti repoba. Nyisd meg a techbot repot, majd kattints a “new pull request” gombra
#. Jelöld ki a saját repodnak az új branchét
#. Submit pull request
#. Add hozzá Ildit és további mentorokat a code reviewhoz
#. Ezek után a mentorok kommentálják a kódot, majd végül elfogadják azt - ha ez megtörtént, a kódrészleted a fő repository részévé válik

