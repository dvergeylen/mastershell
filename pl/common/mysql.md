---
layout: default
title: "mysql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysql">
  <a href="/pl/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie wiersza polecenia MySQL.
> Więcej informacji: <https://www.mysql.com/>.

#### Połącz z bazą danych:
```shell
mysql {{nazwa_bazydanych}}
```
#### Połącz się z bazą danych, użytkownik zostanie poproszony o podanie hasła:
```shell
mysql -u {{uzytkownik}} --password {{nazwa_bazydanych}}
```
#### Połącz się z bazą danych na innym hoście:
```shell
mysql -h {{host_bazydanych}} {{nazwa_bazydanych}}
```
#### Połącz się z bazą danych przez gniazdo Unix:
```shell
mysql --socket {{sciezka/do/socket.sock}}
```
#### Wykonuj instrukcje SQL w pliku skryptu (plik wsadowy):
```shell
mysql -e "source {{nazwapliku.sql}}" {{nazwa_bazydanych}}
```
#### Przywróć bazę danych z kopii zapasowej (użytkownik zostanie poproszony o podanie hasła):
```shell
mysql --user {{uzytkownik}} --password {{nazwa_bazydanych}} < {{sciezka/do/backup.sql}}
```
#### Przywróć wszystkie bazy danych z kopii zapasowej (użytkownik zostanie poproszony o podanie hasła):
```shell
mysql --user {{uzytkownik}} --password < {{sciezka/do/backup.sql}}
```
{% endraw %}