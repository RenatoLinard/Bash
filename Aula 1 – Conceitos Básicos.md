# O que é o Shell/Bash?

O **Shell** é uma camada do sistema operacional responsável por criar uma interface entre o usuário e o núcleo (kernel), geralmente por meio de um console ou terminal.

> **Observação:** O sistema operacional possui vários componentes, sendo o núcleo (kernel) um deles.

O Shell atua como um interpretador de comandos, o que lhe confere a capacidade de interação com o sistema. Esses comandos podem ser fornecidos de duas maneiras: através de entrada padrão (interativamente, digitando comandos no terminal) ou por meio de um arquivo/script (modo não-interativo).

Além de interpretar comandos, o Shell também funciona como uma linguagem de programação de alto nível, semelhante a linguagens como JavaScript. Ele possui recursos como manipulação de variáveis, estruturas de controle de fluxo, laços de repetição e muito mais, não ficando atrás de outras linguagens de programação.

Ao iniciar o Shell, ele procura as configurações globais do sistema e, em seguida, as configurações específicas do usuário. Por fim, ele exibe um indicador de comando, que segue o formato padrão:

```bash
usuario@hostname:~/caminho$
```

Neste caso, o til (~) representa o caminho para a pasta pessoal, abreviando `/home/renatolinard/`. Se você navegar para uma subpasta dentro da pasta pessoal, o caminho será relativo ao til, por exemplo: `~/Downloads/wallPapers/`. No entanto, se você estiver na raiz do sistema, o caminho será exibido da seguinte forma: `/usr/bin/`, sem o til.

Após o til (~), encontramos o símbolo de dólar ($), que indica que estamos executando o Shell como um usuário normal. Se entrarmos no modo root (usuário com privilégios elevados), o símbolo $ será substituído por um sustenido (#), indicando que estamos em uma área crítica, onde é possível realizar operações que podem afetar o sistema.

O **Bash** (Bourne Again Shell), um dos shells mais populares, inclui comandos *built-in* e utiliza utilitários. É importante dar preferência aos comandos *built-in*, pois eles tornam os comandos e scripts mais rápidos e eficientes, uma vez que estão altamente integrados ao sistema.

Para listar os comandos *built-in* disponíveis, podemos utilizar o comando `help` da seguinte forma:

```bash
$ help
```

Isso listará todos os comandos *built-in* do sistema. Além disso, é possível usar o `help` com um comando específico para verificar se ele é *built-in* e também para exibir um pequeno manual de instruções do comando, caso ele seja *built-in*.

Outra maneira de determinar o tipo de shell que estamos usando é através de duas abordagens:

**Método 1:** Utilizando `echo $0`. A variável especial `$0` armazena o nome do programa em execução. No entanto, ao chamar esse comando de um script, ele mostrará o nome do script, não o shell utilizado.

**Método 2:** Utilizando `echo $SHELL`. Esta variável de ambiente armazena o shell definido para o usuário logado e pode ser chamada de qualquer lugar, sempre contendo a informação do shell definido.

A título de curiosidade, o comando `echo` é um comando *built-in* do Shell, utilizado para escrever argumentos na saída padrão, ou seja, o que é exibido na tela do terminal.
