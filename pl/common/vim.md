---
layout: default
title: "vim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vim">
  <a href="/pl/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vim (Vi IMproved), edytor tekstu wiersza polecenia, oferuje kilka trybów dla różnych rodzajów manipulacji tekstem.
> Naciśnięcie przycisku `i` powoduje przejście do trybu edycji. `<Esc>` wraca do normalnego trybu, który nie pozwala na zwykłe wstawianie tekstu.
> Więcej informacji: <https://www.vim.org>.

#### Otwórz plik:
```shell
vim {{sciezka/do/plik}}
```
#### Zobacz instrukcję pomocy Vim:
```shell
:help<Enter>
```
#### Zapisz plik:
```shell
:write<Enter>
```
#### Wyjdź bez zapisywania:
```shell
:quit!<Enter>
```
#### Otwórz plik pod określonym numerem wiersza:
```shell
vim +{{numer_linii}} {{sciezka/do/plik}}
```
#### Cofnij ostatnią operację:
```shell
u
```
#### Wyszukaj wzorzec w pliku (naciśnij `n`/`N` przejść do następnego/poprzedniego dopasowania):
```shell
/{{szukaj_wzorca}}<Enter>
```
#### Wykonaj podstawienie wyrażenia regularnego w całym pliku:
```shell
:%s/{{wzorzec}}/{{zastąpienie}}/g<Enter>
```
{% endraw %}