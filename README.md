# Joc Spânzurătoarea (Hangman) - CLI în C

Un joc clasic de tip "Spânzurătoarea" dezvoltat în limbajul C, care utilizează o interfață în consolă bazată pe manipularea unei matrice de caractere pentru randarea grafică.

## Caracteristici Principale
* **Randare Grafică Dinamică:** Utilizează o matrice 2D de 40x40 pentru a desena progresiv elementele spânzurătorii și ale personajului (cap, corp, membre) în funcție de numărul de greșeli.
* **Sistem de Bază de Date Externă:** Extrage cuvinte dintr-un fișier extern ("text.txt") folosind un algoritm de selecție pseudo-aleatorie bazat pe "rand()" și "time()".
* **Motor de Joc Inteligent:**
    * Gestionează compararea caracterelor și elimină distincția între litere mari și mici (case-insensitivity).
    * Actualizează în timp real masca cuvântului ghicit.
    * Limitează numărul de încercări la 7 etape vizuale.

## Detalii Tehnice
* **Limbaj:** C.
* **Concepte utilizate:**
    * **Manipularea Matricelor:** Definirea de constante pentru coordonatele geometrice ale desenului în consolă.
    * **I/O de fișiere:** Utilizarea "fopen" și "fgets" pentru citirea dintr-o bază de date de cuvinte.
    * **Logică Algoritmică:** Gestionarea stării jocului printr-o buclă "while" și verificări condiționate pentru victoria sau înfrângerea jucătorului.

## Geometria Desenului
Proiectul folosește constante predefinite pentru a asigura proporțiile personajului:
* "dimensiune_matrice": 40
* "body_height": 9
* "picior_height": 10
* "gat_height": 6

## Cum se joacă
1. Asigurați-vă că aveți un fișier numit "text.txt" pe Desktop (sau modificați calea în cod la linia "fopen").
2. Compilați codul.
3. Introduceți litere pentru a ghici cuvântul mascat.
