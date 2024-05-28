
Einfache Mergekonflikte auf GitHub, die beim Zusammenfügen von Branges über Pull request entstehen, können mit dem Konflikteditor im Browser behoben werden.

[https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)

Alle anderen Mergekonflikte sind lokal in der Befehlszeile mit Hilfe eines Editors (z.B. Visual Studio Code) zu beheben.

[https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line)

Die Konfliktstellen werden in den betroffenen Dateien mit Konfliktmarker `<<<<<<<` etc. gekennzeichnet, z.B.

```
If you have questions, please
<<<<<<< HEAD
open an issue
=======
ask your question in IRC.
>>>>>>> branch-a
```

Die Konfliktmarker <<<<<<<, ======= und >>>>>>> sind zu löschen und die gewünschten Änderungen in den Merge zu übernehmen, z.B.:

```
If you have questions, please open an issue or ask in our IRC channel if it's more urgent.
```

Weiter wie üblich:
+ git add .
+ git commit -m "Resolve merge conflict by incorporating both suggestions"
