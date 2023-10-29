# Introdução ao Shell, Terminais e Consoles, Prompt de Comandos, Tipos de Shell e Comandos Builtin

Neste texto, vamos explorar o mundo do shell, a interface técnica e descontraída que nos permite interagir com o sistema operacional. Mesmo que você não seja um programador experiente, se já usou o terminal no Linux, Mac ou console no Windows, você usou um shell.

## 1.1 - O que é o 'shell'

Mesmo que você nunca tenha criado nenhum script, mesmo que não saiba nada de programação, se você usa o terminal ou o console de qualquer distribuição GNU/Linux, ou o terminal do seu Mac, ou até o console do Windows, você já está utilizando algum tipo de shell.

**Exemplo de comando:**
```shell
$ ls -l
```
No exemplo acima, "ls -l" é um comando executado no shell para listar os arquivos no diretório atual.

## 1.2 - Terminais e consoles

Nos tempos mais remotos da computação, a comunicação física entre o usuário e o kernel era feita através da entrada de comandos por fitas ou cartões perfurados, com ou sem a ajuda de um teclado, e do recebimento de respostas através de uma impressora.

**Exemplo de comando:**
```shell
$ echo "Hello, World!"
```
No comando acima, "echo" é usado para exibir "Hello, World!" no terminal.

## 1.3 - O 'prompt' de comandos

Assim que você faz o login no console ou abre um terminal no seu ambiente gráfico, o shell é iniciado e nos mostra um ou mais caracteres e um cursor no local onde serão exibidos os comandos digitados por nós. Este ponto onde aparece o cursor é o prompt de comandos. Sua função é indicar que o shell está "pronto" (daí prompt) para receber comandos. Na verdade, podemos dizer que acessar o prompt de comandos é o mesmo que acessar o shell.

**Exemplo de comando:**
```shell
$ cd /home/user/documents
```
Nesse exemplo, o comando "cd" é usado para mudar o diretório atual para "/home/user/documents".

## 1.4 - A aparência do 'prompt'

Dependendo do sistema operacional e das customizações feitas, o prompt pode apresentar várias informações, mas o que importa para nós por enquanto são os símbolos mostrados imediatamente antes do cursor.

**Exemplo de prompt:**
```
user@machine:~$
```

## 1.5 - Shell interativo e não-interativo

Quando abrimos um terminal e começamos a digitar comandos, nós estamos utilizando o shell de forma interativa. No modo interativo, nós entramos com um comando, o shell processa esse comando, nos dá uma resposta, nós vemos a resposta, pensamos e decidimos o que fazer em seguida.

**Exemplo de shell não-interativo:**
```shell
$ sh myscript.sh
```

## 1.6 - Tipos de shell

Existem vários tipos de shell, figurando entre eles:

- Bourne Shell (sh)
- Bourne-Again Shell (bash)
- Almquist Shell (ash)
- Debian Almquist Shell (dash)
- KornShell (ksh)
- Z Shell (zsh)

**Exemplo de mudança de shell:**
```shell
$ chsh -s /bin/bash
```

## 1.7 - Os comandos builtin do Bash

O bash possui um farto conjunto de comandos internos chamados de builtin, e nós utilizamos alguns deles bem frequentemente no terminal, como é o caso do comando cd, usado para mudar de diretório.

**Exemplo de comando builtin:**
```shell
$ cd /path/to/directory
```

## 1.8 - Como saber que tipo de shell você está utilizando

Você pode descobrir o shell atual de duas maneiras. Uma é usando o comando 'echo $0' no modo interativo, mas ele não funciona dentro de scripts. Outra é usando 'echo $SHELL', que retorna o caminho do shell configurado para o usuário e funciona em scripts.

**Exemplo de comando para verificar o shell atual:**
```shell
$ echo $SHELL
```

Lembre-se de que essas são as formas mais simples de identificar o shell e que existem outras maneiras mais avançadas.
