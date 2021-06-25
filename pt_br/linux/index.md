---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#a2disconf">a2disconf</a>
* <a href="#a2dismod">a2dismod</a>
* <a href="#add-apt-repository">add-apt-repository</a>
* <a href="#adduser">adduser</a>
* <a href="#alpine">alpine</a>
* <a href="#apache2ctl">apache2ctl</a>
* <a href="#apk">apk</a>
* <a href="#apt">apt</a>
* <a href="#apt-cache">apt-cache</a>
* <a href="#apt-file">apt-file</a>
* <a href="#apt-get">apt-get</a>
* <a href="#apt-key">apt-key</a>
* <a href="#apt-mark">apt-mark</a>
* <a href="#aptitude">aptitude</a>
* <a href="#archey">archey</a>
* <a href="#arp-scan">arp-scan</a>
* <a href="#as">as</a>
* <a href="#aspell">aspell</a>
* <a href="#at">at</a>
* <a href="#authconfig">authconfig</a>
* <a href="#autorandr">autorandr</a>
* <a href="#beep">beep</a>
* <a href="#bmon">bmon</a>
* <a href="#bpftrace">bpftrace</a>
* <a href="#brctl">brctl</a>
* <a href="#brew">brew</a>
* <a href="#cal">cal</a>
* <a href="#calc">calc</a>
* <a href="#calcurse">calcurse</a>
* <a href="#certbot">certbot</a>
* <a href="#chage">chage</a>
* <a href="#chattr">chattr</a>
* <a href="#chkconfig">chkconfig</a>
* <a href="#cmus">cmus</a>
* <a href="#compgen">compgen</a>
* <a href="#cpuid">cpuid</a>
* <a href="#csplit">csplit</a>
* <a href="#diff3">diff3</a>
* <a href="#dmesg">dmesg</a>
* <a href="#dmidecode">dmidecode</a>
* <a href="#dnf">dnf</a>
* <a href="#dpkg">dpkg</a>
* <a href="#dpkg-query">dpkg-query</a>
* <a href="#eyed3">eyeD3</a>
* <a href="#fatlabel">fatlabel</a>
* <a href="#fc">fc</a>
* <a href="#fc-list">fc-list</a>
* <a href="#fdisk">fdisk</a>
* <a href="#i3lock">i3lock</a>
* <a href="#rolldice">rolldice</a>
* <a href="#top">top</a>
* <a href="#tree">tree</a>
* <a href="#watch">watch</a>
* <a href="#wtf">wtf</a>

{% raw %}
<h2 id="a2disconf">
  <a href="/pt_br/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Desativar um arquivo de configuração em sistemas operacionais baseados no Debian.
> Mais informações: <https://manpages.debian.org/buster/apache2/a2disconf.8.en.html>.

#### Desativar um arquivo de configuração:
```shell
sudo a2disconf {{arquivo_de_configuracao}}
```
#### Não mostrar mensagens informativas:
```shell
sudo a2disconf --quiet {{arquivo_de_configuracao}}
```
{% endraw %}{% raw %}
<h2 id="a2dismod">
  <a href="/pt_br/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Desativa um módulo do Apache em sistemas operacionais baseados no Debian.
> Mais informações: <https://manpages.debian.org/buster/apache2/a2dismod.8.en.html>.

#### Desativar um módulo:
```shell
sudo a2dismod {{módulo}}
```
#### Não mostrar mensagens informativas:
```shell
sudo a2dismod --quiet {{módulo}}
```
{% endraw %}{% raw %}
<h2 id="add-apt-repository">
  <a href="/pt_br/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciar definições de repositórios APT.

#### Adicionar um repositório:
```shell
add-apt-repository {{especificacao_do_repositorio}}
```
#### Remover um repositório:
```shell
add-apt-repository --remove {{especificacao_do_repositorio}}
```
#### Adicionar um repositório e atualizar o cache do(s) pacote(s) deste repositório:
```shell
add-apt-repository --update {{especificacao_do_repositorio}}
```
#### Adicionar um repositório e habilitar o download do código fonte do(s) pacote(s) deste repositório:
```shell
add-apt-repository --enable-source {{especificacao_do_repositorio}}
```
{% endraw %}{% raw %}
<h2 id="adduser">
  <a href="/pt_br/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para criação de novos usuários.
> Mais informações: <https://manpages.debian.org/latest/adduser/adduser.html>.

#### Criar um novo usuário, o seu diretório na pasta home e solicitar o preenchimento da sua senha:
```shell
adduser {{nome_do_usuario}}
```
#### Criar um novo usuário sem o seu diretório na pasta home:
```shell
adduser --no-create-home {{nome_do_usuario}}
```
#### Criar um novo usuário especificando a localização do seu diretório:
```shell
adduser --home {{caminho_da_pasta_do_usuario}} {{nome_do_usuario}}
```
#### Criar um novo usuário e configurar o seu shell de login:
```shell
adduser --shell {{caminho_para_o_shell}} {{nome_do_usuario}}
```
#### Criar um novo usuário e atribuí-lo a um grupo:
```shell
adduser --ingroup {{grupo}} {{nome_do_usuario}}
```
{% endraw %}{% raw %}
<h2 id="alpine">
  <a href="/pt_br/linux/alpine.html">alpine</a> <a href="#alpine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um cliente de e-mail e programa de newsgroup Usenet com uma interface inspirada no pico e nano.
> Suporta a maioria dos serviços de e-mail por meio de IMAP.

#### Iniciar o alpine:
```shell
alpine
```
#### Abrir o alpine na tela de composição de mensagem com o e-mail do destinatário preenchido:
```shell
alpine {{email@exemplo.net}}
```
#### Encerrar o alpine:
```shell
'q' e 'y'
```
{% endraw %}{% raw %}
<h2 id="apache2ctl">
  <a href="/pt_br/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interface de controle do servidor web HTTP Apache.
> Este comando está disponível nas distribuições baseadas em Debian, para as baseadas em RHEL veja `httpd`.
> Mais informações: <https://manpages.debian.org/latest/apache2/apache2ctl.8.html>.

#### Iniciar o Apache. Caso ele já esteja em execução, uma mensagem será apresentada:
```shell
sudo apache2ctl start
```
#### Encerrar o Apache:
```shell
sudo apache2ctl stop
```
#### Reiniciar o Apache:
```shell
sudo apache2ctl restart
```
#### Verificar se o arquivo de configuração está correto sintaticamente:
```shell
sudo apache2ctl -t
```
#### Listar os módulos carregados:
```shell
sudo apache2ctl -M
```
{% endraw %}{% raw %}
<h2 id="apk">
  <a href="/pt_br/linux/apk.html">apk</a> <a href="#apk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes da distribuição Alpine.

#### Atualizar os índices dos pacotes disponíveis:
```shell
apk update
```
#### Instalar um pacote:
```shell
apk add {{pacote}}
```
#### Remover um pacote:
```shell
apk del {{pacote}}
```
#### Reparar ou atualizar um pacote sem modificar as principais dependências:
```shell
apk fix {{pacote}}
```
#### Procurar um pacote especificando alguma palavra-chave:
```shell
apk search {{palavra_chave}}
```
#### Exibir informações sobre um pacote:
```shell
apk info {{pacote}}
```
{% endraw %}{% raw %}
<h2 id="apt-cache">
  <a href="/pt_br/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Buscador de pacotes para distribuições baseadas no Debian.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Buscar pacotes, no cache de pacotes APT, correspondentes ao critério de busca:
```shell
apt-cache search {{criterio_de_busca}}
```
#### Exibir informações sobre um pacote:
```shell
apt-cache show {{nome_do_pacote}}
```
#### Informar a situação de um pacote, se ele está instalado e atualizado:
```shell
apt-cache policy {{nome_do_pacote}}
```
#### Exibir as dependências de um pacote:
```shell
apt-cache depends {{nome_do_pacote}}
```
#### Exibir pacotes dependentes de um determinado pacote:
```shell
apt-cache rdepends {{nome_do_pacote}}
```
{% endraw %}{% raw %}
<h2 id="apt-file">
  <a href="/pt_br/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Buscador de arquivos nos pacotes apt, incluindo os não instalados.
> Mais informações: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Atualizar as informações dos pacotes a partir de todos os repositórios remotos:
```shell
sudo apt update
```
#### Buscar por pacotes que contêm o arquivo ou caminho especificado:
```shell
apt-file search {{nome_do_pacote_ou_caminho}}
```
#### Listar o conteúdo de um pacote específico:
```shell
apt-file list {{nome_do_pacote}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/pt_br/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em Debian.
> Procure por pacotes utilizando o `apt-cache`.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Atualizar a lista de pacotes disponíveis (recomenda-se executá-lo antes de outros comandos `apt-get`):
```shell
apt-get update
```
#### Instalar um pacote ou atualizá-lo para a versão mais recente:
```shell
apt-get install {{nome_do_pacote}}
```
#### Remover um pacote:
```shell
apt-get remove {{nome_do_pacote}}
```
#### Remover um pacote e os seus arquivos de configuração:
```shell
apt-get purge {{nome_do_pacote}}
```
#### Atualizar todos os pacotes instalados para as versões mais recentes:
```shell
apt-get upgrade
```
#### Limpar o repositório local — removendo os arquivos de pacotes (`.deb`) de downloads interrompidos que não podem mais ser baixados:
```shell
apt-get autoclean
```
#### Remover todos os pacotes obsoletos:
```shell
apt-get autoremove
```
#### Atualizar os pacotes instalados (semelhante ao `upgrade`), porém removendo os obsoletos e instalando pacotes solicitados por novas dependências:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt-key">
  <a href="/pt_br/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de chaves utilizado pelo gerenciador de pacotes APT nas distribuições baseadas em Debian.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Exibir as chaves confiáveis:
```shell
apt-key list
```
#### Adicionar uma chave na lista de chaves confiáveis:
```shell
apt-key add {{arquivo_da_chave_publica.asc}}
```
#### Remover uma chave da lista de chaves confiáveis:
```shell
apt-key del {{key_id}}
```
#### Adicionar uma chave remota na lista de chaves confiáveis:
```shell
wget -qO - {{https://host.tld/arquivo.key}} | apt-key add -
```
#### Adicionar uma chave, de um servidor de chaves, na lista de chaves confiáveis:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{KEYID}}
```
{% endraw %}{% raw %}
<h2 id="apt-mark">
  <a href="/pt_br/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário que altera as configurações dos pacotes instalados.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marcar um pacote como instalado automaticamente:
```shell
sudo apt-mark auto {{nome_do_pacote}}
```
#### Bloquear um pacote na sua versão atual, impedindo que ele seja atualizado:
```shell
sudo apt-mark hold {{nome_do_pacote}}
```
#### Desbloquear um pacote, permitindo que ele seja atualizado:
```shell
sudo apt-mark unhold {{nome_do_pacote}}
```
#### Listar os pacotes instalados manualmente:
```shell
apt-mark showmanual
```
#### Listar os pacotes bloqueados:
```shell
apt-mark showhold
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/pt_br/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em Debian.
> Mais informações: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Atualizar a lista de pacotes disponíveis (recomenda-se executá-lo antes de outros comandos `apt`):
```shell
sudo apt update
```
#### Buscar pacotes correspondentes ao critério de busca:
```shell
apt search {{criterio_de_busca}}
```
#### Exibir as informações de pacote:
```shell
apt show {{nome_do_pacote}}
```
#### Instalar um pacote ou atualizá-lo para a versão mais recente:
```shell
sudo apt install {{nome_do_pacote}}
```
#### Remover um pacote (Para remover os arquivos de configuração deve-se usar a opção `purge` ao invés do `remove`):
```shell
sudo apt remove {{nome_do_pacote}}
```
#### Atualizar os pacotes instalados para as versões mais recentes:
```shell
sudo apt upgrade
```
{% endraw %}{% raw %}
<h2 id="aptitude">
  <a href="/pt_br/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em Debian.
> Mais informações: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Atualizar a lista de pacotes disponíveis (recomenda-se executá-lo antes de outros comandos `aptitude`):
```shell
aptitude update
```
#### Instalar um novo pacote e suas dependências:
```shell
aptitude install {{nome_do_pacote}}
```
#### Buscar pacotes correspondentes ao critério de busca:
```shell
aptitude search {{criterio_de_busca}}
```
#### Remover um pacote e todos que dependam dele:
```shell
aptitude remove {{nome_do_pacote}}
```
#### Atualizar os pacotes instalados para as versões mais recentes:
```shell
aptitude upgrade
```
#### Atualizar os pacotes instalados (semelhante ao `upgrade`), porém removendo os obsoletos e instalando pacotes solicitados por novas dependências:
```shell
aptitude full-upgrade
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/pt_br/linux/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que exibe informações do sistema de forma estilizada.

#### Exibir as informações do sistema:
```shell
archey
```
{% endraw %}{% raw %}
<h2 id="arp-scan">
  <a href="/pt_br/linux/arp-scan.html">arp-scan</a> <a href="#arp-scan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Envia pacotes ARP para máquinas (identificadas por endereço IP ou por nome de domínio) em uma rede local, identificando as máquinas ativas de acordo com as respostas.

#### Verificar as máquinas da rede local:
```shell
arp-scan --localnet
```
#### Verificar as máquinas de uma rede IP especificando a máscara de bit:
```shell
arp-scan {{192.168.1.1}}/{{24}}
```
#### Verificar as máquinas de uma rede IP que estejam em uma faixa de valores:
```shell
arp-scan {{127.0.0.0}}-{{127.0.0.31}}
```
#### Verificar as máquinas de uma rede IP especificando a máscara de rede:
```shell
arp-scan {{10.0.0.0}}:{{255.255.255.0}}
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/pt_br/linux/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Assembler GNU multiplataforma.
> Seu objetivo inicial é realizar o montagem do arquivo gerado pelo `gcc` para ser utilizado pelo `ld`.

#### Realizar a montagem de um arquivo, o resultado dessa operação será gravado no arquivo a.out:
```shell
as {{arquivo.s}}
```
#### Realizar a montagem de um arquivo, o resultado dessa operação será gravado em um arquivo específico:
```shell
as {{arquivo.s}} -o {{saida.o}}
```
#### Realizar a montagem de um arquivo rapidamente, pois ignora o pré-processamento de comentários e espaços em branco. (Deve ser utilizado apenas em compiladores confiáveis):
```shell
as -f {{arquivo.s}}
```
#### Adiciona um caminho na lista de diretórios onde será realizada a busca por arquivos especificados na diretiva .include:
```shell
as -I {{caminho_para_o_diretorio}} {{arquivo.s}}
```
{% endraw %}{% raw %}
<h2 id="aspell">
  <a href="/pt_br/linux/aspell.html">aspell</a> <a href="#aspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verificador ortográfico interativo.

#### Verificar a ortografia do texto de um arquivo:
```shell
aspell check {{arquivo}}
```
#### Exibir as palavras escritas incorretamente no terminal:
```shell
cat {{arquivo}} | aspell list
```
#### Exibir os dicionários disponíveis:
```shell
aspell dicts
```
#### Executar aspell utilizando uma língua diferente (informe o código ISO 639 da língua):
```shell
aspell --lang={{cs}}
```
#### Exibir os erros ortográficos no terminal e ignorando as palavras da lista pessoal:
```shell
cat {{arquivo}} | aspell --personal={{lista_pessoal.pws}} {{list}}
```
{% endraw %}{% raw %}
<h2 id="at">
  <a href="/pt_br/linux/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executa comandos em um determinado momento.
> Mais informações: <https://man.archlinux.org/man/at.1>.

#### Iniciar o prompt `at` para que um novo conjunto de comandos seja agendado, pressione `Ctrl + D` para salvar e sair:
```shell
at {{hh:mm:ss}}
```
#### Executar os comandos e enviar o resultado por e-mail utilizando algum programa de envio de e-mail local, por exemplo o sendmail:
```shell
at {{hh:mm:ss}} -m
```
#### Executar um script em um determinado momento:
```shell
at {{hh:mm:ss}} -f {{caminho_para_o_script}}
```
{% endraw %}{% raw %}
<h2 id="authconfig">
  <a href="/pt_br/linux/authconfig.html">authconfig</a> <a href="#authconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interface de linha comandos para configurar o sistema de autenticação.

#### Exibir as configurações atuais (ou dry run):
```shell
authconfig --test
```
#### Configurar o servidor para utilizar diferentes algoritmos de hash para as senhas:
```shell
authconfig --update --passalgo={{algoritmo}}
```
#### Habilitar a autenticação via LDAP:
```shell
authconfig --update --enableldapauth
```
#### Desabilitar a autenticação via LDAP:
```shell
authconfig --update --disableldapauth
```
#### Habilitar o Network Information Service (NIS):
```shell
authconfig --update --enablenis
```
#### Habilitar Kerberos:
```shell
authconfig --update --enablekrb5
```
#### Habilitar a autenticação Winbind (Active Directory):
```shell
authconfig --update --enablewinbindauth
```
#### Habilitar a autorização local:
```shell
authconfig --update --enablelocauthorize
```
{% endraw %}{% raw %}
<h2 id="autorandr">
  <a href="/pt_br/linux/autorandr.html">autorandr</a> <a href="#autorandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Altera o layout da tela automaticamente.

#### Salvar o layout da tela em uso:
```shell
autorandr -s {{nome_do_perfil}}
```
#### Exibir os perfis salvos:
```shell
autorandr
```
#### Alterar o perfil:
```shell
autorandr -l {{nome_do_perfil}}
```
#### Definir o perfil padrão:
```shell
autorandr -d {{nome_do_perfil}}
```
{% endraw %}{% raw %}
<h2 id="beep">
  <a href="/pt_br/linux/beep.html">beep</a> <a href="#beep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário que permite o computador emitir sons.

#### Emitir um som:
```shell
beep
```
#### Emitir um som repetidamente:
```shell
beep -r {{repeticoes}}
```
#### Emitir um som em uma frequência (Hz) específica e com duração específica (milisegundos):
```shell
beep -f {{frequencia}} -l {{duracao}}
```
#### Emitir cada frequência e duração como um som diferente:
```shell
beep -f {{frequencia}} -l {{duracao}} -n -f {{frequencia}} -l {{duracao}}
```
#### Executar a escala de Dó maior:
```shell
beep -f 262 -n -f 294 -n -f 330 -n -f 349 -n -f 392 -n -f 440 -n -f 494 -n -f 523
```
{% endraw %}{% raw %}
<h2 id="bmon">
  <a href="/pt_br/linux/bmon.html">bmon</a> <a href="#bmon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitora a largura de banda e produz estatísticas relacionadas a rede.

#### Exibir uma lista com todas as interfaces de rede:
```shell
bmon -a
```
#### Exibir as taxas de transferência de dados em bits por segundo:
```shell
bmon -b
```
#### Definir quais interfaces serão visíveis:
```shell
bmon -p {{interface_1,interface_2,interface_3}}
```
#### Definir o intervalo (em segundos) que a taxa por contador será calculada:
```shell
bmon -R {{2.0}}
```
{% endraw %}{% raw %}
<h2 id="bpftrace">
  <a href="/pt_br/linux/bpftrace.html">bpftrace</a> <a href="#bpftrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Linguagem de análise de alto nível para eBPF Linux.
> Mais informações: <https://github.com/iovisor/bpftrace>.

#### Verifique a versão do bpftrace:
```shell
bpftrace -V
```
#### Lista todos os probes:
```shell
sudo bpftrace -l
```
#### Rode um programa de uma linha (e.g. número de syscalls por programa):
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter { @[comm] = count(); }}}'
```
#### Rode um programa de um arquivo:
```shell
sudo bpftrace {{caminho/do/arquivo}}
```
#### Analise um programa por PID:
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter /pid == 123/ { @[comm] = count(); }}}'
```
#### Mostre o resultado do programa em eBPF, sem rodar ele:
```shell
sudo bpftrace -d -e '{{programa_de_uma_linha}}'
```
{% endraw %}{% raw %}
<h2 id="brctl">
  <a href="/pt_br/linux/brctl.html">brctl</a> <a href="#brctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administração de pontes de rede.

#### Exibir uma lista com informações das pontes de rede existentes:
```shell
sudo brctl show
```
#### Cria uma ponte de rede:
```shell
sudo brctl add {{nome_da_ponte}}
```
#### Remover uma ponte de rede:
```shell
sudo brctl del {{nome_da_ponte}}
```
#### Adicionar uma interface de rede em uma ponte de rede existente:
```shell
sudo brctl addif {{nome_da_ponte}} {{nome_da_interface_de_rede}}
```
#### Remover uma interface de rede de uma ponte de rede existente:
```shell
sudo brctl delif {{nome_da_ponte}} {{nome_da_interface_de_rede}}
```
{% endraw %}{% raw %}
<h2 id="brew">
  <a href="/pt_br/linux/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A versão Linux do gerenciador de pacotes Homebrew.

#### Buscar por fórmulas disponíveis:
```shell
brew search {{termo_da_busca}}
```
#### Instalar a última versão estável de uma fórmula (utilizar `--devel` para versões de desenvolvimento):
```shell
brew install {{formula}}
```
#### Listar as fórmulas instaladas:
```shell
brew list
```
#### Atualizar uma fórmula instalada (se não for informado o nome de uma fórmula, todas as fórmulas serão atualizadas):
```shell
brew upgrade {{formula}}
```
#### Recuperar a versão mais recente do Linuxbrew e de todas as fórmulas do GitHub:
```shell
brew update
```
#### Exibir as fórmulas que possuem novas versões disponíveis:
```shell
brew outdated
```
#### Exibir informações sobre uma fórmula (versão, caminho de instalação, dependências, etc.):
```shell
brew info {{formula}}
```
#### Verificar a instalação local em busca de possíveis problemas:
```shell
brew doctor
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/pt_br/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe as informações do calendário, destacando o dia atual.

#### Exibir o calendário do mês atual:
```shell
cal
```
#### Exibir o calendário do meses anterior, atual e seguinte:
```shell
cal -3
```
#### Utilizar segunda-feira como o primeiro dia da semana:
```shell
cal --monday
```
#### Exibir o calendário de um ano específico (4 dígitos):
```shell
cal {{ano}}
```
#### Exibir o calendário para um mês e ano específico:
```shell
cal {{mes}} {{ano}}
```
{% endraw %}{% raw %}
<h2 id="calc">
  <a href="/pt_br/linux/calc.html">calc</a> <a href="#calc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculadora interativa de precisão arbitrária no terminal.

#### Iniciar a calculadora em modo interativo:
```shell
calc
```
#### Realizar o cálculo em modo não interativo:
```shell
calc -p '{{85 * (36 / 4)}}'
```
{% endraw %}{% raw %}
<h2 id="calcurse">
  <a href="/pt_br/linux/calcurse.html">calcurse</a> <a href="#calcurse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um calendário e agenda baseados em texto para a linha de comando.
> Mais informações: <https://calcurse.org>.

#### Iniciar o calcurse em modo interativo:
```shell
calcurse
```
#### Mostrar os agendamentos e eventos para o presente dia:
```shell
calcurse --appointment
```
#### Apagar todos os objetos gravados localmente e importar os objetos remotos:
```shell
calcurse-caldav --init=keep-remote
```
#### Apagar todos os objetos remotos e enviar os objetos gravados localmente:
```shell
calcurse-caldav --init=keep-local
```
#### Copiar os objetos gravados localmente para o servidor CalDAV e vice-versa:
```shell
calcurse-caldav --init=two-way
```
{% endraw %}{% raw %}
<h2 id="certbot">
  <a href="/pt_br/linux/certbot.html">certbot</a> <a href="#certbot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> O agente da Let's Encrypt para obtenção e renovação de certificados TLS automaticamente.
> Sucessor do `letsencrypt`.

#### Obter um novo certificado via autorização webroot, porém sem instalá-lo automaticamente:
```shell
sudo certbot certonly --webroot --webroot-path {{caminho_para_webroot}} --domain {{subdominio.dominio.com}}
```
#### Obter um novo certificado via autorização nginx e instalá-lo automaticamente:
```shell
sudo certbot --nginx --domain {{subdominio.dominio.com}}
```
#### Obter um novo certificado via autorização apache e instalá-lo automaticamente:
```shell
sudo certbot --apache --domain {{subdominio.dominio.com}}
```
#### Renovar todos os certificados que expirarão em 30 dias ou menos (não esqueça de reiniciar todos os servidores que usam os certificados):
```shell
sudo certbot renew
```
#### Simular a obtenção de um novo certificado, porém sem salvá-lo no disco rígido:
```shell
sudo certbot --webroot --webroot-path {{caminho_para_webroot}} --domain {{subdominio.dominio.com}} --dry-run
```
#### Obter um certificado não confiável para testes:
```shell
sudo certbot --webroot --webroot-path {{caminho_para_webroot}} --domain {{subdominio.dominio.com}} --test-cert
```
{% endraw %}{% raw %}
<h2 id="chage">
  <a href="/pt_br/linux/chage.html">chage</a> <a href="#chage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia informações de expiração de conta e senha do usuário.

#### Exibir as informações referentes a senha do usuário:
```shell
chage -l {{nome_do_usuario}}
```
#### Habilitar a expiração da senha do usuário em 10 dias:
```shell
sudo chage -M {{10}} {{nome_do_usuario}}
```
#### Desabilitar a expiração da senha do usuário:
```shell
sudo chage -M -1 {{nome_do_usuario}}
```
#### Definir a data de expiração da conta do usuário:
```shell
sudo chage -E {{YYYY-MM-DD}}
```
#### Obrigar o usuário a alterar sua senha no próximo login:
```shell
sudo chage -d 0
```
{% endraw %}{% raw %}
<h2 id="chattr">
  <a href="/pt_br/linux/chattr.html">chattr</a> <a href="#chattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Altera os atributos de arquivos ou diretórios.

#### Bloquear um arquivo ou diretório para mudanças ou remoção, mesmo para um super usuário:
```shell
chattr +i {{caminho_do_arquivo_ou_diretorio}}
```
#### Desbloquear um arquivo ou diretório:
```shell
chattr -i {{caminho_do_arquivo_ou_diretorio}}
```
#### Bloquear diretório e todos os seus arquivos para mudanças ou remoção:
```shell
chattr -R +i {{caminho_do_diretorio}}
```
{% endraw %}{% raw %}
<h2 id="chkconfig">
  <a href="/pt_br/linux/chkconfig.html">chkconfig</a> <a href="#chkconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia o runlevel dos serviços no CentOS 6.

#### Exibir os serviços com os respectivos runlevels:
```shell
chkconfig --list
```
#### Exibir o runlevel de um serviço:
```shell
chkconfig --list {{ntpd}}
```
#### Habilitar o início de um serviço durante o processo de boot:
```shell
chkconfig {{sshd}} on
```
#### Habilitar o início do serviço durante o processo de boot para os runlevels 2, 3, 4 e 5:
```shell
chkconfig --level {{2345}} {{sshd}} on
```
#### Desabilitar a inicialização de um determinado serviço durante o processo de boot:
```shell
chkconfig {{ntpd}} off
```
#### Desabilitar a inicialização de um determinado serviço durante o processo de boot para o runlevel 3:
```shell
chkconfig --level {{3}} {{ntpd}} off
```
{% endraw %}{% raw %}
<h2 id="cmus">
  <a href="/pt_br/linux/cmus.html">cmus</a> <a href="#cmus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Player de música via terminal.
> Use as setas para navegar, `<enter/return>` para selecionar, e números 1-8 para alterar as telas de opções.

#### Iniciar o cmus em um diretório específico:
```shell
cmus {{caminho_do_diretorio}}
```
#### Adicionar arquivo/diretório a biblioteca:
```shell
:add {{caminho_para_arquivo_ou_diretorio}}
```
#### Parar/reiniciar a música atual:
```shell
c
```
#### Ativar/Desativar o modo aleatório:
```shell
s
```
#### Sair cmus:
```shell
q
```
{% endraw %}{% raw %}
<h2 id="compgen">
  <a href="/pt_br/linux/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um programa para auto completar comandos no Bash, ele é executado ao pressionar duas vezes a tecla TAB.

#### Exibir todos os comandos que você pode executar:
```shell
compgen -c
```
#### Exibir todos os alias:
```shell
compgen -a
```
#### Exibir todas as funções que você pode executar:
```shell
compgen -A function
```
#### Exibir todas as palavras reservadas do shell:
```shell
compgen -k
```
#### Exibir todos os comandos/alias que iniciam com o termo 'ls':
```shell
compgen -ac {{ls}}
```
{% endraw %}{% raw %}
<h2 id="cpuid">
  <a href="/pt_br/linux/cpuid.html">cpuid</a> <a href="#cpuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe informações detalhadas sobre todas as CPUs.

#### Exibir informações de todas as CPUs:
```shell
cpuid
```
#### Exibir informações apenas da CPU atual:
```shell
cpuid -1
```
#### Exibir informações em hexadecimal sem decodificação:
```shell
cpuid -r
```
{% endraw %}{% raw %}
<h2 id="csplit">
  <a href="/pt_br/linux/csplit.html">csplit</a> <a href="#csplit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Divide um arquivo em várias partes.
> O padrão de nomenclatura dos arquivos será "xx00", "xx01" e assim por diante.
> Mais informações: <https://www.gnu.org/software/coreutils/csplit>.

#### Dividir um arquivo nas linhas 5 e 23:
```shell
csplit {{arquivo}} {{5}} {{23}}
```
#### Dividir um arquivo a cada 5 linhas (este comando irá falhar se o total de linhas do arquivo não for divisível por 5):
```shell
csplit {{arquivo}} {{5}} {*}
```
#### Dividir um arquivo a cada 5 linhas, ignorando o fato do total de linhas ser divisível por 5:
```shell
csplit -k {{arquivo}} {{5}} {*}
```
#### Dividir o arquivo na linha 5 e utilizar um prefixo específico para os arquivos de saída:
```shell
csplit {{arquivo}} {{5}} -f {{prefix}}
```
#### Dividir um arquivo na linha que atenda a expressão regular:
```shell
csplit {{arquivo}} /{{expressao_regular}}/
```
{% endraw %}{% raw %}
<h2 id="diff3">
  <a href="/pt_br/linux/diff3.html">diff3</a> <a href="#diff3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compara 3 arquivos linha por linha.

#### Comparar os arquivos:
```shell
diff3 {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Exibir todas as diferenças, destacando os conflitos:
```shell
diff3 --show-all {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/pt_br/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Escreve as mensagens do kernel na terminal.

#### Exibir as mensagens do kernel:
```shell
dmesg
```
#### Exibir as mensagens de erro do kernel:
```shell
dmesg --level err
```
#### Exibir as mensagens do kernel e manter o terminal esperando por novas menagens, semelhante ao `tail -f` (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -w
```
#### Exibir a quantidade de memória física disponível no sistema:
```shell
dmesg | grep -i memory
```
#### Exibir as mensagens do kernel divididas em páginas:
```shell
dmesg | less
```
#### Exibir as menagens do kernel com data/hora (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -T
```
#### Exibir as mensagens do kernel em um formato de fácil leitura (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -H
```
#### Exibir as mensagens do kernel utilizando cores (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -L
```
{% endraw %}{% raw %}
<h2 id="dmidecode">
  <a href="/pt_br/linux/dmidecode.html">dmidecode</a> <a href="#dmidecode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe em formato de fácil leitura o sumário DMI (também conhecido como SMBIOS) .
> Requer privilégio de super usuário.

#### Exibir o sumário do DMI:
```shell
sudo dmidecode
```
#### Exibir a versão da BIOS:
```shell
sudo dmidecode -s bios-version
```
#### Exibir o número de série do sistema:
```shell
sudo dmidecode -s system-serial-number
```
#### Exibir as informações da BIOS:
```shell
sudo dmidecode -t bios
```
#### Exibir as informações da CPU:
```shell
sudo dmidecode -t processor
```
#### Exibir as informações da memória:
```shell
sudo dmidecode -t memory
```
{% endraw %}{% raw %}
<h2 id="dnf">
  <a href="/pt_br/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em RHEL (substituto do yum).

#### Instalar um novo pacote:
```shell
sudo dnf install {{nome_do_pacote}}
```
#### Instalar um novo pacote e responder sim para todas as questões:
```shell
sudo dnf -y install {{nome_do_pacote}}
```
#### Remover um pacote:
```shell
sudo dnf remove {{nome_do_pacote}}
```
#### Atualizar todos os pacotes instalados para as versões mais recentes:
```shell
sudo dnf upgrade
```
{% endraw %}{% raw %}
<h2 id="dpkg-query">
  <a href="/pt_br/linux/dpkg-query.html">dpkg-query</a> <a href="#dpkg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que mostra informações dos pacotes instalados.

#### Exibir os pacotes instalados:
```shell
dpkg-query -l
```
#### Exibir os pacotes instalados correspondentes ao critério de busca:
```shell
dpkg-query -l '{{criterio_de_busca}}'
```
#### Exibir todos os arquivos instalados por um pacote:
```shell
dpkg-query -L {{nome_do_pacote}}
```
#### Exibir informações sobre um pacote:
```shell
dpkg-query -s {{nome_do_pacote}}
```
{% endraw %}{% raw %}
<h2 id="dpkg">
  <a href="/pt_br/linux/dpkg.html">dpkg</a> <a href="#dpkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes Debian.

#### Instalar um pacote:
```shell
dpkg -i {{arquivo.deb}}
```
#### Remover um pacote:
```shell
dpkg -r {{nome_do_pacote}}
```
#### Exibir os pacotes correspondentes ao critério de busca:
```shell
dpkg -l {{criterio_de_busca}}
```
#### Exibe o conteúdo do pacote:
```shell
dpkg -L {{nome_do_pacote}}
```
#### Exibir o conteúdo do arquivo de um pacote:
```shell
dpkg -c {{arquivo.deb}}
```
#### Apresentar o pacote proprietário de um determinado arquivo:
```shell
dpkg -S {{nome_do_arquivo}}
```
{% endraw %}{% raw %}
<h2 id="eyed3">
  <a href="/pt_br/linux/eyed3.html">eyeD3</a> <a href="#eyed3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lê e manipula os metadados de arquivos MP3.
> Mais informações: <https://eyed3.readthedocs.io/en/latest/>.

#### Visualizar as informações de um arquivo MP3:
```shell
eyeD3 {{arquivo.mp3}}
```
#### Definir o título de um arquivo MP3:
```shell
eyeD3 --title "{{titulo}}" {{arquivo.mp3}}
```
#### Definir o álbum de todos os arquivos MP3 de um diretório:
```shell
eyeD3 --album "{{nome_do_album}}" {{*.mp3}}
```
#### Definir a capa do álbum para um arquivo MP3:
```shell
eyeD3 --add-image {{capa.jpeg}}:FRONT_COVER: {{arquivo.mp3}}
```
{% endraw %}{% raw %}
<h2 id="fatlabel">
  <a href="/pt_br/linux/fatlabel.html">fatlabel</a> <a href="#fatlabel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Define ou exibe o rótulo de uma partição FAT32.

#### Exibir o rótulo de uma partição FAT32:
```shell
fatlabel {{/dev/sda1}}
```
#### Definir o rótulo de uma partição FAT32:
```shell
fatlabel {{/dev/sdc3}} "{{rotulo}}"
```
{% endraw %}{% raw %}
<h2 id="fc-list">
  <a href="/pt_br/linux/fc-list.html">fc-list</a> <a href="#fc-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe todas as fontes disponíveis no sistema.

#### Exibir as fontes instaladas correspondentes ao critério de busca:
```shell
fc-list | grep '{{criterio_de_busca}}'
```
{% endraw %}{% raw %}
<h2 id="fc">
  <a href="/pt_br/linux/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Abre o último comando executado em um editor de texto.

#### Abrir o último comando executado no editor de texto padrão do sistema:
```shell
fc
```
#### Especificar o editor de texto que será utilizado ao executar o comando:
```shell
fc -e {{'emacs'}}
```
#### Exibir um histórico dos últimos comandos executados:
```shell
fc -l
```
{% endraw %}{% raw %}
<h2 id="fdisk">
  <a href="/pt_br/linux/fdisk.html">fdisk</a> <a href="#fdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de tabelas de partições e partições no disco rígido.

#### Exibir as partições:
```shell
fdisk -l
```
#### Iniciar o manipulador de partições:
```shell
fdisk {{/dev/sda}}
```
{% endraw %}{% raw %}
<h2 id="i3lock">
  <a href="/pt_br/linux/i3lock.html">i3lock</a> <a href="#i3lock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bloqueador de tela simples para o i3wm.
> Mais informações: <https://i3wm.org/i3lock>.

#### Bloqueia a tela com uma cor de fundo (formato rrggbb):
```shell
i3lock -c {{0000ff}}
```
#### Bloqueia a tela com uma imagem PNG:
```shell
i3lock -i {{local/da/imagem.png}}
```
#### Desabilita o indicador de desbloqueio (remove a resposta ao apertar teclas):
```shell
i3lock -u
```
#### Exibe o ponteiro do mouse ao invés de ocultá-lo ('default' para o ponteiro padrão, 'win' para um ponteiro MS Windows):
```shell
i3lock -p {{default|win}}
```
#### Bloqueia a tela com uma imagem PNG exibida em múltiplos monitores, com o ponteiro do mouse habilitado:
```shell
i3lock -i {{local/da/imagem.png}} -p {{default|win}} -t
```
{% endraw %}{% raw %}
<h2 id="rolldice">
  <a href="/pt_br/linux/rolldice.html">rolldice</a> <a href="#rolldice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rola dados virtuais
> Mais informações: <https://manned.org/rolldice>.

#### Rola um dado de 20 lados:
```shell
rolldice d{{20}}
```
#### Rola dois dados de seis lados e descarta o menor valor:
```shell
rolldice {{2}}d{{6}}s{{1}}
```
#### Rola dois dados de vite lados e adiciona um modificador ao resultado:
```shell
rolldice {{2}}d{{20}}{{+5}}
```
#### Rola um dado de vinte lados duas vezes:
```shell
rolldice {{2}}xd{{20}}
```
{% endraw %}{% raw %}
<h2 id="top">
  <a href="/pt_br/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para exibir informações, em tempo real, sobre os processos em execução.

#### Iniciar top:
```shell
top
```
#### Exibir apenas os processos ativos:
```shell
top -i
```
#### Exibir os processos de um usuário específico:
```shell
top -u {{username}}
```
#### Exibir o(s) processo(s) de um ou mais PID específico(s), separado(s) por vírgula:
```shell
top -p {{PID1,PID2,PID3}}
```
#### Mostra Ajuda sobre os comandos disponíveis:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/pt_br/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe o conteúdo do diretório atual em formato de árvore.
> Mais informações: <https://guialinux.uniriotec.br/tree/>.

#### Exibe os arquivos e diretórios de acordo com o nível de profundidade 'num' informado (onde 1 significa o diretório atual):
```shell
tree -L {{num}}
```
#### Exibe apenas diretórios:
```shell
tree -d
```
#### Inclui a exibição de arquivos ocultos com colorização diferenciada:
```shell
tree -a -C
```
#### Exibe a árvore sem identação, mostrando o caminho completo (usar `-N` para não escapar espaços em branco e caracteres especiais):
```shell
tree -i -f
```
#### Exibe o tamanho de cada arquivo e o tamanho acumulado de cada diretório, em um formato de leitura para humanos:
```shell
tree -s -h --du
```
#### Exibe arquivos em uma árvore hierárquica, utilizando um padrão coringa, e eliminando diretórios que não contêm arquivos correspondentes ao informado:
```shell
tree -P '{{*.txt}}' --prune
```
#### Exibe diretórios em uma árvore hierárquica, utilizando um padrão coringa, e eliminando diretórios que não possuem ancestrais do informado:
```shell
tree -P {{nome_diretorio}} --matchdirs --prune
```
#### Exibe a árvore ignorando os diretórios informados:
```shell
tree -I '{{nome_diretorio1|nome_diretorio2}}'
```
{% endraw %}{% raw %}
<h2 id="watch">
  <a href="/pt_br/linux/watch.html">watch</a> <a href="#watch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executa um comando repetidas vezes, e monitora a saída em tela cheia.

#### Monitora arquivos no diretório atual:
```shell
watch {{ls}}
```
#### Monitora espaço em disco e destaca as alterações:
```shell
watch -d {{df}}
```
#### Monitora processos "node", atualizando a cada 3 segundos:
```shell
watch -n {{3}} "{{ps aux | grep node}}"
```
{% endraw %}{% raw %}
<h2 id="wtf">
  <a href="/pt_br/linux/wtf.html">wtf</a> <a href="#wtf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra a expansão de acrônimos.
> Mais informações: <https://manpages.debian.org/bsdgames/wtf.6.en.html>.

#### Expande um acrônimo:
```shell
wtf {{IMO}}
```
#### Especifica um tipo de busca computacional:
```shell
wtf -t {{comp}} {{WWW}}
```
{% endraw %}