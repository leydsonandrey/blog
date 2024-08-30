![](https://github.com/leydsonandrey/blog/blob/main/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/banner.png?raw=true)

###### Como sincronizar arquivos entres diversos dispositivos, de forma fácil e gratuita.

Se você precisa sincronizar arquivos entre diversos dispositivos, a melhor forma é usando o [Syncthing](https://syncthing.net/). Ele possibilita a sincronização entre [diversos dispositivos](https://syncthing.net/downloads/): Android, Windows, Linux e MacOS. E a sincronização é feita de forma privada e segura:

- **Privado**: Nenhum dos seus dados é armazenado em nenhum outro lugar além dos seus computadores. Não há um servidor central que possa ser comprometido, legal ou ilegalmente.
- **Criptografado**: Toda a comunicação é protegida usando TLS. A criptografia usada inclui perfect forward secrecy para evitar que qualquer bisbilhoteiro tenha acesso aos seus dados.
- **Autenticado**: Cada dispositivo é identificado por um certificado criptográfico forte. Apenas dispositivos que você permitiu explicitamente podem se conectar aos seus outros dispositivos.

Além de ser [Open-source](https://github.com/syncthing/syncthing). 😀

## Instalando o Syncthing no Windows 10

Baixe o executável do Syncthing: https://syncthing.net/downloads/

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/1.png?raw=true)

Ao acessar o link, você será redirecionado para o GitHub do [Syncthing Windows Setup](https://github.com/Bill-Stewart/SyncthingWindowsSetup/):

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/2.png?raw=true)

Clique em [Releases](https://github.com/Bill-Stewart/SyncthingWindowsSetup/releases) para acessar as últimas versões do programa.

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/3.png?raw=true)

Clique em cima de `syncthing-1.27.10-setup.exe` para baixar o executável do programa. Essa é a última versão disponível até o momento (29 de agosto de 2024).

Ao executar o executável, essa tela aparecerá:

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/4.png?raw=true)

A primeira é para instalar apenas para o seu usuário, a segunda é para instalar para todos os usuários. **Escolherei a primeira opção, mas isso não influenciará em nada no tutorial**.

Após escolher a opção desejada, aceite os termos clicando em **Next**; Na próxima tela, selecione o local de instalar ou clique em **Next** para deixar a padrão e seguir para a próxima tela; E, por fim, Clique em **Next** novamente.

Agora vem a parte importante:

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/5.png?raw=true)

Nessa tela estão informações importantes sobre as configurações do Syncthing.

O Syncthing conta com uma GUI, **que será executado no endereço do segundo campo na porta do terceiro campo**. Deixarei os valores padrões. **Guarde os valores, se você os modificar**.

URL padrão: https://127.0.0.1:8384

Aí, é só clicar em **Next**, **Next**, **Install** e **Confirmar** a caixa de diálogo “Create Windows Firewall rule for Syncthing?”. E, finalmente, a última tela mostrando que a instalação do Syncthing foi concluída. Marque a caixa “Open Synching configuration page”, isso abrirá o GUI no URL acima (ou no endereço e porta selecionado).

Após instalado, pesquise pelo `Start Syncthing` no iniciar (clique no botão Windows e digite o nome) e execute-o. Se o Syncthing já estiver rodando, irá aparecer uma caixa de diálogo com “Syncthing is alright running.”.

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/6.png?raw=true)

## Instalando no Linux

### Debian, Ubuntu e derivados

``` bash
sudo apt install syncthing
```

[Mais informações](https://apt.syncthing.net/)

### Arch Linux e derivados

``` bash
sudo pacman -S syncthing
```

### Outros

[Para mais opções de Downloads acesse esse link.](https://syncthing.net/downloads/#base-syncthing)

### Syncthing Tray no linux

GUI feita com Python e GTK, que possibilita o Tray:

- Github: https://github.com/kozec/syncthing-gtk
- Flathub: https://flathub.org/apps/me.kozec.syncthingtk

### Executando o Syncthing

Você pode executar pelo menu do seu sistema `Start Syncthing` ou `Syncthing Web UI`, ou executando pelo terminal:

#### Executar com GUI

``` bash
syncthing
```

#### Executar sem GUI

``` bash
syncthing --no-browser
```

No Linux, o GUI também roda no endereço https://127.0.0.1:8384 por padrão. 

## Instalando no Android

O Syncthing pode ser baixado pela [Google Play Store](https://play.google.com/store/games) ou pelo [F-Droid](https://f-droid.org/):

- Google Play Store: https://play.google.com/store/apps/details?id=com.nutomic.syncthingandroid
- F-Droid: https://f-droid.org/packages/com.nutomic.syncthingandroid/

## Como usar essa bagaça?

Primeiro, é preciso adicionar uma pasta:

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/7.png?raw=true)
![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/8.png?raw=true)

1. Rótulo da pasta

Uma descrição de sua preferência para a pasta. **Recomendo deixar em branco**.

2. ID da pasta

ID pode ser resumido ao nome da pasta — a pasta que será sincronizada. 

3. Caminho da pasta

PATH da pasta, se a pasta não existe, será criada uma nova.

Ao salvar, a pasta estará pronta para a sincronização. Agora é só adicionar um dispositivo e compartilhar a pasta com ele.

### Como adicionar um dispositivo?

Adicionarei meu celular e compartilharei uma pasta com ele.

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/9.png?raw=true)

<sup>Criei essa pasta com o ID `pasta` e deixei o rótulo em branco.</sup>

Click no botão “Adicionar dispositivo remoto”:

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/10.png?raw=true10.png)

E adicione o ID do seu dispositivo e um nome qualquer:

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/11.png?raw=true)

#### Como saber meu ID?

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/12.png?raw=true)

**[(Click aqui para ver o tutorial de como ver o ID no celular)](https://youtube.com/shorts/sQPjSO1jA7Q?feature=share)**


#### Aceitando pedido no Android
| | |
| --- | --- |
| ![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/13.png?raw=true)| ![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/14.png?raw=true) |

<sup>\*Click em aceitar!</sup>

#### Aceitando no PC

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/15.png?raw=true)

#### Compartilhando a pasta entre dispositivos

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/16.png?raw=true)

E marque o dispositivo desejado:

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/17.png?raw=true)

#### Aceitando a pasta no Android

![](https://github.com/leydsonandrey/blog/blob/00d3b80bf424cde9a0d113d2ff22e702c9ba1b6d/Sincroniza%C3%A7%C3%A3o%20de%20Arquivos%20entre%20PC%20e%20Celular:%20Syncthing/18.png?raw=true)

#### Aceitando a pasta no PC

No PC é dá mesma forma que aceita um dispositivo.

## Finalmente acabou :)

**Com isso, você já consegue usar o Syncthing de forma aceitável**. Lembre-se de esperar a sincronização ser concluída para evitar corromper os arquivos.

### Dica: use git para versionamento da pasta.

Script em Bash que uso para fazer commits rapidamente:

``` bash
#!/bin/bash

# Adiciona todos os arquivos modificados ao stage
git add .

# Obtém a data e hora atual no formato desejado para o commit
datahora=$(date +'%Y-%m-%d %H:%M:%S')

# Faz o commit com a mensagem contendo a data e hora atual
git commit -m "Update $datahora" -m "Arquivos modificados:
$(git diff --name-only --cached)"
```
