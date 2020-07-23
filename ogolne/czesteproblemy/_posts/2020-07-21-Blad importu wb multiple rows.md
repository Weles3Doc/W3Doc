---
title: Błąd importu WB multiple rows
---
# Błąd importu WB multiple rows

Jeśli przy imporcie wyciągów zwykłych/elektronicznych wystąpi błąd, którego treści będzie opis "MULTIPLE ROWS IN SINGLE SELECT", oznacza to, że wyszczególnione konto bankowe, którego dotyczy przypisane, jest do kilku kontrahentów (zamiast tylko jednego) i w wyniku niejednoznaczności, nie można zaksięgować transakcji.

Należy wtedy skopiować nr rachunku i przejść do edycji kontrahentów: zakładka Zasoby > menu Zasoby > Edytuj kontrahentów.

Klawiszami [CTRL+F] włączamy wyszukiwarkę i wklejamy skopiowane konto w formacie ze spacjami, aby je wyszukać.

Spośród wyszukanych pozycji, edytujemy i usuwamy je ze zbędnych kontrahentów, zapisujemy i ponawiamy import wyciągu.

![Błąd importu WB multiple rows](impwbmultiplerows.gif)