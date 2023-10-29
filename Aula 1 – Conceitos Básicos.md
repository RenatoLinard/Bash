# Anotações sobre Shells, Terminais, Prompt de Comandos e Tipos de Shells

Ei pessoal, aqui estão algumas anotações sobre shells, terminais, prompts de comandos e tipos de shells. 😎

## 1.1 - O que é o 'shell'

Então, mesmo que você não seja um guru da programação, se você já usou o terminal no Linux, Mac ou o console no Windows, você está lidando com algum tipo de shell. O shell é como uma camada que envolve o sistema operacional, agindo como uma "casca". Sua principal função é criar uma interface entre você, o usuário, e o núcleo do sistema, conhecido como kernel. O kernel cuida da parte física do seu computador, enquanto o shell lida com as instruções dos programas e, claro, com as suas.

**Exemplo técnico:** Se você executar `ls -l`, você está usando o shell para listar os arquivos no diretório.

## 1.2 - Terminais e consoles

No passado, a comunicação entre o usuário e o kernel era feita através de cartões perfurados ou fitas. Com o tempo, as coisas evoluíram, e os consoles e terminais eletrônicos se tornaram virtuais. Agora, quando falamos em "console" ou "terminal", estamos falando sobre a virtualização em software (graças ao kernel) dos antigos terminais físicos.

**Exemplo técnico:** Quando você executa o comando `echo "Hello, World!"`, está usando o shell para exibir uma mensagem no terminal.

## 1.3 - O 'prompt' de comandos

Assim que você entra no console ou abre um terminal, o shell é iniciado, e você vê um prompt de comandos. É o local onde você digita seus comandos. Acessar o prompt de comandos é essencialmente acessar o shell.

**Exemplo técnico:** Ao usar comandos como `cd /home/user/documents`, você está navegando entre diretórios no shell.

## 1.4 - A aparência do 'prompt'

O prompt pode variar de acordo com o sistema e as configurações. Normalmente, você verá símbolos como `$`, `%`, ou `#` antes do cursor. Cada símbolo tem um significado. O `$` indica que você está logado como usuário comum, o `#` indica que você está como usuário administrativo (o temido root).

**Exemplo técnico:** O prompt `user@machine:~$` mostra o nome de usuário, o nome da máquina, o diretório atual e o tipo de usuário.

## 1.5 - Shell interativo e não-interativo

Quando você está no terminal, está interagindo diretamente com o shell. Você digita um comando, o shell processa, você vê a resposta e decide o próximo passo. Mas você também pode usar o shell de forma não interativa, o que é útil quando você precisa executar uma série de comandos em sequência.

**Exemplo técnico:** Para executar um script, você pode usar o comando `sh myscript.sh`.

## 1.6 - Tipos de shell

Existem vários tipos de shell por aí, como o Bourne Shell, Bourne-Again Shell, Almquist Shell, Debian Almquist Shell, KornShell e Z Shell, entre outros. Cada um tem suas próprias características e comandos.

**Exemplo técnico:** Para mudar o shell padrão, você pode usar `chsh -s /bin/bash`.

## 1.7 - Os comandos builtin do Bash

O Bash possui muitos comandos internos, chamados de "builtin". Alguns deles são frequentemente usados no terminal. O comando `cd`, por exemplo, é um comando interno que permite mudar de diretório.

**Exemplo técnico:** Para navegar entre diretórios, use o comando `cd /path/to/directory`.

## 1.8 - Como saber que tipo de shell você está utilizando

Você pode verificar qual shell está em uso de algumas maneiras. Uma delas é usar o comando `echo $0` no modo interativo. Mas lembre-se de que isso não funciona dentro de scripts. Outra maneira é verificar a variável de ambiente `$SHELL`, que armazena o caminho do shell configurado para o usuário.

**Exemplo técnico:** Para verificar o shell atual, use o comando `echo $SHELL`.

Então, pessoal, essas são algumas anotações sobre shells e terminais. Espero que isso ajude você a entender melhor como interagimos com nossos sistemas! 😄✨
