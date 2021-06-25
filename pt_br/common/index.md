---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#2to3">2to3</a>
* <a href="#7z">7z</a>
* <a href="#7za">7za</a>
* <a href="#7zr">7zr</a>
* <a href="#[">[</a>
* <a href="#ab">ab</a>
* <a href="#ack">ack</a>
* <a href="#adb-shell">adb shell</a>
* <a href="#airmon-ng">airmon-ng</a>
* <a href="#airpaste">airpaste</a>
* <a href="#alias">alias</a>
* <a href="#apg">apg</a>
* <a href="#apm">apm</a>
* <a href="#arch">arch</a>
* <a href="#arduino">arduino</a>
* <a href="#arduino-builder">arduino-builder</a>
* <a href="#arp">arp</a>
* <a href="#asdf">asdf</a>
* <a href="#at">at</a>
* <a href="#aws">aws</a>
* <a href="#aws-ec2">aws ec2</a>
* <a href="#aws-s3">aws s3</a>
* <a href="#axel">axel</a>
* <a href="#az">az</a>
* <a href="#bash">bash</a>
* <a href="#bat">bat</a>
* <a href="#bg">bg</a>
* <a href="#bundle">bundle</a>
* <a href="#bzip2">bzip2</a>
* <a href="#cat">cat</a>
* <a href="#clear">clear</a>
* <a href="#clj">clj</a>
* <a href="#code">code</a>
* <a href="#command">command</a>
* <a href="#convert">convert</a>
* <a href="#curl">curl</a>
* <a href="#docker">docker</a>
* <a href="#docker-build">docker build</a>
* <a href="#docker-images">docker images</a>
* <a href="#docker-logs">docker logs</a>
* <a href="#docker-ps">docker ps</a>
* <a href="#docker-run">docker run</a>
* <a href="#docker-start">docker start</a>
* <a href="#doxygen">doxygen</a>
* <a href="#gcc">gcc</a>
* <a href="#gdb">gdb</a>
* <a href="#git">git</a>
* <a href="#git-add">git add</a>
* <a href="#git-mv">git mv</a>
* <a href="#git-remote">git remote</a>
* <a href="#gpg">gpg</a>
* <a href="#gplusplus">gplusplus</a>
* <a href="#gzip">gzip</a>
* <a href="#helm">helm</a>
* <a href="#htop">htop</a>
* <a href="#jar">jar</a>
* <a href="#kill">kill</a>
* <a href="#kubectl">kubectl</a>
* <a href="#ls">ls</a>
* <a href="#lsof">lsof</a>
* <a href="#man">man</a>
* <a href="#meteor">meteor</a>
* <a href="#mongo">mongo</a>
* <a href="#mvn">mvn</a>
* <a href="#mysql">mysql</a>
* <a href="#mysqldump">mysqldump</a>
* <a href="#nativefier">nativefier</a>
* <a href="#node">node</a>
* <a href="#pdftk">pdftk</a>
* <a href="#rails">rails</a>
* <a href="#rails-generate">rails generate</a>
* <a href="#rbenv">rbenv</a>
* <a href="#rvm">rvm</a>
* <a href="#scc">scc</a>
* <a href="#tar">tar</a>
* <a href="#touch">touch</a>
* <a href="#uname">uname</a>
* <a href="#units">units</a>
* <a href="#unrar">unrar</a>
* <a href="#unzip">unzip</a>
* <a href="#wordgrinder">wordgrinder</a>
* <a href="#wpa_supplicant">wpa_supplicant</a>
* <a href="#xcv">xcv</a>
* <a href="#xkill">xkill</a>
* <a href="#xz">xz</a>
* <a href="#yarn-why">yarn-why</a>
* <a href="#yes">yes</a>
* <a href="#zip">zip</a>

{% raw %}
<h2 id="2to3">
  <a href="/pt_br/common/2to3.html">2to3</a> <a href="#2to3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Conversão automática de código Python 2 para Python 3.
> Mais informações: <https://docs.python.org/3/library/2to3.html>.

#### Mostrar as alterações que seriam feitas sem faze-las de fato (simulação):
```shell
2to3 {{caminho/para/arquivo.py}}
```
#### Converter um arquivo feito em Python 2 para Python 3:
```shell
2to3 --write {{caminho/para/arquivo.py}}
```
#### Converter recurso específico de Python 2 para Python 3:
```shell
2to3 --write {{caminho/para/arquivo.py}} --fix={{raw_input}} --fix={{print}}
```
#### Converter todos os recursos de Python 2 para Python 3, exceto as que específicadas:
```shell
2to3 --write {{caminho/para/arquivo.py}} --nofix={{has_key}} --nofix={{isinstance}}
```
#### Mostrar a lista de todas os recursos disponíveis que podem ser convertidas de Python 2 para Python 3:
```shell
2to3 --list-fixes
```
#### Converter todos os arquivos feitos em Python 2 em um diretório para Python 3:
```shell
2to3 --output-dir={{caminho/para/arquivos_python3}} --write-unchanged-files --nobackups {{caminho/para/arquivos_python2}}
```
#### Executar 2to3 com múltiplas threads:
```shell
2to3 --processes={{4}} --output-dir={{caminho/para/arquivos_python3}} --write --nobackups --no-diff {{caminho/para/arquivos_python2}}
```
{% endraw %}{% raw %}
<h2 id="7z">
  <a href="/pt_br/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compactador de arquivos com alta taxa de compressão.
> Mais informações: <https://www.7-zip.org/>.

#### Compactar um arquivo ou diretório:
```shell
7z a {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretório}}
```
#### Criptografar um arquivo existente (incluindo cabeçalhos):
```shell
7z a {{arquivo_criptografado.7z}} -p{{senha}} -mhe=on {{arquivo.7z}}
```
#### Descompactar um arquivo mantendo a estrutura de diretórios original:
```shell
7z x {{arquivo.7z}}
```
#### Descompactar um arquivo em um diretório específicado pelo usuário:
```shell
7z x {{arquivo.7z}} -o{{caminho/diretório}}
```
#### Compactar utilizando um tipo específico de arquivamento/compressão:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretório}}
```
#### Exibir os tipos de arquivamento/compressão disponíveis:
```shell
7z i
```
#### Exibir o conteúdo de um arquivo:
```shell
7z l {{arquivo.7z}}
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/pt_br/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compactador de arquivos com alta taxa de compressão.
> Versão compacta do `7z`, com suporte para menos tipos de arquivamento/compressão.
> Mais informações: <https://www.7-zip.org/>.

#### Compactar um arquivo ou diretório:
```shell
7za a {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretório}}
```
#### Descompactar um arquivo mantendo a estrutura de diretórios original:
```shell
7za x {{arquivo_compactado.7z}}
```
#### Compactar utilizando um tipo específico de arquivamento/compressão:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretório}}
```
#### Exibir os tipos de arquivamento/compressão disponíveis:
```shell
7za i
```
#### Exibir o conteúdo de um arquivo:
```shell
7za l {{arquivo.7z}}
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/pt_br/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compactador de arquivos com alta taxa de compressão.
> Versão do `7z` com suporte apenas para o formato `.7z`.
> Mais informações: <https://www.7-zip.org/>.

#### Compactar um arquivo ou diretório:
```shell
7zr a {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretorio}}
```
#### Descompactar um arquivo mantendo a estrutura de diretórios original:
```shell
7zr x {{arquivo_compactado.7z}}
```
#### Exibir o conteúdo de um arquivo:
```shell
7zr l {{arquivo_compactado.7z}}
```
{% endraw %}{% raw %}
<h2 id="[">
  <a href="/pt_br/common/[.html">[</a> <a href="#["><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Avalia condição.
> Retorna 0 se a condição for verdadeira, 1 se for falsa.
> Mais informações: <https://www.gnu.org/software/coreutils/test>.

#### Testa se uma determinada variável é igual a uma determinada string:
```shell
[ "{{$VARIAVEL}}" == "{{/bin/zsh}}" ]
```
#### Testa se uma determinada variável é vazia:
```shell
[ -z "{{$GIT_BRANCH}}" ]
```
#### Testa se um arquivo existe:
```shell
[ -f "{{caminho/para/arquivo}}" ]
```
#### Testa se um diretório não existe:
```shell
[ ! -d "{{caminho/para/diretorio}}" ]
```
#### Declaração de if-else:
```shell
[ {{condicao}} ] && {{echo "verdadeiro"}} || {{echo "falso"}}
```
{% endraw %}{% raw %}
<h2 id="ab">
  <a href="/pt_br/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta da Apache para realizar benchmarking e testes de carga em servidores web.
> Mais informações: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Executar 100 requisições HTTP do tipo GET para uma determinada URL:
```shell
ab -n {{100}} {{url}}
```
#### Executar 100 requisições HTTP do tipo GET para uma determinada URL, executando 10 requisições simultâneas de cada vez:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Utilizar a funcionalidade HTTP Keep Alive, permitindo que várias requisições sejam feitas em uma sessão HTTP:
```shell
ab -k {{url}}
```
#### Definir o tempo total do benchmarking, em segundos:
```shell
ab -t {{60}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="ack">
  <a href="/pt_br/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uma ferramenta de pesquisa similar ao grep, otimizada para programadores.
> Mais informações: <https://beyondgrep.com/documentation/>.

#### Procurar por arquivos que contenham o termo "foo":
```shell
ack {{foo}}
```
#### Procurar por arquivos em uma linguagem específica:
```shell
ack --ruby {{each_with_object}}
```
#### Contar o número total de correspondências para o termo "foo":
```shell
ack -ch {{foo}}
```
#### Mostrar o nome dos arquivos contendo o termo "foo" e o número de correspondências em cada arquivo:
```shell
ack -cl {{foo}}
```
{% endraw %}{% raw %}
<h2 id="adb-shell">
  <a href="/pt_br/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Executar remotamente comandos shell em instâncias do emulador Android ou dispositivos Android conectados.
> Mais informações: <https://developer.android.com/studio/command-line/adb?hl=pt-br>.

#### Iniciar um shell interativo remoto no emulador/dispositivo:
```shell
adb shell
```
#### Obter todas as propriedades do emulador ou dispositivo:
```shell
adb shell getprop
```
#### Reverter todas as permissões de tempo de execução para o padrão:
```shell
adb shell pm reset-permissions
```
#### Revogar uma permissão perigosa para um aplicação:
```shell
adb shell pm revoke {{pacote}} {{permissao}}
```
#### Acionar um evento:
```shell
adb shell input keyevent {{keycode}}
```
#### Limpar os dados da aplicação no emulador/dispositivo:
```shell
adb shell pm clear {{pacote}}
```
#### Iniciar uma atividade no emulator/dispositivo:
```shell
adb shell am start -n {{pacote}}/{{atividade}}
```
#### Iniciar atividade "home" no emulator/dispositivo:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}{% raw %}
<h2 id="airmon-ng">
  <a href="/pt_br/common/airmon-ng.html">airmon-ng</a> <a href="#airmon-ng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ativa modo de monitoramento em dispositivos de rede sem-fio.
> Mais informações: <https://www.aircrack-ng.org/doku.php?id=airmon-ng>.

#### Lista os dispositivos sem-fio e seus respectivos estados:
```shell
sudo airmon-ng
```
#### Liga o modo de monitoramento para um dispositivo específico:
```shell
sudo airmon-ng start {{wlan0}}
```
#### Encerra processos problemáticos que usam dispositivos sem-fio:
```shell
sudo airmon-ng check kill
```
#### Desativa o modo de monitoramento para um dispositivo específico:
```shell
sudo airmon-ng stop {{wlan0mon}}
```
{% endraw %}{% raw %}
<h2 id="airpaste">
  <a href="/pt_br/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compartilhar mensagens e arquivos na mesma rede.
> Mais informações: <https://github.com/mafintosh/airpaste>.

#### Esperar por mensagens e mostrá-las quando recebidas:
```shell
airpaste
```
#### Enviar texto:
```shell
echo {{texto}} | airpaste
```
#### Enviar arquivo:
```shell
airpaste < {{caminho/para/arquivo}}
```
#### Receber arquivo:
```shell
airpaste > {{caminho/para/arquivo}}
```
#### Criar/Entrar em canal:
```shell
airpaste {{nome_do_canal}}
```
{% endraw %}{% raw %}
<h2 id="alias">
  <a href="/pt_br/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cria apelidos -- palavras que são substituídas por um comando.
> Apelidos expiram ao final da sessão atual do shell de comando, a menos que sejam definidos no arquivo de configuração do shell, por exemplo `~/.bashrc`.
> Mais informações: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Criar um apelido:
```shell
alias {{apelido}}="{{comando}}"
```
#### Visualizar o comando associado a um determinado apelido:
```shell
alias {{apelido}}
```
#### Remover um apelido:
```shell
unalias {{apelido}}
```
#### Exibir todos os apelidos definidos:
```shell
alias -p
```
#### Tornar o comando `rm` interativo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Criar o apelido `la` como um atalho para `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}{% raw %}
<h2 id="apg">
  <a href="/pt_br/common/apg.html">apg</a> <a href="#apg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Criar senhas aleatórias arbitrariamente complexas.
> Mais informações: <https://manned.org/apg>.

#### Criar senha aleatória (tamanho padrão para as senhas é 8 caracteres):
```shell
apg
```
#### Criar senha com pelo menos 1 símbolo (S), 1 número (N), 1 letra maiúscula (C), 1 letra minúscula (L):
```shell
apg -M SNCL
```
#### Criar uma senha com 16 caracteres:
```shell
apg -m {{16}}
```
#### Criar senha com tamanho máximo de 16 caracteres:
```shell
apg -x {{16}}
```
#### Criar uma senha que não aparece em um dicionário provido pelo usuário:
```shell
apg -r {{arquivo_de_dicionario}}
```
{% endraw %}{% raw %}
<h2 id="apm">
  <a href="/pt_br/common/apm.html">apm</a> <a href="#apm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes do editor de texto Atom.
> Ver também `atom`.

#### Instalar pacotes de http://atom.io/packages e temas de http://atom.io/themes:
```shell
apm install {{nome_do_pacote}}
```
#### Remover pacotes/temas:
```shell
apm remove {{nome_do_pacote}}
```
#### Atualizar pacotes/temas:
```shell
apm upgrade {{nome_do_pacote}}
```
{% endraw %}{% raw %}
<h2 id="arch">
  <a href="/pt_br/common/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibir o nome da arquitetura do sistema.
> Veja também `uname`.
> Mais informações: <https://www.gnu.org/software/coreutils/arch>.

#### Exibir a arquitetura do sistema:
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="arduino-builder">
  <a href="/pt_br/common/arduino-builder.html">arduino-builder</a> <a href="#arduino-builder"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uma ferramenta de linha de comando para compilar sketches do arduino.
> AVIDO DE OBSOLESCÊNCIA: Esta ferramenta está sendo descontinuada e substituida pelo `arduino`.
> Mais informações: <https://github.com/arduino/arduino-builder>.

#### Compilar um sketch:
```shell
arduino-builder -compile {{caminho/para/sketch.ino}}
```
#### Definir o nível de debug (1 a 10, o padrão é 5):
```shell
arduino-builder -debug-level {{nivel}}
```
#### Definir um diretório de compilação customizado:
```shell
arduino-builder -build-path {{caminho/para/diretorio}}
```
#### Usar um arquivo com as opções de compilação, em vez de especificar `--hardware`, `--tools`, etc. manualmente toda hora:
```shell
arduino-builder -build-options-file {{caminho/para/build.options.json}}
```
#### Habilitar o modo verboso:
```shell
arduino-builder -verbose {{true}}
```
{% endraw %}{% raw %}
<h2 id="arduino">
  <a href="/pt_br/common/arduino.html">arduino</a> <a href="#arduino"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arduino Studio - Ambiente de Desenvolvimento Integrado para a plataforma Arduino.
> Mais informações: <https://github.com/arduino/Arduino/blob/master/build/shared/manpage.adoc>.

#### Compilar um sketch:
```shell
arduino --verify {{caminho/para/arquivo.ino}}
```
#### Compilar e enviar sketch:
```shell
arduino --upload {{caminho/para/arquivo.ino}}
```
#### Compilar e enviar sketch para um Arduino Nano com uma CPU Atmega328p, conectada na porta `/dev/ttyACM0`:
```shell
arduino --board {{arduino:avr:nano:cpu=atmega328p}} --port {{/dev/ttyACM0}} --upload {{caminho/para/arquivo.ino}}
```
#### Definir a preferência `nome` para um determinado `valor`:
```shell
arduino --pref {{nome}}={{valor}}
```
#### Compilar um sketch, colocar o resultado da compilação no diretório de compilação, e reutilizar qualquer resultado pre-existente neste diretório:
```shell
arduino --pref build.path={{caminho/para/diretório}} --verify {{caminho/para/arquivo.ino}}
```
#### Salvar todas as preferências (alteradas) para `preferences.txt`:
```shell
arduino --save-prefs
```
{% endraw %}{% raw %}
<h2 id="arp">
  <a href="/pt_br/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostrar e manipular a cache ARP do sistema.
> Mais informações: <https://manned.org/arp>.

#### Mostrar a tabela arp atual:
```shell
arp -a
```
#### Limpar toda a cache:
```shell
sudo arp -a -d
```
#### Eliminar uma entrada específica:
```shell
arp -d {{endereço}}
```
#### Criar uma entrada:
```shell
arp -s {{endereço}} {{endereço_mac}}
```
{% endraw %}{% raw %}
<h2 id="asdf">
  <a href="/pt_br/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para a gestão de versões de linguagens e programas.
> Mais informações: <https://asdf-vm.com>.

#### Listar todos os plugins disponíveis:
```shell
asdf plugin-list-all
```
#### Instalar um plugin:
```shell
asdf plugin-add {{nome}}
```
#### Listar todas as versões disponíveis para um pacote:
```shell
asdf list-all {{nome}}
```
#### Instalar uma versão específica de um pacote:
```shell
asdf install {{nome}} {{versão}}
```
#### Definir a versão global de um pacote:
```shell
asdf global {{nome}} {{versão}}
```
#### Definir a versão local de um pacote:
```shell
asdf local {{nome}} {{versão}}
```
{% endraw %}{% raw %}
<h2 id="at">
  <a href="/pt_br/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta para o agendamento de comandos.
> O serviço atd (ou atrun) deve estar sendo executado para as atuais execuções.
> Mais informações: <https://man.archlinux.org/man/at.1>.

#### Executar comandos da standard input em 5 minutos (pressionar `Ctrl + D`quando acabar):
```shell
at now + {{5}} minutes
```
#### Executar um comando da standard input às 10:00 da manhã de hoje:
```shell
echo "{{./comando.sh}}" | at 1000
```
#### Executar comandos de um dado arquivo na próxima terça:
```shell
at -f {{caminho/para/arquivo}} 9:30 PM Tue
```
{% endraw %}{% raw %}
<h2 id="aws-ec2">
  <a href="/pt_br/common/aws-ec2.html">aws ec2</a> <a href="#aws-ec2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inteface de linha de comando para o AWS EC2.
> Provê capacidade computacional segura e flexível na nuvem da AWS para proporcionar um desenvolvimento e subida para produção de aplicações rapidamente.
> Mais informações: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html>.

#### Lista todos os comandos EC2 disponíveis:
```shell
aws ec2 help
```
#### Exibe ajuda específica para um subcomando da EC2:
```shell
aws ec2 {{subcomando}} help
```
#### Exibe informações sobre uma insntância específica:
```shell
aws ec2 describe-instances --instance-ids {{id_da_instância}}
```
#### Exibe informações sobre todas as instâncias:
```shell
aws ec2 describe-instances
```
#### Exibe informações sobre todos os volumes EC2:
```shell
aws ec2 describe-volumes
```
#### Deleta um volume EC2:
```shell
aws ec2 delete-volume --volume-id {{id_do_volume}}
```
#### Cria um snapshot de um volume EC2:
```shell
aws ec2 create-snapshot --volume-id {{id_do_volume}}
```
#### Lista as AMIs (Imagem de Máquina da Amazon) disponíveis:
```shell
aws ec2 describe-images
```
{% endraw %}{% raw %}
<h2 id="aws-s3">
  <a href="/pt_br/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interface de linha de comando para AWS S3.
> Provê armazenamento através de uma interface de web services.
> Mais informações: <https://aws.amazon.com/cli>.

#### Exibe arquivos de um bucket:
```shell
aws s3 ls {{nome_do_bucket}}
```
#### Sincroniza arquivos e diretórios locais para o bucket:
```shell
aws s3 sync {{caminho/para/arquivos}} s3://{{nome_do_bucket}}
```
#### Sincroniza arquivos e diretórios do bucket para diretório local:
```shell
aws s3 sync s3://{{nome_do_bucket}} {{caminho/para/diretório}}
```
#### Sincroniza arquivos e diretórios excluindo algo:
```shell
aws s3 sync {{caminho/para/arquivos}} s3://{{nome_do_bucket}} --exclude {{arquivo/não/sincronizado}} --exclude {{caminho/não/sincronizado}}/*
```
#### Remove arquivo do bucket:
```shell
aws s3 rm s3://{{nome_do_bucket}}/{{caminho/do/arquivo}}
```
#### Somente exibe a prévia das mudanças:
```shell
aws s3 {{qualquer_comando}} --dryrun
```
{% endraw %}{% raw %}
<h2 id="aws">
  <a href="/pt_br/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A interface de linha de comando oficial para o Amazon Web Services.
> Passo-a-passo, Single Sign-On (SSO), autocompletar de recursos e opções de YAML somente na v2.
> Mais informações: <https://aws.amazon.com/cli>.

#### Configura a linha de comando da AWS:
```shell
aws configure wizard
```
#### Configura a linha de comando da AWS usando o SSO:
```shell
aws configure sso
```
#### Veja o texto de ajuda para o comando da AWS:
```shell
aws {{comando}} help
```
#### Obtenha a informações da identidade usada (útil para analisar problemas de permissão):
```shell
aws sts get-caller-identity
```
#### Lista recursos da AWS em uma região em yaml:
```shell
aws dynamodb list-tables --region {{sa-east-1}} --output yaml
```
#### Usa prompt de comando para ajuda com o preenchimento:
```shell
aws iam create-user --cli-auto-prompt
```
#### Usa um passo-a-passo interativo para um recurso da AWS:
```shell
aws dynamodb wizard {{nova-tabela}}
```
#### Gera um arquivo esqueleo em JSON (útil para ser usado em infraestrutura como código):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}{% raw %}
<h2 id="axel">
  <a href="/pt_br/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Acelerador de downloads.
> Suporta HTTP, HTTPS, e FTP.
> Mais informações: <https://github.com/axel-download-accelerator/axel>.

#### Fazer download de uma URL para um arquivo:
```shell
axel {{url}}
```
#### Fazer download especificando o nome do arquivo de destino:
```shell
axel {{url}} -o {{nome_do_arquivo}}
```
#### Fazer download usando múltiplas conexões:
```shell
axel -n {{número_de_conexões}} {{url}}
```
#### Procurar por mirrors:
```shell
axel -S {{número_de_mirrors}} {{url}}
```
#### Limitar velocidade de download (em bytes por segundo):
```shell
axel -s {{velocidade}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="az">
  <a href="/pt_br/common/az.html">az</a> <a href="#az"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A interface de linha de comando oficial do Microsoft Azure.

#### Fazer log in no Azure:
```shell
az login
```
#### Gerenciar informações de assinatura do Microsoft Azure:
```shell
az account
```
#### Listar todos os discos gerenciados pelo Azure:
```shell
az disk list
```
#### Listar todas as máquinas virtuais do Azure:
```shell
az vm list
```
#### Gerenciar os serviços do Azure Kubernetes:
```shell
az aks
```
#### Gerenciar recursos de rede do Azure:
```shell
az network
```
{% endraw %}{% raw %}
<h2 id="bash">
  <a href="/pt_br/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell, um interpretador de linha de comando compatível com `sh`.
> Veja também `histexpand` para a expansão do histórico.
> Mais informações: <https://gnu.org/software/bash/>.

#### Iniciar uma seção interativa do shell:
```shell
bash
```
#### Executar um comando e sair:
```shell
bash -c "{{comando}}"
```
#### Executar um script:
```shell
bash {{caminho/para/script.sh}}
```
#### Executar um script, exibindo cada comando antes de executá-lo:
```shell
bash -x {{caminho/para/script.sh}}
```
#### Executar os comandos de um script, parando de executar no primeiro erro:
```shell
bash -e {{caminho/para/script.sh}}
```
#### Ler e executar comandos do stdin (entrada padrão):
```shell
bash -s
```
#### Exibir a versão do Bash (`$BASH_VERSION` abrange apenas a versão sem informações da licença):
```shell
bash --version
```
{% endraw %}{% raw %}
<h2 id="bat">
  <a href="/pt_br/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprimir e concatenar arquivos.
> Um clone do `cat` com realce de sintaxe e integração com Git.
> Mais informações: <https://github.com/sharkdp/bat>.

#### Imprimir o conteúdo de um arquivo para a saída padrão:
```shell
bat {{arquivo}}
```
#### Concatenar vários arquivos em um arquivo de destino:
```shell
bat {{caminho/para/arquivo1}} {{caminho/para/arquivo2}} > {{caminho/para/arquivo_destino}}
```
#### Numerar todas as linhas do output:
```shell
bat -n {{caminho/para/arquivo}}
```
#### Realçar a sintaxe em um arquivo JSON:
```shell
bat --language json {{caminho/para/arquivo.json}}
```
#### Mostrar todas as linguagens suportadas:
```shell
bat --list-languages
```
{% endraw %}{% raw %}
<h2 id="bg">
  <a href="/pt_br/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retomar a execução, em segundo plano, de processos que foram suspensos (e.g. utilizando `Ctrl + Z`).
> Mais informações: <https://manned.org/bg>.

#### Retomar a execução, em segundo plano, do processo que foi suspenso mais recentemente:
```shell
bg
```
#### Retomar a execução, em segundo plano, de um processo especifico (utilizando `jobs -l` para obter o seu ID):
```shell
bg {{id_processo}}
```
{% endraw %}{% raw %}
<h2 id="bundle">
  <a href="/pt_br/common/bundle.html">bundle</a> <a href="#bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de dependências da linguagem de programação Ruby.
> Mais informações: <https://bundler.io/man/bundle.1.html>.

#### Instalar todas as gemas definidas no `Gemfile`:
```shell
bundle install
```
#### Atualizar todas as gemas, respeitando as regras definidas no `Gemfile`, e recriar o arquivo `Gemfile.lock`:
```shell
bundle update
```
#### Atualizar uma gema específica definida no `Gemfile`:
```shell
bundle update --source {{nome_da_gema}}
```
#### Criar o esqueleto do projeto de uma nova gema:
```shell
bundle gem {{nome_da_gema}}
```
{% endraw %}{% raw %}
<h2 id="bzip2">
  <a href="/pt_br/common/bzip2.html">bzip2</a> <a href="#bzip2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compressor de arquivos que utiliza o algoritmo Burrows–Wheeler.

#### Compactar um arquivo:
```shell
bzip2 {{arquivo}}
```
#### Descompactar um arquivo:
```shell
bzip2 -d {{arquivo.bz2}}
```
#### Descompactar um arquivo exibindo o conteúdo no terminal:
```shell
bzip2 -dc {{arquivo.bz2}}
```
{% endraw %}{% raw %}
<h2 id="cat">
  <a href="/pt_br/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe e concatena o conteúdo de arquivos.
> Mais informações: <https://www.gnu.org/software/coreutils/cat>.

#### Exibir o conteúdo de um arquivo no terminal:
```shell
cat {{arquivo}}
```
#### Concatenar o conteúdo de vários arquivos em um arquivo de destino:
```shell
cat {{arquivo1}} {{arquivo2}} > {{arquivo_de_destino}}
```
#### Adicionar o conteúdo de vários arquivos ao final de um arquivo de destino:
```shell
cat {{arquivo1}} {{arquivo2}} >> {{arquivo_de_destino}}
```
#### Exibir o conteúdo de um arquivo no terminal numerando as linhas:
```shell
cat -n {{arquivo}}
```
{% endraw %}{% raw %}
<h2 id="clear">
  <a href="/pt_br/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Limpa a tela do terminal.
> Mais informações: <https://manned.org/clear>.

#### Limpar a tela (equivalente a apertar Control-L no terminal Bash):
```shell
clear
```
#### Limpar a tela mantendo o buffer de rolagem do terminal:
```shell
clear -x
```
#### Especificar o tipo de terminal a ser limpado (por padrão é o valor da variável de ambiente `TERM`):
```shell
clear -T {{tipo_do_terminal}}
```
#### Mostra a versão do `ncurses` usado pelo `clear`:
```shell
clear -V
```
{% endraw %}{% raw %}
<h2 id="clj">
  <a href="/pt_br/common/clj.html">clj</a> <a href="#clj"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de Clojure para iniciar um REPL ou invocar uma função com argumentos.
> Todas as opções podem ser definidas em um arquivo `deps.edn`.
> Mais informações: <https://clojure.org/guides/deps_and_cli>.

#### Inicia um REPL:
```shell
clj
```
#### Executa uma função:
```shell
clj -X {{namespace/function_name}}
```
#### Executa a função principal (*main*) do *namespace* especificado:
```shell
clj -M -m {{namespace}} {{args}}
```
#### Prepara um projeto resolvendo dependências, baixando bibliotecas, e criando / cacheando *classpaths*:
```shell
clj -P
```
#### Inicia um servidor nREPL com o *middleware* CIDER:
```shell
clj -Sdeps '{:deps {nrepl {:mvn/version "0.7.0"} cider/cider-nrepl {:mvn/version "0.25.2"}}}' -m nrepl.cmdline --middleware '["cider.nrepl/cider-middleware"]' --interactive
```
#### Inicia um REPL para ClojureScript e abre um navegador web:
```shell
clj -Sdeps '{:deps {org.clojure/clojurescript {:mvn/version "1.10.758"}}}' --main cljs.main --repl
```
{% endraw %}{% raw %}
<h2 id="code">
  <a href="/pt_br/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> Mais informações: <https://github.com/microsoft/vscode>.

#### Abrir o VS Code:
```shell
code
```
#### Abrir o diretório atual no VS Code:
```shell
code .
```
#### Abrir um arquivo ou diretório no VS Code:
```shell
code {{caminho/para/arquivo-ou-diretório}}
```
#### Abrir um arquivo ou diretório numa janela já aberta do VS Code:
```shell
code --reuse-window {{caminho/para/arquivo-ou-diretório}}
```
#### Comparar o conteúdo de dois arquivos no VS Code:
```shell
code -d {{arquivo1}} {{arquivo2}}
```
#### Iniciar o VS Code com permissão de super usuário (sudo):
```shell
sudo code {{path/to/file_or_directory}} --user-data-dir
```
{% endraw %}{% raw %}
<h2 id="command">
  <a href="/pt_br/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Obriga o shell a executar o programa, ignorando qualquer função ou alias com o mesmo nome.
> Mais informações: <https://manned.org/command>.

#### Executar o programa ls, mesmo que exista algum alias ls:
```shell
command {{ls}}
```
{% endraw %}{% raw %}
<h2 id="convert">
  <a href="/pt_br/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de conversão de imagens da ImageMagick.
> Mais informações: <https://imagemagick.org/script/convert.php>.

#### Converter uma imagem do formato JPG para o formato PNG:
```shell
convert {{imagem.jpg}} {{imagem.png}}
```
#### Escalar uma imagem para 50% do seu tamanho original:
```shell
convert {{imagem.png}} -resize 50% {{nova_imagem.png}}
```
#### Escalar uma imagem, mantendo as suas proporções originais, para uma dimensão máxima de 640x480:
```shell
convert {{imagem.png}} -resize 640x480 {{nova_imagem.png}}
```
#### Juntar várias imagens horizontalmente:
```shell
convert {{imagem1.png}} {{imagem2.png}} {{imagem3.png}} +append {{nova_imagem.png}}
```
#### Criar um GIF a partir de uma série de imagens, com um intervalo de 100ms entre elas:
```shell
convert {{imagem1.png}} {{imagem2.png}} {{imagem3.png}} -delay {{100}} {{nova_imagem.gif}}
```
#### Criar uma nova imagem de tamanho 800x600 com apenas um fundo sólido vermelho:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{imagem.png}}
```
{% endraw %}{% raw %}
<h2 id="curl">
  <a href="/pt_br/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transfere dados entre o computador local e um servidor remoto.
> Suporta a maioria dos protocolos de comunicação, incluindo HTTP, FTP e POP3.
> Mais informações: <https://curl.se>.

#### Descarregar os conteúdos de um URL para um arquivo:
```shell
curl {{http://example.com}} --output {{arquivo}}
```
#### Descarregar um arquivo, gravando o resultado sob o nome do arquivo indicado pelo URL:
```shell
curl --remote-name {{http://example.com/arquivo}}
```
#### Descarregar um arquivo, seguindo redirecionamentos e automaticamente continuando transferências idênticas que tenham sido interrompidas:
```shell
curl --remote-name --location --continue-at - {{http://example.com/arquivo}}
```
#### Enviar dados codificados por formulário (pedido POST do tipo `application/x-www-form-urlencoded`):
```shell
curl --data {{'nome=maria'}} {{http://example.com/formulario}}
```
#### Enviar um pedido com um cabeçalho adicional, usando um método HTTP personalizado:
```shell
curl --header {{'X-Meu-Cabecalho: 123'}} --request {{PUT}} {{http://example.com}}
```
#### Enviar dados no formato JSON, especificando o cabeçalho de tipo de conteúdo (content-type) apropriado:
```shell
curl --data {{'{"nome":"maria"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/usuarios/123}}
```
#### Passar ao pedido o nome de usuário e senha para autenticação no servidor:
```shell
curl -u usuario:senha {{http://example.com}}
```
#### Passar ao pedido o certificado do cliente e a chave para um recurso, omitindo a validação do certificado:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://example.com}}
```
{% endraw %}{% raw %}
<h2 id="docker-build">
  <a href="/pt_br/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cria uma imagem a partir de um Dockerfile.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Cria uma imagem docker usando o Dockerfile presente no diretório atual:
```shell
docker build .
```
#### Cria uma imagem docker usando o Dockerfile de uma URL específica:
```shell
docker build {{github.com/creack/docker-firefox}}
```
#### Cria uma imagem docker e cria uma tag para ela:
```shell
docker build --tag {{nome:tag}} .
```
#### Não usa o cache na criação da imagem:
```shell
docker build --no-cache --tag {{nome:tag}} .
```
#### Cria uma imagem docker usando um Dockerfile específico:
```shell
docker build --file {{Dockerfile}} .
```
#### Cria uma imagem docker utilizando variáveis customizadas para a criação de imagens:
```shell
docker build --build-arg {{PROXY_DO_HTTP=http://10.20.30.2:1234}} --build-arg {{PROXY_DO_FTP=http://40.50.60.5:4567}} .
```
{% endraw %}{% raw %}
<h2 id="docker-images">
  <a href="/pt_br/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia imagens Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Lista todas as imagens Docker:
```shell
docker images
```
#### Lista todas as imagens Docker incluíndo imagens intermedirárias:
```shell
docker images --all
```
#### Lista no modo silencioso (somente IDs numéricos):
```shell
docker images --quiet
```
#### Lista todas as imagens Docker não usadas por nenhum container:
```shell
docker images --filter dangling=true
```
#### Lista imagens que contenham um substring no seu nome:
```shell
docker images "{{*nome*}}"
```
{% endraw %}{% raw %}
<h2 id="docker-logs">
  <a href="/pt_br/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe os logs dos containers.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Exibe logs de um container:
```shell
docker logs {{nome_do_container}}
```
#### Exibe logs de um container e segue exibindo:
```shell
docker logs -f {{nome_do_container}}
```
#### Exibe as últimas 5 linhas:
```shell
docker logs {{nome_do_container}} --tail {{5}}
```
#### Exibe logs e adiciona a informação de hora ao log:
```shell
docker logs -t {{nome_do_container}}
```
#### Exibe logs até um certo ponto no tempo de execução do container (por exemplo: 23m, 10s, 2013-01-02T13:23:37):
```shell
docker logs {{nome_do_container}} --until {{tempo}}
```
{% endraw %}{% raw %}
<h2 id="docker-ps">
  <a href="/pt_br/common/docker-ps.html">docker ps</a> <a href="#docker-ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lista os containers Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/ps/>.

#### Lista containers docker em execução:
```shell
docker ps
```
#### Lista todos containers docker (em execução e parados):
```shell
docker ps --all
```
#### Lista os últimos containers criados (incluí todos os estados):
```shell
docker ps --latest
```
#### Filtra os containers que contém uma substring no seu nome:
```shell
docker ps --filter="name={{nome}}"
```
#### Filtra todos os containers que possuem uma imagem antepassada:
```shell
docker ps --filter "ancestor={{imagem}}:{{tag}}"
```
#### Filtra containers que tenha o código de saída:
```shell
docker ps --all --filter="exited={{código}}"
```
#### Filtra containers por estado (criado, execução, removendo, pausado, finalizado e morto):
```shell
docker ps --filter="status={{estado}}"
```
#### Filtra containers que contenham um volume específico ou montado em um caminho específico:
```shell
docker ps --filter="volume={{caminho/para/diretório}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"
```
{% endraw %}{% raw %}
<h2 id="docker-run">
  <a href="/pt_br/common/docker-run.html">docker run</a> <a href="#docker-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executa um comando em um novo container Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/run/>.

#### Executa um comando em um novo container de uma imagem tagueada:
```shell
docker run {{imagem:tag}} {{comando}}
```
#### Executa um comando em um novo container em background e exibe o ID:
```shell
docker run -d {{image}} {{command}}
```
#### Executa um comando em um novo container que será removido após a execução em um modo interativo e com um terminal TTY:
```shell
docker run --rm -it {{image}} {{command}}
```
#### Executa um comando em um novo container com variáveis de ambiente:
```shell
docker run -e '{{variável}}={{valor}}' -e {{variável}} {{imagem}} {{comando}}
```
#### Executa um comando em um novo container montando volumes nos caminhos específicos:
```shell
docker run -v {{caminho/no/host_local}}:{{caminho/no/container}} {{imagem}} {{comando}}
```
#### Executa um comando em um novo container e abre as portas para acesso:
```shell
docker run -p {{porta_do_host_local}}:{{porta_do_container}} {{imagem}} {{comando}}
```
{% endraw %}{% raw %}
<h2 id="docker-start">
  <a href="/pt_br/common/docker-start.html">docker start</a> <a href="#docker-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inicia um ou mais containers parados.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/start/>.

#### Exibe a ajuda:
```shell
docker start
```
#### Inicia um container docker:
```shell
docker start {{container}}
```
#### Inicia um container, atachando ao terminal os sinais stdout e stderr e outros sinais:
```shell
docker start --attach {{container}}
```
#### Inicia um ou mais containers com ID separados por espaço:
```shell
docker start {{container(s)}}
```
{% endraw %}{% raw %}
<h2 id="docker">
  <a href="/pt_br/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de containers e imagens Docker.
> Mais informações: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Listar os containers Docker que se encontram em execução:
```shell
docker ps
```
#### Listar todos os containers Docker:
```shell
docker ps -a
```
#### Inicializar um container com um nome personalizado a partir de uma imagem:
```shell
docker run --name {{nome_container}} {{imagem}}
```
#### Começar ou parar um container existente:
```shell
docker {{start|stop}} {{nome_container}}
```
#### Extrair uma imagem a partir de um Docker Registry:
```shell
docker pull {{imagem}}
```
#### Abrir um terminal dentro de um container em execução:
```shell
docker exec -it {{nome_container}} {{sh}}
```
#### Remover um container parado:
```shell
docker rm {{nome_container}}
```
#### Obter e acompanhar o histórico de um container:
```shell
docker logs -f {{nome_container}}
```
{% endraw %}{% raw %}
<h2 id="doxygen">
  <a href="/pt_br/common/doxygen.html">doxygen</a> <a href="#doxygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um sistema de documentação para várias linguagens de programação.
> Mais informações: <http://www.doxygen.nl>.

#### Gerar um arquivo de configuração padrão (Doxyfile):
```shell
doxygen -g
```
#### Gerar um arquivo de configuração, especificando o nome do arquivo de configuração:
```shell
doxygen -g {{caminho/para/arquivo_configuração}}
```
#### Gerar documentação utilizando um arquivo de configuração existente:
```shell
doxygen {{caminho/para/arquivo_configuração}}
```
{% endraw %}{% raw %}
<h2 id="gplusplus">
  <a href="/pt_br/common/g++.html">gplusplus</a> <a href="#gplusplus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compilador de arquivos de código fonte C++.
> Parte do GCC (GNU Compiler Collection).
> Mais informações: <https://gcc.gnu.org>.

#### Compilar um arquivo de código fonte para um binário executável:
```shell
g++ {{arquivo_fonte.cpp}} -o {{arquivo_executável}}
```
#### Compilar mostrando todos os erros e avisos:
```shell
g++ {{arquivo_fonte.cpp}} -Wall -o {{arquivo_executável}}
```
#### Compilar utilizando um padrão específico da linguagem (C++98/C++11/C++14/C++17):
```shell
g++ {{arquivo_fonte.cpp}} -std={{standard_linguagem}} -o {{arquivo_executável}}
```
#### Compilar incluindo bibliotecas localizadas em um local diferente do arquivo de código fonte:
```shell
g++ {{arquivo_fonte.cpp}} -o {{arquivo_executável}} -I{{caminho/para/header}} -L{{caminho/para/biblioteca}} -l{{nome_biblioteca}}
```
{% endraw %}{% raw %}
<h2 id="gcc">
  <a href="/pt_br/common/gcc.html">gcc</a> <a href="#gcc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compilador de arquivos de código fonte C e C++, efetuando também as fases de pré-processamento, assembling e linking.
> Mais informações: <https://gcc.gnu.org>.

#### Compilar múltiplos arquivos de código fonte, produzindo um arquivo executável:
```shell
gcc {{arquivo_fonte1.c}} {{arquivo_fonte2.c}} -o {{arquivo_executável}}
```
#### Habilitar avisos durante a compilação:
```shell
gcc {{arquivo_fonte.c}} -Wall -Og -o {{arquivo_executável}}
```
#### Incluir bibliotecas de um local diferente:
```shell
gcc {{arquivo_fonte.c}} -o {{arquivo_executável}} -I{{caminho/para/header}} -L{{caminho/para/biblioteca}} -l{{nome_biblioteca}}
```
#### Compilar o código fonte para instruções Assembler:
```shell
gcc -S {{arquivo_fonte.c}}
```
#### Compilar o código fonte sem efetuar a fase de linking:
```shell
gcc -c {{arquivo_fonte.c}}
```
{% endraw %}{% raw %}
<h2 id="gdb">
  <a href="/pt_br/common/gdb.html">gdb</a> <a href="#gdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> O depurador GNU.
> Mais informações: <https://www.gnu.org/software/gdb>.

#### Depurar um executável:
```shell
gdb {{executável}}
```
#### Vincular um processo ao gdb:
```shell
gdb -p {{PID}}
```
#### Depurar usando um arquivo de "core dump":
```shell
gdb -c {{core}} {{executável}}
```
#### Executa um dado comando do gdb ao iniciar:
```shell
gdb -ex "{{comandos}}" {{executável}}
```
#### Inicia o gdb passando argumentos para o executável:
```shell
gdb --args {{executável}} {{argumento1}} {{argumento2}}
```
{% endraw %}{% raw %}
<h2 id="git-add">
  <a href="/pt_br/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adiciona arquivos modificados na área de preparação.
> Mais informações: <https://git-scm.com/docs/git-add>.

#### Adiciona um arquivo na área de preparação:
```shell
git add {{caminho/do/arquivo}}
```
#### Adiciona todos arquivos (rastreados ou não):
```shell
git add -A
```
#### Adiciona apenas arquivos rastreados:
```shell
git add -u
```
#### Adiciona arquivos ignorados:
```shell
git add -f
```
#### Interativamente adiciona partes dos arquivo:
```shell
git add -p
```
#### Interativamente adiciona partes de um dado arquivo:
```shell
git add -p {{caminho/para/arquivo}}
```
#### Interativamente adiciona arquivos ou partes modificadas:
```shell
git add -i
```
{% endraw %}{% raw %}
<h2 id="git-mv">
  <a href="/pt_br/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move ou renomeia arquivos e atualiza o index do Git.
> Mais informações: <https://git-scm.com/docs/git-mv>.

#### Move arquivos dentro de um repositório e adiciona no próximo commit:
```shell
git mv {{caminho/para/arquivo}} {{novo/caminho}}
```
#### Renomeia um arquivo e adiciona a renomeação no próximo commit:
```shell
git mv {{nome_do_arquivo}} {{novo_nome}}
```
#### Sobrescreve o arquivo no caminho alvo se ele já existir:
```shell
git mv --force {{arquivo}} {{alvo}}
```
{% endraw %}{% raw %}
<h2 id="git-remote">
  <a href="/pt_br/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia repositórios monitorados ("remotes").
> Mais informações: <https://git-scm.com/docs/git-remote>.

#### Mostre uma lista de remotes existentes, seus nomes e URL:
```shell
git remote -v
```
#### Mostra infomação de um remote específico:
```shell
git remote show {{nome_do_remote}}
```
#### Adiciona um remote:
```shell
git remote add {{nome_do_remote}} {{url_do_remote}}
```
#### Muda a URL de um remote (use `--add` para manter a URL existente):
```shell
git remote set-url {{nome_do_remote}} {{nova_url}}
```
#### Remove um remote:
```shell
git remote remove {{nome_do_remote}}
```
#### Renomeia um remote:
```shell
git remote rename {{nome_antigo}} {{novo_nome}}
```
{% endraw %}{% raw %}
<h2 id="git">
  <a href="/pt_br/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sistema de versionamento distribuído.
> Mais informações: <https://git-scm.com>.

#### Verifique a versão do Git:
```shell
git --version
```
#### Mostre ajuda geral:
```shell
git --help
```
#### Mostre ajuda de um subcomando do Git (como `commit`, `log`, etc.):
```shell
git help {{subcomando}}
```
#### Execute um subcomando Git:
```shell
git {{subcomando}}
```
#### Execute um subcomando Git no caminho raíz de um repositório específico:
```shell
git -C {{caminho/para/repo}} {{subcomando}}
```
#### Execute um subcomando Git com uma dada configuração:
```shell
git -c '{{config.chave}}={{valor}}' {{subcomando}}
```
{% endraw %}{% raw %}
<h2 id="gpg">
  <a href="/pt_br/common/gpg.html">gpg</a> <a href="#gpg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard.
> Mais informações: <https://gnupg.org>.

#### Assina doc.txt, sem criptografá-lo (cria um arquivo de saída doc.txt.asc):
```shell
gpg --clearsign {{doc.txt}}
```
#### Criptografa doc.txt para alice@example.com (cria um arquivo de saída `doc.txt.gpg`):
```shell
gpg --encrypt --recipient {{alice@example.com}} {{doc.txt}}
```
#### Criptografa doc.txt apenas com uma senha simétrica (cria um arquivo de sadída `doc.txt.gpg`):
```shell
gpg --symmetric {{doc.txt}}
```
#### Descriptografa doc.txt.gpg (envia saída para stdout):
```shell
gpg --decrypt {{doc.txt.gpg}}
```
#### Importa uma chave pública:
```shell
gpg --import {{public.gpg}}
```
#### Exporta a chave pública da alice@example.com (envia saída para stdout):
```shell
gpg --export --armor {{alice@example.com}}
```
#### Exporta chave privada da alice@example.com (envia saída para stdout):
```shell
gpg --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}{% raw %}
<h2 id="gzip">
  <a href="/pt_br/common/gzip.html">gzip</a> <a href="#gzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de compactação de arquivos com compressão gzip.
> Mais informações: <https://www.gnu.org/software/gzip/manual/gzip.html>.

#### Alterar compressão de um arquivo compactado com compressão gzip:
```shell
gzip {{arquivo.ext}}
```
#### Descompactar arquivo gzip definindo arquivo final:
```shell
gzip -c -d {{arquivo.ext}}.gz > {{arquivo_descompactado.ext}}
```
#### Compactar arquivo definindo arquivo final:
```shell
gzip -c {{arquivo.ext}} > {{arquivo_compactado.ext.gz}}
```
#### Compactando arquivos em gzip definindo o nível de compressão [9]:
```shell
gzip -{{9}} -c {{arquivo.ext}} > {{arquivo_compactado.ext.gz}}
```
{% endraw %}{% raw %}
<h2 id="helm">
  <a href="/pt_br/common/helm.html">helm</a> <a href="#helm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helm é um gerenciador de pacores para Kubernetes.
> Mais informações: <https://helm.sh/>.

#### Cria um chart do helm:
```shell
helm create {{nome_do_chart}}
```
#### Adiciona um novo repositório helm:
```shell
helm repo add {{nome_do_repositório}}
```
#### Lista os repositórios helm:
```shell
helm repo list
```
#### Atualiza os repositórios helm:
```shell
helm repo update
```
#### Remova um repositório helm:
```shell
helm repo remove {{nome_do_repositório}}
```
#### Instala um chart helm:
```shell
helm install {{nome_do_repositório}}/{{nome_do_chart}}
```
#### Obtém um chart helm chart como um arquivo tar:
```shell
helm get {{nome_do_release_do_chart}}
```
#### Atualiza as dependências helm:
```shell
helm dependency update
```
{% endraw %}{% raw %}
<h2 id="htop">
  <a href="/pt_br/common/htop.html">htop</a> <a href="#htop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visualizar informação dinâmica em tempo real acerca de processos em execução. Uma versão melhorada do comando `top`.

#### Inicializar htop:
```shell
htop
```
#### Inicializar htop mostrando somente processos pertencentes a um usuário:
```shell
htop -u {{nome_usuário}}
```
#### Obter ajuda acerca de comandos interativos:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="jar">
  <a href="/pt_br/common/jar.html">jar</a> <a href="#jar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compactador de Bibliotecas e Aplicações Java.
> Mais informações: <https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

#### Arquiva recursivamente todos os arquivos do diretório atual em um arquivo .jar:
```shell
jar cf {{arquivo.jar}} *
```
#### Descompacta o arquivo .jar/.war para o diretório atual:
```shell
jar -xvf {{arquivo.jar}}
```
#### Lista o conteúdo do arquivo .jar/.war:
```shell
jar tf {{caminho/para/arquivo.jar}}
```
#### Lista o conteúdo do arquivo .jar/.war com mais detalhes (verbose):
```shell
jar tvf {{caminho/para/arquivo.jar}}
```
{% endraw %}{% raw %}
<h2 id="kill">
  <a href="/pt_br/common/kill.html">kill</a> <a href="#kill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Envia um sinal para um processo, geralmente para finalizar o processo.
> Todos os sinais exceto pelo SIGKILL e SIGSTOP podem ser interceptados pelo processo para finalizar de forma limpa.

#### Finaliza um programa usando o sinal default SIGTERM (terminate):
```shell
kill {{id_do_processo}}
```
#### Lista todos os nomes dos sinais disponíveis (para serem usados sem o prefixo `SIG`):
```shell
kill -l
```
#### Finaliza um processo em background:
```shell
kill %{{id_do_processo}}
```
#### Finaliza um programa usando o sinal SIGHUP. Muitos daemons vão recarregar ao invés de finalizar:
```shell
kill -{{1|HUP}} {{id_do_processo}}
```
#### Finaliza um programa usando o sinal SIGINT (interrupt). Isto é tipicamente iniciado pelo usuário ao pressionar `Ctrl + C`:
```shell
kill -{{2|INT}} {{id_do_processo}}
```
#### Envia sinal para o sistema operacional para finalizar imediatamente o programa (quem não tem chance de capturar o sinal):
```shell
kill -{{9|KILL}} {{id_do_processo}}
```
#### Envia sinal para o sistema operacional para pausar o programa até um sinal SIGCONT ("continue") seja recebido:
```shell
kill -{{17|STOP}} {{id_do_processo}}
```
#### Envia um sinal `SIGUSR1` para todos os processos de um dado GID (group id):
```shell
kill -{{SIGUSR1}} -{{id_do_grupo}}
```
{% endraw %}{% raw %}
<h2 id="kubectl">
  <a href="/pt_br/common/kubectl.html">kubectl</a> <a href="#kubectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Linha de comando para executar comando em clusters do Kubernetes.
> Mais informações: <https://kubernetes.io/docs/reference/kubectl/>.

#### Lista toda a informação sobre um recurso em detalhes:
```shell
kubectl get {{pod|service|deployment|ingress|...}} -o wide
```
#### Atualiza um pod específico com o label 'unhealthy' e o valor 'true':
```shell
kubectl label pods {{name}} unhealthy=true
```
#### Lista todos os recursos de diferentes tipos:
```shell
kubectl get all
```
#### Exibe os usos de recursos (CPU/Memória/Espaço alocado) dos nós ou pods:
```shell
kubectl top {{pod|node}}
```
#### Exibe os endereços dos serviços do master e do cluster:
```shell
kubectl cluster-info
```
#### Exibe uma explicação de um campo específico:
```shell
kubectl explain {{pods.spec.containers}}
```
#### Exibe os logs de um container em um pod ou de um recurso específico:
```shell
kubectl logs {{pod_name}}
```
#### Executa um comando em um pod existente:
```shell
kubectl exec {{pod_name}} -- {{ls /}}
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/pt_br/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Listar o conteúdo de um diretório.
> Mais informações: <https://www.gnu.org/software/coreutils/ls>.

#### Listar todos os arquivos, apresentando um arquivo por linha:
```shell
ls -1
```
#### Listar todos os arquivos, incluindo arquivos ocultos:
```shell
ls -a
```
#### Listar todos os arquivos, exibindo permissões, propriedade, tamanho e data de modificação:
```shell
ls -la
```
#### Listar todos os arquivos, apresentando o tamanho em medidas legíveis por humanos (KiB, MiB, GiB):
```shell
ls -lh
```
#### Listar todos os arquivos ordenados por tamanho (descendente):
```shell
ls -lS
```
#### Listar todos os arquivos ordenados por data de modificação (mais antigos primeiro):
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="lsof">
  <a href="/pt_br/common/lsof.html">lsof</a> <a href="#lsof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lista arquivos abertos e os seus processos correspondentes.
> Nota: Privilégios de administrador (ou sudo) são necessários para listar arquivos abertos por outros.

#### Localizar os processos que têm um certo arquivo aberto:
```shell
lsof {{caminho/para/arquivo}}
```
#### Localizar o processo que abriu uma porta de internet local:
```shell
lsof -i :{{porta}}
```
#### Mostrar o ID (PID) do processo que abriu um arquivo especificado:
```shell
lsof -t {{caminho/para/arquivo}}
```
#### Listar arquivos abertos por um certo usuário:
```shell
lsof -u {{nome_usuario}}
```
#### Listar arquivos abertos por um certo comando ou processo:
```shell
lsof -c {{nome_processo_ou_comando}}
```
#### Listar arquivos abertos por um certo processo, dado o seu PID:
```shell
lsof -p {{PID}}
```
#### Listar arquivos abertos em um diretório:
```shell
lsof +D {{caminho/para/diretório}}
```
#### Encontrar o processo que está ouvindo uma porta de TCP local:
```shell
lsof -iTCP:{{porta}} -sTCP:LISTEN
```
{% endraw %}{% raw %}
<h2 id="man">
  <a href="/pt_br/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para exibir páginas do manual.
> Mais informações: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Visualizar o manual de um comando:
```shell
man {{comando}}
```
#### Visualizar a página da seção 7 do manual de um comando:
```shell
man {{comando}}.{{7}}
```
#### Visualizar o caminho procurado pelas páginas do manual:
```shell
man --path
```
#### Visualizar o caminho do manual de um comando:
```shell
man -w {{comando}}
```
#### Procurar manuais contendo um termo de pesquisa:
```shell
man -k "{{termo_de_pesquisa}}"
```
{% endraw %}{% raw %}
<h2 id="meteor">
  <a href="/pt_br/common/meteor.html">meteor</a> <a href="#meteor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plataforma Full-Stack de JavaScript para desenvolver aplicações web.
> Mais informações: <https://meteor.com>.

#### Executar um projeto meteor a partir do seu diretório base em modo de desenvolvimento:
```shell
meteor
```
#### Criar um novo projeto em um diretório específico:
```shell
meteor create {{caminho/para/diretório}}
```
#### Listar todos os pacotes usados pelo projeto:
```shell
meteor list
```
#### Adicionar um pacote ao projeto:
```shell
meteor add {{nome_pacote}}
```
#### Remover um pacote do projeto:
```shell
meteor remove {{nome_pacote}}
```
#### Criar uma build de produção do projeto, no formato tarball, em um diretório específico:
```shell
meteor build {{caminho/para/diretório}}
```
{% endraw %}{% raw %}
<h2 id="mongo">
  <a href="/pt_br/common/mongo.html">mongo</a> <a href="#mongo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cliente shell interativo de MongoDB.
> Mais informações: <https://docs.mongodb.com/manual/reference/program/mongo>.

#### Conectar a uma base de dados:
```shell
mongo {{base_de_dados}}
```
#### Conectar a uma base de dados em um host e porta específicos:
```shell
mongo --host {{host}} --port {{porta}} {{base_de_dados}}
```
#### Conectar a uma base de dados com um usuário específico, uma senha será pedida ao usuário:
```shell
mongo --username {{usuário}} {{base_de_dados}} --password
```
#### Avaliar JavaScript na base de dados:
```shell
mongo --eval '{{JSON.stringify(db.foo.findOne())}}' {{base_de_dados}}
```
{% endraw %}{% raw %}
<h2 id="mvn">
  <a href="/pt_br/common/mvn.html">mvn</a> <a href="#mvn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta para a criação e gerenciamento de projetos Java.
> Mais informações: <https://maven.apache.org/>.

#### Compilar um projeto:
```shell
mvn compile
```
#### Criar um artefato de distribuição utilizando o formato espeficado no `pom.xml`, por exemplo o formato `jar`:
```shell
mvn package
```
#### Criar um artefato de distribuição sem executar testes unitários:
```shell
mvn package -Dmaven.test.skip=true
```
#### Instalar um artefato gerado em um repositório local:
```shell
mvn install
```
#### Apagar artefatos gerados no diretório `target`:
```shell
mvn clean
```
#### Executar as fases `clean` e `package` em um projeto:
```shell
mvn clean package
```
#### Executar as fases `clean` e `package` em um projeto utilizando um perfil:
```shell
mvn clean -P{{perfil}} package
```
#### Executar uma classe que possua o método `main`:
```shell
mvn exec:java -Dexec.mainClass="{{nome.do.pacote.classe}}" -Dexec.args="{{arg1 arg2}}"
```
{% endraw %}{% raw %}
<h2 id="mysql">
  <a href="/pt_br/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A ferramenta de linha de comando do MySQL.
> Mais informações: <https://www.mysql.com/>.

#### Conectar a um banco de dados:
```shell
mysql {{nome_do_banco_de_dados}}
```
#### Conectar a um banco de dados (será solicitada a senha de acesso do usuário):
```shell
mysql -u {{usuário}} --password {{nome_do_banco_de_dados}}
```
#### Conectar a um banco de dados disponível em um endereço específico:
```shell
mysql -h {{endereco_do_banco_de_dados}} {{nome_do_banco_de_dados}}
```
#### Conectar a um banco de dados utilizando um socket Unix:
```shell
mysql --socket {{caminho/para/socket.sock}}
```
#### Executar todos os comandos de um arquivo SQL em um banco de dados:
```shell
mysql -e "source {{nome_do_arquivo.sql}}" {{nome_do_banco_de_dados}}
```
{% endraw %}{% raw %}
<h2 id="mysqldump">
  <a href="/pt_br/common/mysqldump.html">mysqldump</a> <a href="#mysqldump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Realizar e restaurar backups no MySQL.
> Mais informações: <https://dev.mysql.com/doc/refman/en/mysqldump.html>.

#### Criar o backup do banco de dados em arquivo de saída (será solicitada a senha de acesso do usuário):
```shell
mysqldump -u {{usuário}} --password {{nome_do_banco_de_dados}} -r {{arquivo_de_saida.sql}}
```
#### Restaurar o conteúdo contido no arquivo de backup em banco de dados específico (será solicitada a senha de acesso do usuário):
```shell
mysql -u {{usuário}} --password -e "source {{arquivo_de_backup.sql}}" {{nome_do_banco_de_dados}}
```
{% endraw %}{% raw %}
<h2 id="nativefier">
  <a href="/pt_br/common/nativefier.html">nativefier</a> <a href="#nativefier"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para criação de aplicativos para desktop à partir de web sites.
> Mais informações: <https://github.com/jiahaog/nativefier>.

#### Gerar aplicativo desktop para site:
```shell
nativefier {{url}}
```
#### Gerar aplicativo desktop com nome customizado:
```shell
nativefier --name {{nome}} {{url}}
```
#### Gerar aplicativo desktop usando um ícone PNG customizado:
```shell
nativefier --icon {{caminho/para/icone.png}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="node">
  <a href="/pt_br/common/node.html">node</a> <a href="#node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plataforma de JavaScript para o lado do Servidor (Node.js).
> Mais informações: <https://nodejs.org>.

#### Executar um arquivo JavaScript:
```shell
node {{arquivo}}.js
```
#### Inicializar a REPL (shell interativa):
```shell
node
```
#### Executar JavaScript, passando-o no comando:
```shell
node -e "{{código}}"
```
#### Executar um arquivo JavaScript, imprimindo o resultado:
```shell
node -p "{{script}}"
```
{% endraw %}{% raw %}
<h2 id="pdftk">
  <a href="/pt_br/common/pdftk.html">pdftk</a> <a href="#pdftk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Conjunto de utilitários para manipular arquivos PDF.
> Mais informações: <https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit>.

#### Extrair conjuntos de páginas de um arquivo PDF (páginas 1 a 3, 5 e 6 a 10) e guardá-las num novo arquivo:
```shell
pdftk {{arquivo.pdf}} cat {{1-3 5 6-10}} output {{novo_arquivo.pdf}}
```
#### Concatenar uma lista de arquivos PDF, guardando o resultado num novo arquivo:
```shell
pdftk {{arquivo1.pdf arquivo2.pdf arquivoN.pdf ...}} cat output {{novo_arquivo.pdf}}
```
#### Partir cada página de um arquivo PDF num arquivo separado, com um padrão para o nome dos novos arquivos:
```shell
pdftk {{arquivo.pdf}} burst output {{página_%d.pdf}}
```
#### Girar em 180° todas as páginas de um arquivo PDF:
```shell
pdftk {{arquivo.pdf}} cat {{1-endsouth}} output {{novo_arquivo.pdf}}
```
#### Girar a terceira página de um arquivo PDF em 90° no sentido horário, não modificando as restantes:
```shell
pdftk {{arquivo.pdf}} cat {{1-2 3east 4-end}} output {{novo_arquivo.pdf}}
```
{% endraw %}{% raw %}
<h2 id="rails-generate">
  <a href="/pt_br/common/rails-generate.html">rails generate</a> <a href="#rails-generate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerar artefatos Rails a partir de um modelo em um projeto existente.

#### Exibir todos os geradores disponíveis:
```shell
rails generate
```
#### Criar um modelo:
```shell
rails generate model {{nome_da_classe}}
```
#### Criar um controlador:
```shell
rails generate controller {{nome_do_controlador}}
```
#### Criar uma estrutura completa (modelo, controlador, testes, etc.) para um novo modelo:
```shell
rails generate scaffold {{nome_do_modelo}}
```
{% endraw %}{% raw %}
<h2 id="rails">
  <a href="/pt_br/common/rails.html">rails</a> <a href="#rails"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Framework MVC para o desenvolvimento de aplicações web, desenvolvido em Ruby.
> Mais informações: <https://guides.rubyonrails.org/command_line.html>.

#### Criar um novo projeto:
```shell
rails new "{{nome_do_projeto}}"
```
#### Iniciar o servidor local para o projeto atual na porta 3000:
```shell
rails server
```
#### Iniciar o servidor local para o projeto atual em um porta específica:
```shell
rails server -p "{{porta}}"
```
#### Iniciar o console Rails para manipular o projeto atual utilizando o terminal:
```shell
rails console
```
#### Verificar a versão atual do Rails:
```shell
rails --version
```
{% endraw %}{% raw %}
<h2 id="rbenv">
  <a href="/pt_br/common/rbenv.html">rbenv</a> <a href="#rbenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que facilita a instalação e gerenciamento de múltiplas versões da linguagem Ruby.

#### Instalar uma ou mais versões, separadas por espaço:
```shell
rbenv install {{uma_ou_mais_versoes}}
```
#### Exibir a lista de versões instaladas:
```shell
rbenv versions
```
#### Determinar uma versão específica para ser a instalação padrão:
```shell
rbenv global {{versao}}
```
#### Determinar uma versão específica para um projeto. Este comando deve ser executado no diretório do projeto:
```shell
rbenv local {{versao}}
```
#### Exibir a versão ativa:
```shell
rbenv version
```
#### Remover uma versão:
```shell
rbenv uninstall {{versao}}
```
#### Exibir todas as versões que contém um determinado executável:
```shell
rbenv whence {{executavel}}
```
{% endraw %}{% raw %}
<h2 id="rvm">
  <a href="/pt_br/common/rvm.html">rvm</a> <a href="#rvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que facilita a instalação e gerenciamento de múltiplas versões da linguagem Ruby.

#### Instalar uma ou mais versões separadas por espaço:
```shell
rvm install {{uma_ou_mais_versoes}}
```
#### Exibir a lista de versões instaladas:
```shell
rvm list
```
#### Definir uma versão específica para ser utilizada temporariamente:
```shell
rvm use {{versao}}
```
#### Definir uma versão específica para ser a instalação padrão:
```shell
rvm --default use {{versao}}
```
#### Atualizar uma versão já instalada para uma nova versão:
```shell
rvm upgrade {{versao_atual}} {{nova_versao}}
```
#### Remover uma versão mantendo o código fonte:
```shell
rvm uninstall {{versao}}
```
#### Remover uma versão e o código fonte:
```shell
rvm remove {{versao}}
```
#### Exibir as dependências específicas para o seu sistema operacional:
```shell
rvm requirements
```
{% endraw %}{% raw %}
<h2 id="scc">
  <a href="/pt_br/common/scc.html">scc</a> <a href="#scc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário escrito em GO que conta linhas de código.
> Mais informações: <https://github.com/boyter/scc>.

#### Mostrar o número de linhas de código no diretório atual:
```shell
scc
```
#### Mostrar o número de linhas de código de um diretório especificado:
```shell
scc {{caminho/para/diretorio}}
```
#### Mostrar o número de linhas de código por arquivo:
```shell
scc --by-file
```
#### Mostrar o resultado usando um formato específico (formato padrão é o `tabular`):
```shell
scc --format {{tabular|wide|json|csv|cloc-yaml|html|html-table}}
```
#### Contar apenas os arquivos com as extensões especificadas:
```shell
scc --include-ext {{go, java, js}}
```
#### Excluir diretórios da contagem:
```shell
scc --exclude-dir {{.git,.hg}}
```
#### Mostrar output organizado de acordo com o parâmetro especificado (organização padrão é `files`):
```shell
scc --sort {{files|name|lines|blanks|code|comments|complexity}}
```
#### Mostra a tela de ajuda:
```shell
scc -h
```
{% endraw %}{% raw %}
<h2 id="tar">
  <a href="/pt_br/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de compressão de arquivos.
> Utilizado com metodos de compressão como o de gzip ou bzip2.
> Mais informações: <https://www.gnu.org/software/tar>.

#### Compactando arquivos em um arquivo tar:
```shell
tar -cvf {{output.tar}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Compactando arquivos em arquivo gzip:
```shell
tar -czvf {{output.tar.gz}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Compactando arquivos definindo tipo de compressão automaticamente por extensão:
```shell
tar -cavf {{output.tar.xz}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Extraindo arquivos de um arquivo compactado:
```shell
tar -xvf {{input.tar[.gz|.bz2|.xz]}}
```
#### Extraindo arquivos de um arquivo compactado filtrando por gzip:
```shell
tar -xzvf {{input.tar[.gz|.bz2|.xz]}}
```
#### Extraindo arquivos de um arquivo compactado para um diretório específico:
```shell
tar -xvf {{input.tar[.gz|.bz2|.xz]}} -C {{diretório}}
```
#### Extrair arquivos seguindo um padrão:
```shell
tar -xvf {{input.tar}} --wildcards "{{*.html}}"
```
#### Listando arquivos de um arquivo tar:
```shell
tar -tvf {{input.tar}}
```
{% endraw %}{% raw %}
<h2 id="touch">
  <a href="/pt_br/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atualizar as timestamps de um arquivo para a hora atual.
> Se o arquivo não existir, cria um arquivo vazio, a menos que seja passado o parâmetro -c ou -h.
> Mais informações: <https://www.gnu.org/software/coreutils/touch>.

#### Criar um novo arquivo vazio, ou atualizar as timestamps para a hora atual:
```shell
touch {{arquivo}}
```
#### Definir as timestamps de um arquivo para a hora especificada:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{arquivo}}
```
#### Usar as timestamps do arquivo1 para definir as timestamps do arquivo2:
```shell
touch -r {{arquivo1}} {{arquivo2}}
```
#### Alterar as timestamps de um arquivo. Não cria novo arquivo se não existir:
```shell
touch -c {{arquivo}}
```
{% endraw %}{% raw %}
<h2 id="uname">
  <a href="/pt_br/common/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apresenta detalhes sobre o hardware e sistema operacional do computador.
> Nota: Para maiores detalhes sobre o sistema operacional, utilize o comando `lsb_release`.
> Mais informações: <https://www.gnu.org/software/coreutils/uname>.

#### Exibir informações relacionadas ao hardware: arquitetura e tipo de processador:
```shell
uname -mp
```
#### Exibir informações relacionadas ao software: sistema operacional, número da release e versão:
```shell
uname -srv
```
#### Exibir o nome de rede do computador:
```shell
uname -n
```
#### Exibir todas as informações disponíveis do sistema (hardware, software, nome de rede):
```shell
uname -a
```
{% endraw %}{% raw %}
<h2 id="units">
  <a href="/pt_br/common/units.html">units</a> <a href="#units"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Realiza a conversão entre duas unidades de medida.
> Mais informações: <https://www.gnu.org/software/units/>.

#### Rodar no modo interativo:
```shell
units
```
#### Mostrar a conversão entre duas unidades simples:
```shell
units {{quarts}} {{tablespoons}}
```
#### Converter entre unidades com quantidades definidas:
```shell
units {{15 pounds}} {{kilograms}}
```
#### Mostrar a conversão entre duas unidades compostas:
```shell
units "{{meters / second}}" "{{inches / hour}}"
```
#### Mostrar a conversão entre unidades de diferentes dimensões:
```shell
units "{{acres}}" "{{ft^2}}"
```
{% endraw %}{% raw %}
<h2 id="unrar">
  <a href="/pt_br/common/unrar.html">unrar</a> <a href="#unrar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Descompactar arquivos comprimidos no formato RAR.

#### Descompactar o arquivo mantendo a estrutura de diretórios original:
```shell
unrar x {{arquivo.rar}}
```
#### Descompactar o arquivo sem manter a estrutura de diretórios original:
```shell
unrar e {{arquivo.rar}}
```
#### Verificar a integridade do conteúdo de um arquivo:
```shell
unrar t {{arquivo.rar}}
```
#### Exibir o conteúdo de um arquivo sem descompactá-lo:
```shell
unrar l {{arquivo.rar}}
```
{% endraw %}{% raw %}
<h2 id="unzip">
  <a href="/pt_br/common/unzip.html">unzip</a> <a href="#unzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de descompactação de arquivos zip.

#### Extraindo arquivos zip:
```shell
unzip {{arquivo.zip}}
```
#### Extraindo arquivos zip para caminhos específicos:
```shell
unzip {{arquivo.zip}} -d {{caminho/para}}
```
#### Listando conteúdos de arquivos zip:
```shell
unzip -l {{arquivo.zip}}
```
#### Extraindo arquivos zip sobrescrevendo outros arquivos:
```shell
unzip -o {{arquivo.zip}}
```
#### Extraindo arquivos zip não sobrescrevendo outros arquivos:
```shell
unzip -n {{arquivo.zip}}
```
#### Extraindo arquivos zip sem a estrutura dos diretórios:
```shell
unzip -j {{arquivo.zip}}
```
{% endraw %}{% raw %}
<h2 id="wordgrinder">
  <a href="/pt_br/common/wordgrinder.html">wordgrinder</a> <a href="#wordgrinder"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Processador de texto em linha de comando.
> Mais informações: <https://cowlark.com/wordgrinder>.

#### Iniciar o wordgrinder (carrega um documento vazio por padrão):
```shell
wordgrinder
```
#### Abrir um arquivo específico:
```shell
wordgrinder {{nome_do_arquivo}}
```
#### Mostrar o menu:
```shell
Alt + M
```
{% endraw %}{% raw %}
<h2 id="wpa_supplicant">
  <a href="/pt_br/common/wpa_supplicant.html">wpa_supplicant</a> <a href="#wpa_supplicant"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de redes wireless protegidas.

#### Entrar em uma rede wireless protegida:
```shell
wpa_supplicant -i {{interface}} -c {{caminho/para/wpa_supplicant_conf.conf}}
```
#### Entrar em uma rede wireless protegida e executar o wpa_cli em um daemon:
```shell
wpa_supplicant -B -i {{interface}} -c {{caminho/para/wpa_supplicant_conf.conf}}
```
{% endraw %}{% raw %}
<h2 id="xcv">
  <a href="/pt_br/common/xcv.html">xcv</a> <a href="#xcv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Corta, copia e cola na linha de comando.
> Mais informações: <https://github.com/busterc/xcv>.

#### Cortar um arquivo:
```shell
xcv x {{arquivo_a_ser_cortado}}
```
#### Copiar um arquivo:
```shell
xcv c {{arquivo_a_ser_copiado}}
```
#### Colar um arquivo:
```shell
xcv v {{arquivo_a_ser_colado}}
```
#### Listar todos os arquivos disponíveis para serem colados:
```shell
xcv l
```
{% endraw %}{% raw %}
<h2 id="xkill">
  <a href="/pt_br/common/xkill.html">xkill</a> <a href="#xkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Termina o cliente associado a um elemento gráfico.
> Utilizado para forçar a terminação de processos que não respondem ou não apresentam botão "fechar".

#### Ativar um cursor para fechar uma janela com o clique do botão esquerdo do mouse (pressionar qualquer outro botão para cancelar):
```shell
xkill
```
{% endraw %}{% raw %}
<h2 id="xz">
  <a href="/pt_br/common/xz.html">xz</a> <a href="#xz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compactar ou descompactar arquivos com a extensão .xz ou .lzma.
> Mais informações: <https://tukaani.org/xz/format.html>.

#### Compactar um arquivo no formato xz:
```shell
xz {{arquivo}}
```
#### Descompactar um arquivo no formato xz:
```shell
xz -d {{arquivo.xz}}
```
#### Compactar um arquivo no formato lzma:
```shell
xz --format=lzma {{arquivo}}
```
#### Descompactar um arquivo no formato lzma:
```shell
xz -d --format=lzma {{arquivo.lzma}}
```
#### Descompactar um arquivo e escrever a saída no terminal:
```shell
xz -dc {{arquivo.xz}}
```
#### Compactar um arquivo sem apagar o arquivo original:
```shell
xz -k {{arquivo}}
```
#### Compactar um arquivo utilizando a compactação mais rápida:
```shell
xz -0 {{arquivo}}
```
#### Compactar um arquivo utilizando a compactação mais eficiente:
```shell
xz -9 {{arquivo}}
```
{% endraw %}{% raw %}
<h2 id="yarn-why">
  <a href="/pt_br/common/yarn-why.html">yarn-why</a> <a href="#yarn-why"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Identifica por que um pacote Yarn foi instalado.
> Mais informações: <https://www.npmjs.com/package/yarn-why>.

#### Exibir na tela o motivo de um pacote Yarn estar instalado:
```shell
yarn-why {{nome_do_pacote}}
```
{% endraw %}{% raw %}
<h2 id="yes">
  <a href="/pt_br/common/yes.html">yes</a> <a href="#yes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe algo na tela repetidamente.
> Mais informações: <https://www.gnu.org/software/coreutils/yes>.

#### Exibir na tela a palavra "mensagem" repetidamente:
```shell
yes {{mensagem}}
```
#### Exibir na tela a letra "y" repetidamente:
```shell
yes
```
{% endraw %}{% raw %}
<h2 id="zip">
  <a href="/pt_br/common/zip.html">zip</a> <a href="#zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de compressão de arquivos em arquivos zip.

#### Compactando arquivos em um arquivo zip:
```shell
zip {{output.zip}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Compactando todos os arquivos de um diretório:
```shell
zip {{output.zip}} {{caminho/do/diretorio/*}}
```
#### Adicionando arquivos a um arquivo zip existente:
```shell
zip {{arquivo_existente.zip}} {{caminho/do/diretorio}}
```
#### Compactando todos os arquivos de um diretório mantendo estruturas de diretórios:
```shell
zip -r {{output.zip}} {{caminho/do/diretorio}}
```
#### Compactando arquivos de um diretório excluindo arquivos específicos:
```shell
zip -r {{output.zip}} {{caminho/do/diretorio}} -x {{caminho/a/ser/excluido}}
```
#### Compactando arquivos definindo o nível de compressão [9]:
```shell
zip -r -{{9}} {{output.zip}} {{caminho/do/diretorio}}
```
#### Deletando arquivos de um arquivo zip:
```shell
zip -d {{output.zip}} "{{foo/*.ext}}"
```
{% endraw %}