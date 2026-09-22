# Antworten zu Git

## Was ist der Unterschied zwischen Working Directory, Staging Area und Repository?

- **Working Directory:** Hier arbeitest du an deinen Dateien und nimmst Änderungen vor.
- **Staging Area:** Ein Zwischenbereich, in dem festgelegt wird, welche Änderungen in den nächsten Commit übernommen werden sollen.
- **Repository:** Die Git-Datenbank, in der alle Commits und die Versionshistorie gespeichert werden.

## Woran erkennst du, ob ein Merge Fast-Forward war?

Ein Fast-Forward-Merge erzeugt keinen neuen Merge-Commit. Stattdessen wird der Branch-Zeiger einfach auf den neuesten Commit des anderen Branches verschoben. Git zeigt beim Merge oft die Meldung „Fast-forward“ an.

## Warum kann `git merge --ff-only` manchmal fehlschlagen?

Der Befehl schlägt fehl, wenn ein Fast-Forward-Merge nicht möglich ist. Das passiert beispielsweise, wenn auf beiden Branches unterschiedliche Commits erstellt wurden und daher ein echter Merge erforderlich wäre.

## Was ist der Vorteil, Änderungen zuerst auf einem Branch wie `dev` zu machen?

Änderungen können getestet und geprüft werden, ohne den Hauptbranch (`main`) zu beeinflussen. Dadurch bleibt die stabile Version des Projekts erhalten und Fehler können frühzeitig erkannt werden.

## Mit welchem Befehl siehst du den aktuellen Branch?

```bash
git branch
