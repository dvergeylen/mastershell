---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#7z">7z</a>
* <a href="#7za">7za</a>
* <a href="#7zr">7zr</a>
* <a href="#ack">ack</a>
* <a href="#adb">adb</a>
* <a href="#adb-install">adb install</a>
* <a href="#adb-reverse">adb reverse</a>
* <a href="#adb-shell">adb shell</a>
* <a href="#ag">ag</a>
* <a href="#arp">arp</a>
* <a href="#astronomer">astronomer</a>
* <a href="#at">at</a>
* <a href="#atom">atom</a>
* <a href="#atq">atq</a>
* <a href="#atrm">atrm</a>
* <a href="#autoflake">autoflake</a>
* <a href="#awk">awk</a>
* <a href="#aws">aws</a>
* <a href="#babel">babel</a>
* <a href="#base32">base32</a>
* <a href="#base64">base64</a>
* <a href="#batch">batch</a>
* <a href="#bitcoin-cli">bitcoin-cli</a>
* <a href="#csslint">csslint</a>
* <a href="#diff">diff</a>
* <a href="#docker-images">docker images</a>
* <a href="#dotnet">dotnet</a>
* <a href="#eslint">eslint</a>
* <a href="#http">http</a>
* <a href="#java">java</a>
* <a href="#mysql">mysql</a>
* <a href="#pathchk">pathchk</a>
* <a href="#pdfimages">pdfimages</a>
* <a href="#pdftk">pdftk</a>
* <a href="#php">php</a>
* <a href="#python">python</a>
* <a href="#r">r</a>
* <a href="#rar">rar</a>
* <a href="#rm">rm</a>
* <a href="#sass">sass</a>
* <a href="#sudo">sudo</a>
* <a href="#tldr">tldr</a>
* <a href="#vim">vim</a>
* <a href="#vue">vue</a>
* <a href="#xkcdpass">xkcdpass</a>
* <a href="#xkill">xkill</a>
* <a href="#youtube-dl">youtube-dl</a>

{% raw %}
<h2 id="7z">
  <a href="/pl/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator plików o wysokim stopniu kompresji.
> Więcej informacji: <https://www.7-zip.org/>.

#### Zarchiwizuj plik lub katalog:
```shell
7z a {{zarchiwizowane.7z}} {{sciezka/do/pliku_lub_katalogu}}
```
#### Zaszyfruj istniejące archiwum (w tym nagłówki)):
```shell
7z a {{zaszyfrowane.7z}} -p{{haslo}} -mhe=on {{zarchiwizowane.7z}}
```
#### Wyodrębnij istniejący plik 7z z oryginalną strukturą katalogów:
```shell
7z x {{zarchiwizowane.7z}}
```
#### Wyodrębnij archiwum ze ścieżką wyjściową zdefiniowaną przez użytkownika:
```shell
7z x {{zarchiwizowane.7z}} -o{{sciezka/do/wyjscia}}
```
#### Wypakuj archiwum do stdout:
```shell
7z x {{zarchiwizowane.7z}} -so
```
#### Archiwizuj przy użyciu określonego typu archiwum:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{zarchiwizowane.7z}} {{sciezka/do/pliku_lub_katalogu}}
```
#### Wyświetl dostępne typy archiwów:
```shell
7z i
```
#### Wyświetl zawartość pliku archiwum:
```shell
7z l {{zarchiwizowane.7z}}
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/pl/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator plików o wysokim współczynniku kompresji.
> Samodzielna wersja `7z` z obsługą mniejszej liczby typów archiwów.
> Więcej informacji: <https://www.7-zip.org/>.

#### Zarchiwizuj plik lub katalog:
```shell
7za a {{archiwum.7z}} {{scieżka/do/pliku_lub_katalogu}}
```
#### Wyodrębnij istniejący plik 7z z oryginalną strukturą katalogów:
```shell
7za x {{archiwum}}
```
#### Zarchiwizuj przy użyciu określonego typu archiwum:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{archiwum}} {{scieżka/do/pliku_lub_katalogu}}
```
#### Wypisz dostępe typy archiwów:
```shell
7za i
```
#### Wypisz zawartość pliku archiwum:
```shell
7za l {{archiwum}}
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/pl/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator plików o wysokim współczynniku kompresji.
> Samodzielna wersja `7z` obsługująca tylko pliki typu .7z.
> Więcej informacji: <https://www.7-zip.org/>.

#### Zarchiwizuj plik lub katalog:
```shell
7zr a {{archiwum.7z}} {{scieżka/do/pliku_lub_katalogu}}
```
#### Wyodrębnij istniejący plik 7z z oryginalną strukturą katalogów:
```shell
7zr x {{archiwum.7z}}
```
#### Wypisz zawartość pliku archiwum:
```shell
7zr l {{archiwum.7z}}
```
{% endraw %}{% raw %}
<h2 id="ack">
  <a href="/pl/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie wyszukiwania, takie jak grep, zoptymalizowane dla programistów.
> Więcej informacji: <https://beyondgrep.com/documentation/>.

#### Znajdź pliki zawierające „foo”:
```shell
ack {{foo}}
```
#### Znajdź pliki określonego typu:
```shell
ack --ruby {{foo}}
```
#### Policz całkowitą liczbę dopasowań dla terminu „foo”:
```shell
ack -ch {{foo}}
```
#### Pokaż nazwy plików zawierające „foo” i liczbę dopasowań w każdym pliku:
```shell
ack -cl {{foo}}
```
#### Przeszukaj plik pod kątem określonego ciągu znaków:
```shell
ack bar "{{foo bar}}" {{scieżka/do/pliku_lub_katalogu}}
```
#### Przeszukaj plik pod kątem określonego wzorca wyrażenia regularnego:
```shell
ack bar "{{[bB]ar \d+}}" {{scieżka/do/pliku_lub_katalogu}}
```
#### Wypisz wszystkie prawidłowe typy:
```shell
ack --help-types
```
{% endraw %}{% raw %}
<h2 id="adb-install">
  <a href="/pl/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: wysyłaj pakiety do instancji emulatora Androida lub podłączonych urządzeń z systemem Android.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Wyślij aplikację na Androida do emulatora / urządzenia:
```shell
adb install {{scieżka/do/pliku.apk}}
```
#### Zainstaluj ponownie istniejącą aplikację, zachowując jej dane:
```shell
adb install -r {{scieżka/do/pliku.apk}}
```
#### Przyznaj wszystkie uprawnienia wymienione w pliku manifestu aplikacji:
```shell
adb install -g {{scieżka/do/pliku.apk}}
```
#### Szybko zaktualizuj zainstalowany pakiet, aktualizując tylko te części APK, które się zmieniły:
```shell
adb install --fastdeploy {{scieżka/do/pliku.apk}}
```
{% endraw %}{% raw %}
<h2 id="adb-reverse">
  <a href="/pl/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: zwrotne połączenie socketowe z emulowanego lub prawdziwego urządzenia Android.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Listuj wszystkie zwrotne połączenia socketowe z emulatorów i urządzeń:
```shell
adb reverse --list
```
#### Przekieruj port TCP z emulatora lub urządzenia do localhost:
```shell
adb reverse tcp:{{remote_port}} tcp:{{local_port}}
```
#### Usuń wybrane zwrotne połączenie z emulatora lub urządzenia:
```shell
adb reverse --remove tcp:{{remote_port}}
```
#### Usuń wszystkie zwrotne połączenie z emulatorów lub urządzeń:
```shell
adb reverse --remove-all
```
{% endraw %}{% raw %}
<h2 id="adb-shell">
  <a href="/pl/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: uruchamiaj zdalne polecenia powłoki na instancji emulatora Androida lub podłączonych urządzeniach z Androidem.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Uruchom interaktywną zdalną powłokę na emulatorze / urządzeniu:
```shell
adb shell
```
#### Pobierz wszystkie właściwości z emulatora lub urządzenia:
```shell
adb shell getprop
```
#### Przywróć wszystkie uprawnienia wykonawcze do ich wartości domyślnych:
```shell
adb shell pm reset-permissions
```
#### Odwołaj niebezpieczne pozwolenie dla aplikacji:
```shell
adb shell pm revoke {{paczka}} {{pozwolenie}}
```
#### Wywołaj zdarzenie klawisza:
```shell
adb shell input keyevent {{kod_klucza}}
```
#### Wyczyść dane aplikacji na emulatorze lub urządzeniu:
```shell
adb shell pm clear {{paczka}}
```
#### Rozpocznij aktywność na emulatorze / urządzeniu:
```shell
adb shell am start -n {{paczka}}/{{aktywność}}
```
#### Rozpocznij aktywność domową na emulatorze lub urządzeniu:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}{% raw %}
<h2 id="adb">
  <a href="/pl/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: komunikuj się z instancją emulatora Androida lub podłączonym urządzeniem z Androidem.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Sprawdź czy proces serwera adb działa, jeśli nie, uruchom go:
```shell
adb start-server
```
#### Zakończ proces serwera adb:
```shell
adb kill-server
```
#### Uruchom powłokę w instancji emulatora lub urządzeniu:
```shell
adb shell
```
#### Wypchnij aplikację Androidową do instancji emulatora lub urządzenia:
```shell
adb install -r {{ścieżka/do/pliku.apk}}
```
#### Skopiuj plik/katalog do urządzenia:
```shell
adb pull {{ścieżka/do/pliku_lub_katalogu_na_urządzeniu}} {{ścieżka/do/lokalnego_katalogu}}
```
#### Skopiuj plik/katalog z urządzenia:
```shell
adb push {{ścieżka/do/pliku_lub_katalogu_na_urządzeniu}} {{ścieżka/do/lokalnego_katalogu}}
```
#### Listuj połączone lub emulowane urządzenia:
```shell
adb devices
```
{% endraw %}{% raw %}
<h2 id="ag">
  <a href="/pl/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. Podobny do ack, ale ma być szybszy.
> Więcej informacji: <https://github.com/ggreer/the_silver_searcher>.

#### Znajdź pliki zawierające „foo” i wypisz dopasowane linie:
```shell
ag {{foo}}
```
#### Znajdź pliki zawierające „foo” w określonym katalogu:
```shell
ag {{foo}} {{scieżka/do/katalogu}}
```
#### Znajdź pliki zawierające „foo”, ale podaj tylko nazwy plików:
```shell
ag -l {{foo}}
```
#### Znajdź pliki zawierające „FOO” bez rozróżniania wielkości liter i wypisz tylko dopasowanie, a nie całą linię:
```shell
ag -i -o {{FOO}}
```
#### Znajdź „foo” w plikach o nazwie pasującej do „bar”:
```shell
ag {{foo}} -G {{bar}}
```
#### Znajdź pliki, których zawartość pasuje do wyrażenia regularnego:
```shell
ag '{{^ba(r|z)$}}'
```
#### Znajdź pliki o nazwie pasującej do „foo”:
```shell
ag -g {{foo}}
```
{% endraw %}{% raw %}
<h2 id="arp">
  <a href="/pl/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pokaż i manipuluj pamięcią podręczną ARP systemu.
> Więcej informacji: <https://manned.org/arp>.

#### Pokaż bieżącą tabelę arp:
```shell
arp -a
```
#### Wyczyść całość cache:
```shell
sudo arp -a -d
```
#### Usuń konkretny wpis:
```shell
arp -d {{adres}}
```
#### Utwórz wpis:
```shell
arp -s {{adres}} {{adres_mac}}
```
{% endraw %}{% raw %}
<h2 id="astronomer">
  <a href="/pl/common/astronomer.html">astronomer</a> <a href="#astronomer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie wykrywające nielegalne gwiazdki z kont botów w projektach GithHub.
> Więcej informacji: <https://github.com/Ullaakut/astronomer>.

#### Skanuj repozytorium:
```shell
astronomer {{tldr-pages/tldr-node-client}}
```
#### Zeskanuj maksymalną liczbę gwiazdek w repozytorium:
```shell
astronomer {{tldr-pages/tldr-node-client}} --stars {{50}}
```
#### Przeskanuj repozytorium, w tym raporty porównawcze:
```shell
astronomer {{tldr-pages/tldr-node-client}} --verbose
```
{% endraw %}{% raw %}
<h2 id="at">
  <a href="/pl/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wykonuje polecenia o zadanym czasie.
> Aby działać poprawnie wymaga działającego serwisu atd (lub atrun).
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Wykonaj za 5 minut polecenie wprowadzone przy użyciu wejścia standardowego (aby zakończyć naciśnij `Ctrl + D`):
```shell
at now + 5 minutes
```
#### Wykonaj o 10:00 rano polecenie podane z wejścia standardowego:
```shell
echo "{{./zrób_backup.sh}}" | at 1000
```
#### Wykonaj polecenia z podanego pliku w najbliższy wtorek o 21:30:
```shell
at -f {{ścieżka/do/pliku}} 9:30 PM Tue
```
{% endraw %}{% raw %}
<h2 id="atom">
  <a href="/pl/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wieloplatformowy edytor tekstu z obsługą wtyczek.
> Wtyczkami zarządza się poprzez `apm`.
> Więcej informacji: <https://atom.io/>.

#### Otwórz plik lub katalog:
```shell
atom {{sciezka/do/pliku_lub_katalogu}}
```
#### Otwórz plik lub katalog w nowym oknie:
```shell
atom -n {{sciezka/do/pliku_lub_katalogu}}
```
#### Otwórz plik lub katalog w istniejącym oknie:
```shell
atom --add {{sciezka/do/pliku_lub_katalogu}}
```
#### Otwórz Atom w trybie bezpiecznym (nie ładuje żadnych dodatkowych pakietów):
```shell
atom --safe
```
#### Zapobiega rozwidlaniu się w tle, utrzymuje Atom podłączony do terminala:
```shell
atom --foreground
```
#### Poczekaj na zamknięcie okna Atom przed powrotem (przydatne dla Git commit editor):
```shell
atom --wait
```
{% endraw %}{% raw %}
<h2 id="atq">
  <a href="/pl/common/atq.html">atq</a> <a href="#atq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pokaż oczekujące zadania użytkownika wprowadzone wcześniej przez polecenia `at` lub `batch`.
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Pokaż zaplanowane zadania:
```shell
atq
```
#### Pokaż zadania z kolejki oznaczonej 'a' (kolejki mają jednoznakowe identyfikatory):
```shell
atq -q {{a}}
```
#### Pokaż zadania wszystkich użytkowników (uruchom jako superużytkownik):
```shell
sudo atq
```
{% endraw %}{% raw %}
<h2 id="atrm">
  <a href="/pl/common/atrm.html">atrm</a> <a href="#atrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Usuwa zadania o zadanych identyfikatorach (numerach) wcześniej zakolejkowane przez `at` lub `batch`
> Aby znaleźć numery zadań, użyj `atq`.
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Usuń zadanie numer 10:
```shell
atrm {{10}}
```
#### Usuń kilka zadań, oddzielonych spacjami:
```shell
atrm {{15}} {{17}} {{22}}
```
{% endraw %}{% raw %}
<h2 id="autoflake">
  <a href="/pl/common/autoflake.html">autoflake</a> <a href="#autoflake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie do usuwania nieużywanych importów i zmiennych z kodu Python.
> Więcej informacji: <https://github.com/myint/autoflake>.

#### Usuń nieużywane zmienne z jednego pliku i wyświetl różnicę:
```shell
autoflake --remove-unused-variables {{file.py}}
```
#### Usuń nieużywane importy z wielu plików i wyświetl różnice:
```shell
autoflake --remove-all-unused-imports {{file1.py}} {{file2.py}} {{file3.py}}
```
#### Usuń nieużywane zmienne z pliku, zastępując plik:
```shell
autoflake --remove-unused-variables --in-place {{file.py}}
```
#### Usuń nieużywane zmienne rekurencyjnie ze wszystkich plików w katalogu, nadpisując każdy plik:
```shell
autoflake --remove-unused-variables --in-place --recursive {{sciezka/do/katalogu}}
```
{% endraw %}{% raw %}
<h2 id="awk">
  <a href="/pl/common/awk.html">awk</a> <a href="#awk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wszechstronny język programowania do pracy na plikach.
> Więcej informacji: <https://github.com/onetrueawk/awk>.

#### Wydrukuj piątą kolumnę (aka. pole) w pliku oddzielonym spacjami:
```shell
awk '{print $5}' {{nazwapliku}}
```
#### Wydrukuj drugą kolumnę wierszy zawierających "something" w pliku oddzielonym spacjami:
```shell
awk '/{{coś}}/ {print $2}' {{nazwapliku}}
```
#### Wydrukuj ostatnią kolumnę każdego wiersza w pliku, używając przecinka (zamiast spacji) jako separatora pola:
```shell
awk -F ',' '{print $NF}' {{nazwapliku}}
```
#### Zsumuj wartości w pierwszej kolumnie pliku i wydrukuj sumę:
```shell
awk '{s+=$1} END {print s}' {{nazwapliku}}
```
#### Zsumuj wartości w pierwszej kolumnie i wydrukuj wartości, a następnie sumę:
```shell
awk '{s+=$1; print $1} END {print "--------"; print s}' {{nazwapliku}}
```
#### Drukuj co trzeci wiersz, zaczynając od pierwszego wiersza:
```shell
awk 'NR%3==1' {{nazwapliku}}
```
#### Wydrukuj wszystkie wartości, zaczynając od trzeciej kolumny:
```shell
awk '{for (i=3; i <= NF; i++) printf $i""FS; print""}' {{nazwapliku}}
```
#### Wydrukuj różne wartości w zależności od warunków:
```shell
awk '{if ($1 == "foo") print "Dokładne dopasowanie foo"; else if ($1 ~ "bar") print "Częściowe dopasowanie bar"; else print "Baz"}' {{nazwapliku}}
```
{% endraw %}{% raw %}
<h2 id="aws">
  <a href="/pl/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Oficjalne narzędzie CLI dla Amazon Web Services.
> Wizard, SSO, Resource Autocompletion, i opcje YAML są tylko v2.
> Więcej informacji: <https://aws.amazon.com/cli>.

#### Konfiguruj AWS Command-line:
```shell
aws configure wizard
```
#### Konfiguruj AWS Command-line używając SSO:
```shell
aws configure sso
```
#### Zobacz tekst pomocy dla polecenia AWS:
```shell
aws {{komenda}} help
```
#### Uzyskaj tożsamość wywołującego (służy do rozwiązywania problemów z uprawnieniami):
```shell
aws sts get-caller-identity
```
#### Wyświetla listę zasobów AWS w regionie i wyświetla w yaml:
```shell
aws dynamodb list-tables --region {{us-east-1}} --output yaml
```
#### Użyj auto prompt do pomocy z poleceniem:
```shell
aws iam create-user --cli-auto-prompt
```
#### Uzyskaj interaktywnego kreatora dla zasobu AWS:
```shell
aws dynamodb wizard {{nowa_tabela}}
```
#### Generuj JSON CLI Skeleton (przydatne dla infrastruktury jako kodu):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}{% raw %}
<h2 id="babel">
  <a href="/pl/common/babel.html">babel</a> <a href="#babel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transpiler, który konwertuje kod ze składni JavaScript ES6 / ES7 na składnię ES5.
> Więcej informacji: <https://babeljs.io/>.

#### Transpiluj określony plik wejściowy i dane wyjściowe do stdout:
```shell
babel {{siezka/do/pliku}}
```
#### Transpiluj określony plik wejściowy i wyjście do określonego pliku:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --out-file {{sciezka/do/pliku_wyjsciowego}}
```
#### Transpiluj plik wejściowy przy każdej zmianie:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --watch
```
#### Transpiluj cały katalog plików:
```shell
babel {{sciezka/do/katalogu_wejsciowego}}
```
#### Zignoruj określone pliki oddzielone przecinkami w katalogu:
```shell
babel {{sciezka/do/katalogu_wejsciowego}} --ignore {{ignorowane_pliki}}
```
#### Transpiluj i wypisz jako zminimalizowany JavaScript:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --minified
```
#### Wybierz zestaw ustawień dla formatowania wyjściowego:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --presets {{presets}}
```
#### Wyświetl wszystkie dostępne opcje:
```shell
babel --help
```
{% endraw %}{% raw %}
<h2 id="base32">
  <a href="/pl/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enkoduj lub dekoduj plik lub standardowe wejście do/z Base32, na standardowe wyjście.
> Więcej informacji: <https://www.gnu.org/software/coreutils/base32>.

#### Enkoduj plik:
```shell
base32 {{nazwapliku}}
```
#### Dekoduj plik:
```shell
base32 --decode {{nazwapliku}}
```
#### Enkoduj z stdin:
```shell
{{jakiespolecenie}} | base32
```
#### Dekoduj z stdin:
```shell
{{jakiespolecenie}} | base32 --decode
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/pl/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enkoduj lub dekoduj plik lub standardowe wejście do/z Base64, na standardowe wyjście.
> Więcej informacji: <https://www.gnu.org/software/coreutils/base64>.

#### Enkoduj plik:
```shell
base64 {{nazwapliku}}
```
#### Dekoduj plik:
```shell
base64 --decode {{nazwapliku}}
```
#### Enkoduj z stdin:
```shell
{{jakiespolecenie}} | base64
```
#### Dekoduj z stdin:
```shell
{{jakiespolecenie}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="batch">
  <a href="/pl/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wykonaj polecenia, gdy pozwoli na to poziom obciążenia systmu.
> Aby działać poprawnie wymaga działającego serwisu atd (lub atrun).
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Wykonaj polecenie wprowadzone przy użyciu wejścia standardowego (aby zakończyć naciśnij `Ctrl + D`):
```shell
batch
```
#### Wykonaj polecenie podane z wejścia standardowego:
```shell
echo "{{./zrób_backup.sh}}" | batch
```
#### Wykonaj polecenia z podanego pliku:
```shell
batch -f {{ścieżka/do/pliku}}
```
{% endraw %}{% raw %}
<h2 id="bitcoin-cli">
  <a href="/pl/common/bitcoin-cli.html">bitcoin-cli</a> <a href="#bitcoin-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Klient konsolowy do interakcji z demonem Bitcoina poprzez zapytania RPC.
> Używa konfiguracji zdefiniowanej w `bitcoin.conf`.
> Więcej informacji: <https://en.bitcoin.it/wiki/Running_Bitcoin#Command-line_arguments>.

#### Wyślij transakcję na dany adres:
```shell
bitcoin-cli sendtoaddress "{{adres}}" {{ilość}}
```
#### Wygeneruj jeden lub więcej bloków:
```shell
bitcoin-cli generate {{ilość_bloków}}
```
#### Wyświetl informacje o portfelu:
```shell
bitcoin-cli getwalletinfo
```
#### Wyświetl wszystkie poprzednie transakcje dostępne do opłacenia transakcji wychodzących:
```shell
bitcoin-cli listunspent
```
#### Wyeksportuj dane portfela do pliku tekstowego:
```shell
bitcoin-cli dumpwallet "{{ścieżka/do/pliku}}"
```
{% endraw %}{% raw %}
<h2 id="csslint">
  <a href="/pl/common/csslint.html">csslint</a> <a href="#csslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Linter dla kodu CSS.
> Więcej informacji: <https://github.com/CSSLint/csslint/wiki/Command-line-interface>.

#### Lintowanie pojedynczego pliku CSS:
```shell
csslint {{plik.css}}
```
#### Lintowanie wiele plików CSS:
```shell
csslint {{plik1.css}} {{plik2.css}} {{plik3.css}}
```
#### Wymień wszystkie możliwe reguły stylu:
```shell
csslint --list-rules
```
#### Określ pewne reguły jako błędy (które powodują niezerowy kod wyjścia):
```shell
csslint --errors={{bledy,universal-selector,imports}} {{plik.css}}
```
#### Określ pewne reguły jako ostrzeżenia:
```shell
csslint --warnings={{box-sizing,selector-max,floats}} {{plik.css}}
```
#### Określ pewne reguły, które będą całkowicie ignorowane:
```shell
csslint --ignore={{ids,rules-count,shorthand}} {{plik.css}}
```
{% endraw %}{% raw %}
<h2 id="diff">
  <a href="/pl/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Porównaj pliki i foldery.

#### Porównaj pliki (lista zmian między `stary_plik` a `nowy_plik`):
```shell
diff {{stary_plik}} {{nowy_plik}}
```
#### Porównaj pliki, ignoruj białe znaki (white spaces):
```shell
diff -w {{stary_plik}} {{nowy_plik}}
```
#### Porównaj pliki, pokaż różnice obok siebie:
```shell
diff -y {{stary_plik}} {{nowy_plik}}
```
#### Porównaj pliki, pokaż różnice w ujednoliconym formacie (tak jak w przypadku `git diff`):
```shell
diff -u {{stary_plik}} {{nowy_plik}}
```
#### Porównaj foldery rekurencyjnie (pokazuje nazwy różniących się plików/folderów a także zmiany w plikach):
```shell
diff -r {{stary_folder}} {{nowy_folder}}
```
#### Porównaj foldery rekurencyjnie, pokaż tylko nazwy plików które się różnią:
```shell
diff -rq {{stary_folder}} {{nowy_folder}}
```
{% endraw %}{% raw %}
<h2 id="docker-images">
  <a href="/pl/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zarządzaj obrazami Dockera.
> Więcej informacji: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Wyświetl wszystkie obrazy Docker:
```shell
docker images
```
#### Wyświetl wszystkie obrazy Dockera, w tym intermediates:
```shell
docker images -a
```
#### Wyświetl dane wyjściowe w trybie quiet (tylko identyfikatory numeryczne):
```shell
docker images -q
```
#### Wyświetl wszystkie obrazy Docker nieużywane przez żaden kontener:
```shell
docker images --filter dangling=true
```
{% endraw %}{% raw %}
<h2 id="dotnet">
  <a href="/pl/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wieloplatformowe narzędzia wiersza polecenia .NET dla platformy .NET Core.
> Więcej informacji: <https://docs.microsoft.com/dotnet/core/tools>.

#### Zainicjuj nowy projekt .NET:
```shell
dotnet new {{szablon_krotka_nazwa}}
```
#### Przywróć pakiety nuget:
```shell
dotnet restore
```
#### Zbuduj i uruchom projekt .NET w bieżącym katalogu:
```shell
dotnet run
```
#### Uruchom pakietową aplikację dotnet (wymaga tylko środowiska wykonawczego, pozostałe polecenia wymagają zainstalowanego zestawu .NET Core SDK):
```shell
dotnet {{sciezka/do/aplikacji.dll}}
```
{% endraw %}{% raw %}
<h2 id="eslint">
  <a href="/pl/common/eslint.html">eslint</a> <a href="#eslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Podłączane narzędzie lintowania dla JavaScript i JSX.
> Więcej informacji: <https://eslint.org>.

#### Stwórz eslint config:
```shell
eslint --init
```
#### Lint na danym zestawie plików:
```shell
eslint {{nazwapliku}}.js {{nazwapliku1}}.js
```
#### Napraw lint issues:
```shell
eslint --fix
```
#### Lint z config:
```shell
eslint -c {{sciezka/do/pliku_config}} {{app/src}}
```
{% endraw %}{% raw %}
<h2 id="http">
  <a href="/pl/common/http.html">http</a> <a href="#http"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> HTTPie: HTTP client, ma być łatwiejszy w użyciu niż cURL.
> Więcej informacji: <https://httpie.org>.

#### Pobierz adres URL do pliku:
```shell
http --download {{przyklad.org}}
```
#### Wyślij dane zakodowane w formularzu:
```shell
http --form {{przyklad.org}} {{nazwa='bob'}} {{zdjecie_profilowe@'bob.png'}}
```
#### Wyślij obiekt JSON:
```shell
http {{przyklad.org}} {{name='bob'}}
```
#### Określ metodę HTTP:
```shell
http {{HEAD}} {{przyklad.org}}
```
#### Dołącz dodatkowy nagłówek:
```shell
http {{przyklad.org}} {{X-MyHeader:123}}
```
#### Podaj nazwę użytkownika i hasło do uwierzytelnienia serwera:
```shell
http --auth {{nazwauzytkownika:haslo}} {{przyklad.org}}
```
#### Określ surowe ciało żądania za pośrednictwem stdin:
```shell
cat {{dane.txt}} | http PUT {{przyklad.org}}
```
{% endraw %}{% raw %}
<h2 id="java">
  <a href="/pl/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Application Launcher.
> Więcej informacji: <https://java.com>.

#### Uruchom plik .class java, który zawiera główną metodę, używając tylko nazwy klasy:
```shell
java {{nazwaklasy}}
```
#### Uruchom program .jar:
```shell
java -jar {{nazwapliku.jar}}
```
#### Wyświetl wersje JDK, JRE i HotSpot:
```shell
java -version
```
#### Wyświetl informacje o użyciu polecenia java:
```shell
java -help
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="pathchk">
  <a href="/pl/common/pathchk.html">pathchk</a> <a href="#pathchk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sprawdź poprawność oraz przenośność jednej lub większej ilości ścieżek.
> Więcej informacji: <https://www.gnu.org/software/coreutils/pathchk>.

#### Sprawdź ścieżki pod kątem poprawności w obecnym systemie:
```shell
pathchk {{ścieżka1 ścieżka2 …}}
```
#### Sprawdź ścieżki pod kątem poprawności w szerszym zakresie systemów zgodnych z POSIX:
```shell
pathchk -p {{ścieżka1 ścieżka2 …}}
```
#### Sprawdź ścieżki pod kątem poprawności we wszystkich systemach zgodnych z POSIX:
```shell
pathchk --portability {{ścieżka1 ścieżka2 …}}
```
#### Sprawdź tylko pod kątem pustych ścieżek lub wiodących myślników (-):
```shell
pathchk -P {{ścieżka1 ścieżka2 …}}
```
{% endraw %}{% raw %}
<h2 id="pdfimages">
  <a href="/pl/common/pdfimages.html">pdfimages</a> <a href="#pdfimages"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie do wyodrębniania obrazów z plików PDF.

#### Wyodrębnij wszystkie obrazy z pliku PDF i zapisz je jako pliki PNG:
```shell
pdfimages -png {{ścieżka/do/pliku.pdf}} {{przedrostek_nazwy_pliku}}
```
#### Wyodrębnij obrazy ze stron 3 do 5:
```shell
pdfimages -f {{3}} -l {{5}} {{ścieżka/do/pliku.pdf}} {{przedrostek_nazwy_pliku}}
```
#### Wyodrębnij obrazy z pliku PDF oraz zawrzyj numer strony w nazwach wyjściowych:
```shell
pdfimages -p {{ścieżka/do/pliku.pdf}} {{przedrostek_nazwy_pliku}}
```
#### Wyświetl listę informacji o każdym obrazie w pliku PDF:
```shell
pdfimages -list {{ścieżka/do/pliku.pdf}}
```
{% endraw %}{% raw %}
<h2 id="pdftk">
  <a href="/pl/common/pdftk.html">pdftk</a> <a href="#pdftk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zestaw narzędzi PDF.
> Więcej informacji: <https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit>.

#### Wyodrębnij strony 1-3, 5 i 6-10 z pliku PDF oraz zapisz je jako inny plik PDF:
```shell
pdftk {{plik_wejściowy.pdf}} cat {{1-3 5 6-10}} output {{plik_wyjściowy.pdf}}
```
#### Połącz listę plików PDF i zapisz połączony plik jako:
```shell
pdftk {{plik1.pdf plik2.pdf ...}} cat output {{plik_wyjściowy.pdf}}
```
#### Podziel każdą stronę pliku PDF do osobnych plików, o nazwie nadanej według zdefiniowanego wzoru:
```shell
pdftk {{plik_wejściowy.pdf}} burst output {{plik_wyjściowy_%d.pdf}}
```
#### Obróć wszystkie strony o 180 stopni zgodnie ze wskazówkami zegara:
```shell
pdftk {{plik_wejściowy.pdf}} cat {{1-endsouth}} output {{plik_wyjściowy.pdf}}
```
#### Obóć trzecią stronę o 90 stopni zgodnie ze wskazówkami zegara oraz pozostaw pozostałe strony bez zmian:
```shell
pdftk {{plik_wejściowy.pdf}} cat {{1-2 3east 4-end}} output {{plik_wyjściowy.pdf}}
```
{% endraw %}{% raw %}
<h2 id="php">
  <a href="/pl/common/php.html">php</a> <a href="#php"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfejs wiersza poleceń PHP.
> Więcej informacji: <https://php.net>.

#### Parsuj i uruchom skrypt php:
```shell
php {{plik}}
```
#### Sprawdź składnię skryptu PHP (np. lint):
```shell
php -l {{plik}}
```
#### Uruchom PHP interaktywnie:
```shell
php -a
```
#### Uruchom kod PHP (uwagi: nie używaj znaczników <? ?> ; unikaj podwójnych cudzysłowów z odwrotnym ukośnikiem):
```shell
php -r "{{kod}}"
```
#### uruchom wbudowany serwer PHP w bieżącym katalogu:
```shell
php -S {{host:port}}
```
#### Uzyskaj listę zainstalowanych rozszerzeń PHP:
```shell
php -m
```
#### Wyświetl informacje o bieżącej konfiguracji PHP:
```shell
php -i
```
{% endraw %}{% raw %}
<h2 id="python">
  <a href="/pl/common/python.html">python</a> <a href="#python"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interpreter języka Python.
> Więcej informacji: <https://www.python.org>.

#### Wywołaj interaktywną powłokę Pythona (REPL):
```shell
python
```
#### Wykonaj skrypt w danym pliku Python:
```shell
python {{skrypt.py}}
```
#### Wykonaj skrypt jako część interaktywnej powłoki:
```shell
python -i {{skrypt.py}}
```
#### Wykonaj wyrażenie w języku Python:
```shell
python -c "{{wyrazenie}}"
```
#### Uruchom moduł biblioteki jako skrypt (kończy listę opcji):
```shell
python -m {{moduł}} {{argumenty}}
```
#### Interaktywnie debuguj skrypt w języku Python:
```shell
python -m pdb {{skrypt.py}}
```
{% endraw %}{% raw %}
<h2 id="r">
  <a href="/pl/common/r.html">r</a> <a href="#r"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interpreter języka R.
> Więcej informacji: <https://www.r-project.org>.

#### Uruchom interaktywną powłokę R (REPL):
```shell
R
```
#### Sprawdź wersję R:
```shell
R --version
```
#### Uruchom plik:
```shell
R -f {{plik.R}}
```
{% endraw %}{% raw %}
<h2 id="rar">
  <a href="/pl/common/rar.html">rar</a> <a href="#rar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator RAR. Obsługuje wielotomowe archiwa, które mogą być opcjonalnie samorozpakowujące się.

#### Zarchiwizuj 1 lub więcej plików:
```shell
rar a {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik1}} {{sciezka/do/plik2}} {{sciezka/do/plik3}}
```
#### Zarchiwizuj katalog:
```shell
rar a {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/katalog}}
```
#### Podziel archiwum na części równej wielkości (50M):
```shell
rar a -v{{50M}} -R {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
#### Chroń hasło wynikowego archiwum:
```shell
rar a -p{{haslo}} {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
#### Szyfruj dane pliku i nagłówki za pomocą hasła:
```shell
rar a -hp{{haslo}} {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
#### Użyj określonego poziomu kompresji (0-5):
```shell
rar a -m{{poziom_kompresji}} {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
{% endraw %}{% raw %}
<h2 id="rm">
  <a href="/pl/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Usuwa pliki lub foldery.
> Więcej informacji: <https://www.gnu.org/software/coreutils/rm>.

#### Usuń pliki z dowolnej lokalizacji:
```shell
rm {{ścieżka/do/pliku}} {{ścieżka/do/innego/pliku}}
```
#### Rekursywnie usuń folder oraz wszystkie jego podfoldery:
```shell
rm -r {{ścieżka/do/folderu}}
```
#### Wymuś usunięcie folderu, bez pytania o potwierdzenie lub pokazywania błędów:
```shell
rm -rf {{ścieżka/do/folderu}}
```
#### Interaktywnie usuń kilka plików z pytaniem o potwierdzenie przed każdym usunięciem:
```shell
rm -i {{plik(i)}}
```
#### Usuń pliki w trybie opisowym, pokazując wiadomość o każdym usuniętym pliku:
```shell
rm -v {{ścieżka/do/folderu/*}}
```
{% endraw %}{% raw %}
<h2 id="sass">
  <a href="/pl/common/sass.html">sass</a> <a href="#sass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konwertuje pliki SCSS lub Sass na CSS.
> Więcej informacji: <https://sass-lang.com/documentation/cli/dart-sass>.

#### Konwertuj plik SCSS lub Sass do CSS i wypisz wynik:
```shell
sass {{plikwejsciowy.scss|plikwejsciowy.sass}}
```
#### Konwertuj plik SCSS lub Sass do CSS i zapisz wynik w pliku:
```shell
sass {{plikwejsciowy.scss|plikwejsciowy.sass}} {{plikwyjsciowy.css}}
```
#### Obejrzyj zmiany w pliku SCSS lub Sass i wyślij lub zaktualizuj plik CSS o tej samej nazwie:
```shell
sass --watch {{plikwejsciowy.scss|plikwejsciowy.sass}}
```
#### Obejrzyj zmiany w pliku SCSS lub Sass i wyślij lub zaktualizuj plik CSS o podanej nazwie:
```shell
sass --watch {{plikwejsciowy.scss|plikwejsciowy.sass}}:{{plikwyjsciowy.css}}
```
{% endraw %}{% raw %}
<h2 id="sudo">
  <a href="/pl/common/sudo.html">sudo</a> <a href="#sudo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wykonuje pojedyncze polecenie jako superuser lub inny użytkownik.

#### Uruchom polecenie jako superuser:
```shell
sudo {{less /var/log/syslog}}
```
#### Edytuj plik jako superuser w domyślnym edytorze:
```shell
sudo -e {{/etc/fstab}}
```
#### Uruchom polecenie jako inny użytkownik i/lub grupa:
```shell
sudo -u {{uzytkownik}} -g {{grupa}} {{id -a}}
```
#### Powtórz ostatnie polecenie poprzedzone `sudo` (tylko w `bash`, `zsh`, etc.):
```shell
sudo !!
```
#### Uruchom domyślną powłokę z uprawnieniami superuser:
```shell
sudo -i
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/pl/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Klient wiersza polecenia dla stron tldr.
> Wyświetla uproszczone i obsługiwane przez społeczność strony podręcznika man.
> Więcej informacji: <https://tldr.sh>.

#### Uzyskaj typowe zastosowania polecenia (wskazówka: oto jak się tu dostałeś!):
```shell
tldr {{polecenie}}
```
#### Pokaż tar tldr page dla Linux:
```shell
tldr -p {{linux}} {{tar}}
```
#### Uzyskaj pomoc dotyczącą komendy Git:
```shell
tldr {{git-checkout}}
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="vue">
  <a href="/pl/common/vue.html">vue</a> <a href="#vue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wielofunkcyjny interfejs CLI dla Vue.js.
> Więcej informacji: <https://cli.vuejs.org>.

#### Utwórz nowy projekt vue interaktywnie:
```shell
vue create {{nazwa_projektu}}
```
#### Utwórz nowy projekt z web UI:
```shell
vue ui
```
{% endraw %}{% raw %}
<h2 id="xkcdpass">
  <a href="/pl/common/xkcdpass.html">xkcdpass</a> <a href="#xkcdpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konfigurowalny generator haseł tworzący mocne hasła.
> Zainspirowane przez XKCD 936.
> Więcej informacji: <https://github.com/redacted/XKCD-password-generator>.

#### Stwórz hasło z domyślną konfiguracją:
```shell
xkcdpass
```
#### Stwórz hasło w którym pierwsze litery każdego słowa układają się w podany argument:
```shell
xkcdpass -a {{acrostic}}
```
#### Interaktywnie stwórz hasło:
```shell
xkcdpass -i
```
{% endraw %}{% raw %}
<h2 id="xkill">
  <a href="/pl/common/xkill.html">xkill</a> <a href="#xkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zabija okno z sesji graficznej.
> Zobacz też `kill` i `killall`.

#### Wyświetla kursor pozwalający na wybranie okna do zabicia przy pomocy lewego przycisku myszy (pozostałe przyciski anulują):
```shell
xkill
```
{% endraw %}{% raw %}
<h2 id="youtube-dl">
  <a href="/pl/common/youtube-dl.html">youtube-dl</a> <a href="#youtube-dl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pobieraj wideo i audio z YouTube i podobnych portali
> Więcej informacji: <http://rg3.github.io/youtube-dl/>.

#### Pobierz plik wideo lub wszystkie pliki z playlisty:
```shell
youtube-dl '{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}'
```
#### Listuj wszystkie formaty dostępne dla filmu lub playlisty:
```shell
youtube-dl --list-formats '{{https://www.youtube.com/watch?v=Mwa0_nE9H7A}}'
```
#### Pobierz wideo lub playlistę w wybranej jakości:
```shell
youtube-dl --format "{{best[height<=480]}}" '{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}'
```
#### Pobierz audio z wideo w formacie mp3:
```shell
youtube-dl -x --audio-format {{mp3}} '{{url}}'
```
#### Pobierz wideo ze ścieżką audio złączone w jendym pliku w najlepszej dostępnej jakości:
```shell
youtube-dl -f bestvideo+bestaudio '{{url}}'
```
#### Pobierz wideo jako pliki MP4 i nazwij wedle schematu:
```shell
youtube-dl --format {{mp4}} -o "{{%(title)s by %(uploader)s on %(upload_date)s in %(playlist)s.%(ext)s}}" '{{url}}'
```
#### Pobierz plik razem z napisami:
```shell
youtube-dl --sub-lang {{en}} --write-sub '{{https://www.youtube.com/watch?v=Mwa0_nE9H7A}}'
```
#### Pobierz ścieżkę dźwiękową ze wszystkich filmów z playlisty:
```shell
youtube-dl -i --extract-audio --audio-format mp3 -o "%(title)s.%(ext)s" '{{adres_url_playlisty}}'
```
{% endraw %}