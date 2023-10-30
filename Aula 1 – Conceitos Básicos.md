```markdown
# O que é o Shell?

O Shell é uma camada do sistema operacional responsável por criar uma interface entre o usuário e o kernel, geralmente através de um console ou terminal.

Observação: O sistema operacional possui vários componentes, sendo o núcleo o kernel.

O Shell é um interpretador de comandos, o que significa que possui a capacidade de interagir com o sistema. Esses comandos podem ser fornecidos de duas formas: interativamente, através da entrada padrão no terminal, ou de maneira não interativa, através de um arquivo ou script.

Além de interpretar comandos, o Shell também é uma linguagem de programação de alto nível, semelhante a linguagens como JavaScript. Como linguagem de programação, ele oferece manipulação de variáveis, estruturas de controle de fluxo, loops e muitos outros recursos, não deixando nada a desejar em comparação com outras linguagens de programação.

Quando o Shell é iniciado, ele procura as configurações globais do sistema, seguidas das configurações do usuário, e, finalmente, exibe um indicador de comando, que é o prompt de comando, com a seguinte forma padrão:

```
usuario@hostname:~/caminho$
```

Nesse caso, o til (~) representa o caminho abreviado para a pasta pessoal do usuário, que equivale a `/home/usuario/`. Se o usuário estiver em outra pasta dentro da pasta pessoal, o caminho será exibido a partir do til (~), por exemplo: `~/Downloads/wallPapers/`. A menos que o usuário esteja na raiz do sistema, caso em que o caminho será exibido como `/usr/bin/`, sem o til (~).

Após o til (~), temos o símbolo de dólar ($) que indica que estamos executando o Shell como um usuário normal. Caso entremos no modo root (usuário com superpoderes), o símbolo de dólar será substituído por uma cerquilha (#), indicando que estamos em uma área perigosa para quem não está familiarizado com o sistema, pois nesse modo, podemos realizar ações críticas.

O Bash (Bourne Again Shell) possui comandos internos (built-in) e também faz uso de utilitários externos. É importante dar preferência aos comandos internos, pois eles tornam os comandos e scripts muito mais rápidos e eficientes devido à integração profunda com o sistema.

Para listar os comandos internos disponíveis, você pode utilizar o seguinte comando:

```bash
$ help
```

Este comando irá listar todos os comandos internos do sistema. Você também pode usar o comando `help` com um comando específico para saber se ele é um comando interno e, caso seja, ele exibirá um pequeno manual de instruções do comando.

Outra maneira de determinar qual tipo de shell está em uso é através de dois métodos:

**Método 1:** Utilizando o comando `echo $0`. A variável `$0` armazena o nome do programa em execução, no entanto, deve-se ter cuidado ao usar esse método com scripts, pois ele mostrará o nome do script em execução, não o shell.

**Método 2:** Utilizando o comando `echo $SHELL`. Essa variável de ambiente armazena o shell definido para o usuário que está logado e pode ser chamada de qualquer lugar, sempre exibindo a informação do shell.

Para fins de curiosidade, o comando `echo` é um comando interno do Shell que escreve argumentos na saída padrão, ou seja, o que será exibido na tela do terminal.
```
