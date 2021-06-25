---
layout: default
title: "RU"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#common">Common</a>
  * <a href="#7z">7z</a>
  * <a href="#7za">7za</a>
  * <a href="#7zr">7zr</a>
  * <a href="#adguardhome">AdGuardHome</a>
  * <a href="#aapt">aapt</a>
  * <a href="#ab">ab</a>
  * <a href="#abduco">abduco</a>
  * <a href="#ack">ack</a>
  * <a href="#act">act</a>
  * <a href="#adb">adb</a>
  * <a href="#adb-install">adb install</a>
  * <a href="#adb-reverse">adb reverse</a>
  * <a href="#adb-shell">adb shell</a>
  * <a href="#ag">ag</a>
  * <a href="#cat">cat</a>
  * <a href="#chmod">chmod</a>
  * <a href="#dotnet">dotnet</a>
  * <a href="#dotnet-build">dotnet build</a>
  * <a href="#dotnet-publish">dotnet publish</a>
  * <a href="#dotnet-restore">dotnet restore</a>
  * <a href="#ls">ls</a>
  * <a href="#micro">micro</a>
  * <a href="#tar">tar</a>
  * <a href="#tldr">tldr</a>
  * <a href="#unzip">unzip</a>
  * <a href="#weasyprint">weasyprint</a>
  * <a href="#zip">zip</a>


# Common
{% raw %}
<h2 id="7z">
  <a href="/ru/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Архиватор файлов с высокой степенью сжатия.
> Больше информации: <https://www.7-zip.org/>.

#### Архивировать файл или папку:
```shell
7z a {{архив.7z}} {{путь/до/файла_или_папки}}
```
#### Зашифровать существующий архив (включая заголовки):
```shell
7z a {{зашифрованный.7z}} -p{{пароль}} -mhe=on {{архив.7z}}
```
#### Распаковать существующий архив 7z с оригинальной структурой папок:
```shell
7z x {{архив.7z}}
```
#### Распаковать архив в нужную папку:
```shell
7z x {{архив.7z}} -o{{путь/до/папки}}
```
#### Распаковать архив в stdout:
```shell
7z x {{архив.7z}} -so
```
#### Архивировать, используя определённый тип архива:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{архив.7z}} {{путь/до/файла_или_папки}}
```
#### Вывести вписок всех доступных типов архивов:
```shell
7z i
```
#### Вывести список файлов и папок в архиве:
```shell
7z l {{архив.7z}}
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/ru/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Архиватор файлов с высокой степенью сжатия.
> Автономная версия `7z` с поддержкой меньшего количества типов архивов
> Больше информации: <https://www.7-zip.org/>.

#### Архивировать файл или папку:
```shell
7za a {{архив.7z}} {{путь/до/файла_или_папки}}
```
#### Распаковать существующий архив 7z с оригинальной структурой папок:
```shell
7za x {{архив.7z}}
```
#### Архивировать, используя определённый тип архива:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{архив.7z}} {{путь/до/файла_или_папки}}
```
#### Вывести вписок всех доступных типов архивов:
```shell
7za i
```
#### Вывести список файлов и папок в архиве:
```shell
7za l {{архив.7z}}
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/ru/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Архиватор файлов с высокой степенью сжатия.
> Автономная версия `7z`, которая поддерживает только файлы .7z.
> Больше информации: <https://www.7-zip.org/>.

#### Архивировать файл или папку:
```shell
7zr a {{архив.7z}} {{путь/до/файла_или_папки}}
```
#### Распаковать существующий архив 7z с оригинальной структурой папок:
```shell
7zr x {{архив.7z}}
```
#### Вывести список файлов и папок в архиве:
```shell
7zr l {{архив.7z}}
```
{% endraw %}{% raw %}
<h2 id="aapt">
  <a href="/ru/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита для упаковки ресурсов для Android.
> Компилирует и упаковывает ресурсы приложений Android.

#### Вывести список файлов содержащихся в APK-архиве:
```shell
aapt list {{путь/до/приложения.apk}}
```
#### Отобразить мета-данные приложения (версия, разрешения, и т.д.):
```shell
aapt dump badging {{путь/до/приложения.apk}}
```
#### Создать новый APK-архив с файлами из указанной папки:
```shell
aapt package -F {{путь/до/приложения.apk}} {{путь/до/папки}}
```
{% endraw %}{% raw %}
<h2 id="ab">
  <a href="/ru/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита бенчмаркинга Apache. Самая простая утилита для проведения нагрузочного тестирования.
> Больше информации: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Запустить 100 запросов HTTP GET по заданному URL:
```shell
ab -n {{100}} {{url}}
```
#### Запустить 100 запросов HTTP GET, обрабатывая до 10 одновременно, по заданному URL:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Использовать постоянное соединение (keep-alive):
```shell
ab -k {{url}}
```
#### Задать максимальное число секунд, которое можно затратить на бенчмаркинг:
```shell
ab -t {{60}} {{url}}
```
#### Запустить 100 запросов HTTP POST по заданному URL, используя в качестве полезной нагрузки JSON из файла:
```shell
ab -n {{100}} -T {{application/json}} -p {{путь/до/файла.json}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="abduco">
  <a href="/ru/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Менеджер сессий терминала.
> Больше информации: <http://www.brain-dump.org/projects/abduco/>.

#### Вывести список сеансов:
```shell
abduco
```
#### Подключиться к сеансу, и создать его, если он не существует:
```shell
abduco -A {{имя}} {{bash}}
```
#### Подключиться к сеансу с `dvtm`, и создать его, если он не существует:
```shell
abduco -A {{имя}}
```
#### Отключиться от сеанса:
```shell
Ctrl + \
```
#### Подключиться к сеансу в режиме только для чтения:
```shell
abduco -Ar {{имя}}
```
{% endraw %}{% raw %}
<h2 id="ack">
  <a href="/ru/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита для поиска, подобная grep, оптимизировання для программистов.
> Больше информации: <https://beyondgrep.com/documentation/>.

#### Найти файлы, содержащие "foo":
```shell
ack {{foo}}
```
#### Найти файлы заданного типа:
```shell
ack --ruby {{foo}}
```
#### Подсчитать общее число совпадений для термина "foo":
```shell
ack -ch {{foo}}
```
#### Показать имен файлов, содержащие "foo" и число совпадений в каждом файле:
```shell
ack -cl {{foo}}
```
#### Поиск заданной строки в файле:
```shell
ack bar "{{foo bar}}" {{путь/до/файла}}
```
#### Поиск в файле по заданному регулярному выражению:
```shell
ack bar "{{[bB]ar \d+}}" {{путь/до/файла}}
```
#### Вывести список всех допустимых типов:
```shell
ack --help-types
```
{% endraw %}{% raw %}
<h2 id="act">
  <a href="/ru/common/act.html">act</a> <a href="#act"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Запуск GitHub Actions локально с использованием Docker.
> Больше информации: <https://github.com/nektos/act>.

#### Вывести список доступных actions:
```shell
act -l
```
#### Запустить событие по умолчанию:
```shell
act
```
#### Запустить заданное событие:
```shell
act {{тип_события}}
```
#### Запустить заданный action:
```shell
act -a {{action_id}}
```
#### Не производить реальный запуск actions (пробный прогон):
```shell
act -n
```
#### Отображать расширенный лог:
```shell
act -v
```
{% endraw %}{% raw %}
<h2 id="adb-install">
  <a href="/ru/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: Установка пакетов на эмулятор Android или подключенное устройство Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Установить приложение Android на эмулятор/устройство:
```shell
adb install {{путь/до/файла.apk}}
```
#### Переустановить существующее приложение, оставив его данные:
```shell
adb install -r {{путь/до/файла.apk}}
```
#### Дать все разрешения, перечисленные в манифесте приложения:
```shell
adb install -g {{путь/до/файла.apk}}
```
#### Быстрое обновление установленного пакета путём обновления только тех частей APK, которые изменились:
```shell
adb install --fastdeploy {{путь/до/файла.apk}}
```
{% endraw %}{% raw %}
<h2 id="adb-reverse">
  <a href="/ru/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: обратное соединение от эмулятора Android или подключенного устройства Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Вывести список всех обратных соединений от эмуляторов и устройств:
```shell
adb reverse --list
```
#### Создать обратное соединение по TCP-порту от эмулятора или устройства до localhost:
```shell
adb reverse tcp:{{удалённый_порт}} tcp:{{локальный_порт}}
```
#### Удалить обратное соединение из эмулятора или устройства:
```shell
adb reverse --remove tcp:{{удалённый_порт}}
```
#### Удалить все обратные соединения на всех эмуляторах и устройствах:
```shell
adb reverse --remove-all
```
{% endraw %}{% raw %}
<h2 id="adb-shell">
  <a href="/ru/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Запуск удалённой командной оболочки на эмуляторе Android или подключенном устройстве Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Запустить удалённую интерактивную оболочку на эмуляторе или устройстве:
```shell
adb shell
```
#### Получить все свойства от эмулятора или устройства:
```shell
adb shell getprop
```
#### Вернуть всем разрешениям значение по умолчанию:
```shell
adb shell pm reset-permissions
```
#### Отозвать опасные разрешения для приложения:
```shell
adb shell pm revoke {{пакет}} {{разрешения}}
```
#### Вызвать событие клавиши:
```shell
adb shell input keyevent {{код_клавиши}}
```
#### Очистить данные приложения на эмуляторе или устройстве:
```shell
adb shell pm clear {{пакет}}
```
#### Запустить activity на эмуляторе или устройстве:
```shell
adb shell am start -n {{пакет}}/{{активность}}
```
#### Запустить базовый activity на эмуляторе или устройстве:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}{% raw %}
<h2 id="adb">
  <a href="/ru/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: управление запущенным эмулятором Android или подключенным устройством Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Проверить, запущен ли процесс сервера adb и запустить его:
```shell
adb start-server
```
#### Завершить процесс сервера adb:
```shell
adb kill-server
```
#### Запустить удалённую оболочку на целевом эмуляторе/устройстве:
```shell
adb shell
```
#### Установить приложение Android на эмуляторе/устройстве:
```shell
adb install -r {{путь/до/файла.apk}}
```
#### Скопировать файл/папку с целевого устройства:
```shell
adb pull {{путь/до/папки_или_файла_на_устройстве}} {{путь/до/локальной_папки}}
```
#### Скопировать файл/папку на целевое устройство:
```shell
adb push {{путь/до/локального_файла_или_папки}} {{путь/до/целевой_папки_на_устройстве}}
```
#### Вывести список подключенных устройств:
```shell
adb devices
```
{% endraw %}{% raw %}
<h2 id="adguardhome">
  <a href="/ru/common/adguardhome.html">AdGuardHome</a> <a href="#adguardhome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Программное обеспечение для блокировки рекламы и отслеживания во всей сети.
> Больше информации: <https://github.com/AdguardTeam/AdGuardHome>.

#### Запустить AdGuard Home:
```shell
AdGuardHome
```
#### Запустить AdGuard с заданной конфигурацией:
```shell
AdGuardHome --config {{путь/до/AdGuardHome.yaml}}
```
#### Установить рабочую папку, где будут сохранятья данные:
```shell
AdGuardHome --work-dir {{путь/до/папки}}
```
#### Установить или удалить AdGuard Home как службу:
```shell
AdGuardHome --service {{install|uninstall}}
```
#### Запустить службу AdGuard Home:
```shell
AdGuardHome --service start
```
#### Перезагрузить конфигурацию для службы AdGuard Home:
```shell
AdGuardHome --service reload
```
#### Остановить или перезапустить службу AdGuard Home:
```shell
AdGuardHome --service {{stop|restart}}
```
{% endraw %}{% raw %}
<h2 id="ag">
  <a href="/ru/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. Аналог ack, но имеет цель быть быстрее.
> Больше информации: <https://github.com/ggreer/the_silver_searcher>.

#### Найти файлы, содержащие "foo", и вывести подходящие строки в контексте:
```shell
ag {{foo}}
```
#### Найти файлы, содержащие "foo", в заданной папке:
```shell
ag {{foo}} {{путь/до/папки}}
```
#### Найти файлы, содержащие "foo", но вывести только имена файлов:
```shell
ag -l {{foo}}
```
#### Найти файлы, содержащие "FOO", независимо от регистра, и вывести только совпадения, а не строки целиком:
```shell
ag -i -o {{FOO}}
```
#### Найти "foo" в файлах, у которых в имени есть "bar":
```shell
ag {{foo}} -G {{bar}}
```
#### Найти файлы, содержимое которых совпадает с регулярным выражением:
```shell
ag '{{^ba(r|z)$}}'
```
#### Найти файлы, у которых имя совпадает с "foo":
```shell
ag -g {{foo}}
```
{% endraw %}{% raw %}
<h2 id="cat">
  <a href="/ru/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Выводит и объединяет файлы.
> Больше информации: <https://www.gnu.org/software/coreutils/cat>.

#### Выводит содержимое файла:
```shell
cat {{файл}}
```
#### Объединяет несколька файлов в один:
```shell
cat {{файл1}} {{файл2}} > {{итоговый_файл}}
```
#### Добавляет несколько файлов в конец файла:
```shell
cat {{файл1}} {{файл2}} >> {{итоговый_файл}}
```
#### Выводит содержимое файла с нумерацией строк:
```shell
cat -n {{файл}}
```
#### Показывает все непечатные символы и пробелы (с префиксом `M-` для не-ASCII символов):
```shell
cat -v -t -e {{файл}}
```
{% endraw %}{% raw %}
<h2 id="chmod">
  <a href="/ru/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Изменить права доступа файлу или папке.
> Больше информации: <https://www.gnu.org/software/coreutils/chmod>.

#### Дать [u]пользователю, который владеет файлом, права на его [x]исполнение:
```shell
chmod u+x {{файл}}
```
#### Дать права [u]пользователю права [r]чтения и [w]записи в файл/папку:
```shell
chmod u+rw {{файл_или_папка}}
```
#### Убрать права на [x]исполнение у [g]группы:
```shell
chmod g-x {{файл}}
```
#### Дать [a]всем пользователям права на [r]чтение и [x]исполенеие:
```shell
chmod a+rx {{файл}}
```
#### Дать [o]другим (не из группы владельцев файлом) такие же права как и у [g]группы:
```shell
chmod o=g {{файл}}
```
#### Убрать все права у [o]других:
```shell
chmod o= {{файл}}
```
#### Изменить права рекурсивно, дав [g]группе и [o]другим возможность [w]записи в папку:
```shell
chmod -R g+w,o+w {{папка}}
```
{% endraw %}{% raw %}
<h2 id="dotnet-build">
  <a href="/ru/common/dotnet-build.html">dotnet build</a> <a href="#dotnet-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Собирает приложение .NET и все его зависимости.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools/dotnet-build>.

#### Скомпилировать проект или решение в текущей директории:
```shell
dotnet build
```
#### Скомпилировать проект или решение .NET в режиме debug:
```shell
dotnet build {{путь/до/проекта_или_решения}}
```
#### Скомпилировать в режиме release:
```shell
dotnet build --configuration {{Release}}
```
#### Скомпилировать без восстановления зависимостей:
```shell
dotnet build --no-restore
```
#### Скомпилировать с заданным уровнем детализации выводимой информации:
```shell
dotnet build --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
#### Скомпилировать для заданной среды исполнения:
```shell
dotnet build --runtime {{идентификатор_среды_исполения}}
```
#### Указать целевую папку:
```shell
dotnet build --output {{путь/до/папки}}
```
{% endraw %}{% raw %}
<h2 id="dotnet-publish">
  <a href="/ru/common/dotnet-publish.html">dotnet publish</a> <a href="#dotnet-publish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Публикует .NET-приложение и его зависимости в папку для развёртываения на целевой системе.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools/dotnet-publish>.

#### Скомпилировать проект .NET в режиме release:
```shell
dotnet publish --configuration Release {{путь/до/файла_проекта}}
```
#### Опубликовать ваше приложение с заданной средой исполнения .NET Core:
```shell
dotnet publish --self-contained true --runtime {{идентификатор_среды_исполения}} {{путь/до/файла_проекта}}
```
#### Упаковать приложение в один исполняемый файл для заданной платформы:
```shell
dotnet publish --runtime {{идентификатор_среды_исполения}} -p:PublishSingleFile=true {{путь/до/файла_проекта}}
```
#### Обрезать неиспользуемые библиотеки чтобы уменьшить размер развёртывания приложения:
```shell
dotnet publish --self-contained true --runtime {{идентификатор_среды_исполения}} -p:PublishTrimmed=true {{путь/до/файла_проекта}}
```
#### Скомпилировать проект .NET без восстановления зависимостей:
```shell
dotnet publish --no-restore {{путь/до/файла_проекта}}
```
#### Указать целевую папку:
```shell
dotnet publish --output {{путь/до/папки}} {{путь/до/файла_проекта}}
```
{% endraw %}{% raw %}
<h2 id="dotnet-restore">
  <a href="/ru/common/dotnet-restore.html">dotnet restore</a> <a href="#dotnet-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Восстанавливает зависимости и утилиты для проекта .NET.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools/dotnet-restore>.

#### Восстановить зависимости для проекта или решения .NET в текущей директории:
```shell
dotnet restore
```
#### Восстановить зависимости для проекта или решенияs .NET по заданному пути:
```shell
dotnet restore {{путь/до/проекта_или_решения}}
```
#### Восстановить зависимости без кеширования HTTP-запросов:
```shell
dotnet restore --no-cache
```
#### Принудительно восстановить все зависимости, даже если предыдущее восстановление было успешным:
```shell
dotnet restore --force
```
#### Восстановить зависимости, считая что ошибки источника пакетов это предупреждения:
```shell
dotnet restore --ignore-failed-sources
```
#### Восстановить зависимости, используя заданный уровень детализации выводимой информации:
```shell
dotnet restore --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
{% endraw %}{% raw %}
<h2 id="dotnet">
  <a href="/ru/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Кросс-платформенная утилита командной строки .NET для .NET Core.
> Больше информации: <https://docs.microsoft.com/dotnet/core/tools>.

#### Инициализировать новый проект .NET:
```shell
dotnet new {{короткое_имя_шаблона}}
```
#### Восстановить пакеты nuget:
```shell
dotnet restore
```
#### Собрать и запустить проект .NET в текущей папке:
```shell
dotnet run
```
#### Запустить собранное приложение .NET (требуется только среда исполнения, для остальных команд требуется установленный .NET Core SDK):
```shell
dotnet {{путь/до/приложения.dll}}
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/ru/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Выводит содержимого каталога.
> Больше информации: <https://www.gnu.org/software/coreutils/ls>.

#### Список файлов по одному в строке:
```shell
ls -1
```
#### Список всех файлов, включая скрытые:
```shell
ls -a
```
#### Список всех файлов с добавлением в конце `/` к именам каталогов:
```shell
ls -F
```
#### Подробный список с выводом разрешений, прав собственности, размера и даты изменения всех файлов:
```shell
ls -la
```
#### Подробный список с выводом размера файла в удобочитаемых единицах (КиБ, МиБ, ГиБ):
```shell
ls -lh
```
#### Подробный список отсортированный по размеру файлов (по убыванию):
```shell
ls -lS
```
#### Подробный список отсортированный по дате изменения файла (более старые файлы сначала):
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="micro">
  <a href="/ru/common/micro.html">micro</a> <a href="#micro"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Micro - это современный и интуитивно понятный консольный текстовый редактор.
> Micro поддерживает клавиатуру и мышь для навигации и/или выделения текста.
> Больше информации: <https://micro-editor.github.io>.

#### Открыть файл:
```shell
micro {{файл}}
```
#### Вырезать всю строку:
```shell
Ctrl + K
```
#### Искать в файле (используйте `Ctrl + N`/`Ctrl + P` чтобы перейти к следующему/предыдущему совпадению):
```shell
Ctrl + F "{{паттерн}}" <Ввод>
```
#### Выполнить команду:
```shell
Ctrl + E {{команда}} <Ввод>
```
#### Выполнить замену во всем файле:
```shell
Ctrl + E replaceall "{{строка}}" "{{замена}}" <Ввод>
```
#### Выход:
```shell
Ctrl + Q
```
{% endraw %}{% raw %}
<h2 id="tar">
  <a href="/ru/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита архивирования.
> Обычно используется в сочетании с методом сжатия, такими как gzip или bzip2.
> Больше информации: <https://www.gnu.org/software/tar>.

#### Создать архив из файлов:
```shell
tar cf {{целевой.tar}} {{файл1}} {{файл2}} {{файл3}}
```
#### Создать gzip архив:
```shell
tar czf {{целевой.tar.gz}} {{файл1}} {{файл2}} {{файл3}}
```
#### Создать gzip архив из деректории, используя относительные пути:
```shell
tar czf {{целевой.tar.gz}} -C {{путь/до/папки}} .
```
#### Извлечь (сжатый) архив в текущую папку:
```shell
tar xf {{исходный.tar[.gz|.bz2|.xz]}}
```
#### Извлечь (сжатый) архив в указанную папку:
```shell
tar xf {{исходный.tar[.gz|.bz2|.xz]}} -C {{папка}}
```
#### Создать сжатый архив, использую суффикс архива для определения программы сжатия:
```shell
tar caf {{целевой.tar.xz}} {{файл1}} {{файл2}} {{файл3}}
```
#### Вывести список содержимого tar файла:
```shell
tar tvf {{исходный.tar}}
```
#### Извлечь файлы удовлетворяющие шаблону:
```shell
tar xf {{исходный.tar}} --wildcards "{{*.html}}"
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/ru/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Показывает простые страницы помощи для инструментов коммандной строки из проекта tldr-pages.
> Больше информации: <https://tldr.sh>.

#### Показывает типичное использование комманды (подсказка: то как вы попали сюда!):
```shell
tldr {{комманда}}
```
#### Показывает tldr страницу для комманды tar для Linux:
```shell
tldr -p {{linux}} {{tar}}
```
#### Получить помощь по подкоманде Git:
```shell
tldr {{git-checkout}}
```
#### Обновить локальные tldr страницы (если клиент поддерживает кэширование):
```shell
tldr -u
```
{% endraw %}{% raw %}
<h2 id="unzip">
  <a href="/ru/common/unzip.html">unzip</a> <a href="#unzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Извлекает сжатые файлы из архива zip.

#### Распаковать файл(ы) zip (для нескольких файлов укажите пути через пробел):
```shell
unzip {{архив(ы)}}
```
#### Распаковать файл(ы) по нужному пути:
```shell
unzip {{архив(ы)}} -d {{/путь/куда/положить/извлечённый_файл(ы)}}
```
#### Вывести список файлов в архиве zip, не распаковывая их:
```shell
unzip -l {{архив.zip}}
```
#### Извлечь содержимое файла в stdout вместе с именами распакованных файлов:
```shell
unzip -c {{архив.zip}}
```
#### Распаковать архив zip, который был создан на windows и содержит не-ascii имена файлов (напр. кириллица):
```shell
unzip -O {{gbk}} {{архив.zip}}
```
{% endraw %}{% raw %}
<h2 id="weasyprint">
  <a href="/ru/common/weasyprint.html">weasyprint</a> <a href="#weasyprint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Переводить HTML в PDF или PNG.
> Больше информации: <https://weasyprint.org/>.

#### Перевести HTML файл в PDF:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.pdf}}
```
#### Перевести HTML файл в PNG, включая дополнительные пользовательские таблицы стилей:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.png}} --stylesheet {{путь/до/таблицы-стилей.css}}
```
#### При переводе выводить дополнительную отладочную информацию:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.pdf}} --verbose
```
#### При выводе в PNG указать нестандартное разрешение:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.png}} --resolution {{300}}
```
#### Во входном HTML файле указать базовый URL для относительных URLs:
```shell
weasyprint {{путь/до/входного.html}} {{путь/до/выходного.png}} --base-url {{url_или_имя-файла}}
```
{% endraw %}{% raw %}
<h2 id="zip">
  <a href="/ru/common/zip.html">zip</a> <a href="#zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Упаковывает и сжимает (архивирует) файлы в файл zip.

#### Упаковать и сжать папку и её содержимое, рекурсивно ([r]ecursive):
```shell
zip -r {{архив.zip}} {{/путь/до/папки}}
```
#### Исключить (e[x]clude) ненужные файлы из добавляемых в сжатый архив:
```shell
zip -r {{архив.zip}} {{путь/до/папки}} -x {{путь/который/исключаем}}
```
#### Архивировать папку и её содержимое с самым сильным [9] сжатием:
```shell
zip -r -{{9}} {{архив.zip}} {{/путь/до/папки}}
```
#### Упаковать и сжать несколько папок и файлов:
```shell
zip -r {{архив.zip}} {{/путь/до/папки1 /путь/до/папки2 /путь/до/файла}}
```
#### Создать зашифрованный архив (пользователя спросят пароль):
```shell
zip -e -r {{архив.zip}} {{путь/до/папки}}
```
#### Добавить файлы в существующий файл zip:
```shell
zip {{архив.zip}} {{путь/до/файла}}
```
#### Удалить файлы из существующего файла zip:
```shell
zip -d {{архив.zip}} "{{папка/*.tmp}}"
```
#### Архивировать папку и её содержимое, разделив ([s]plit) файл zip на несколько томов (например, кусками по 3 ГБ):
```shell
zip -r -s {{3g}} {{архив.zip}} {{путь/до/папки}}
```
{% endraw %}