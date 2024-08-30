Como sincronizar arquivos entres diversos dispositivos, de forma fácil e gratuita.

Se você precisa sincronizar arquivos entre diversos dispositivos, a melhor forma é usando o Syncthing. Ele possibilita a sincronização entre diversos dispositivos: Android, Windows, Linux e MacOS. E a sincronização é feita de forma privada e segura:

- Privado. Nenhum dos seus dados é armazenado em nenhum outro lugar além dos seus computadores. Não há um servidor central que possa ser comprometido, legal ou ilegalmente.
- Criptografado. Toda a comunicação é protegida usando TLS. A criptografia usada inclui perfect forward secrecy para evitar que qualquer bisbilhoteiro tenha acesso aos seus dados.
- Autenticado. Cada dispositivo é identificado por um certificado criptográfico forte. Apenas dispositivos que você permitiu explicitamente podem se conectar aos seus outros dispositivos.

Além de ser open-source. 😀

## Instalando o Syncthing no Windows 10

Baixe o executável do Syncthing: https://syncthing.net/downloads/

Ao acessar o link, você será redirecionado para o GitHub do Syncthing Windows Setup:

Clique em Releases para acessar as últimas versões do programa.

Clique em cima de syncthing-1.27.10-setup.exe para baixar o executável do programa. Essa é a última versão disponível até o momento (29 de agosto de 2024).

Ao executar o executável, essa tela aparecerá:

A primeira é para instalar apenas para o seu usuário, a segunda é para instalar para todos os usuários. Escolherei a primeira opção, mas isso não influenciará em nada no tutorial.

Após escolher a opção desejada, aceite os termos clicando em Next; Na próxima tela, selecione o local de instalar ou clique em Next para deixar a padrão e seguir para a próxima tela; Clique em Next para novamente.

Agora vem a parte importante:

Nessa tela estão informações importantes sobre as configurações do Syncthing.

O Syncthing conta com uma GUI, que será executado no endereço do segundo campo na porta do terceiro campo. Deixarei os valores padrões. Guarde os valores, se você os modificar.

URL padrão: https://127.0.0.1:8384

Aí, é só clicar em Next, Next, Install e Confirmar a caixa de diálogo "Create Windows Firewall rule for Syncthing?". E, finalmente, a última tela mostrando que a instalação do Syncthing foi concluída. Marque a caixa "Open Synching configuration page", isso abrirá o GUI no URL acima (ou no endereço e porta selecionado).

Após instalado, pesquise pelo Start Syncthing no iniciar (clique no botão Windows e digite o nome) e execute-o. Se o Syncthing já estiver rodando, irá aparecer uma caixa de diálogo com "Syncthing is alright running.".
