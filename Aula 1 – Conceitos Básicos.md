```markdown
# Introdução ao Shell

O Shell é uma parte essencial do sistema operacional que permite aos usuários interagirem com o sistema. Ele serve como uma interface entre você e o núcleo do sistema operacional, normalmente através de um console ou terminal.

- O Shell é um **interpretador de comandos**, o que significa que ele pode executar comandos quando você os digita no terminal.

- Esses comandos podem ser inseridos interativamente, enquanto você digita no terminal, ou podem ser armazenados em um arquivo (script) para execução não interativa.

- Além de interpretar comandos, o Shell também é uma linguagem de programação de alto nível, semelhante a linguagens como JavaScript. Isso significa que você pode escrever scripts para automatizar tarefas e controlar o fluxo de execução.

## Entendendo o Prompt

Quando você inicia o Shell, ele exibe um indicador de comando conhecido como **prompt**. O prompt padrão geralmente se parece com isso:

```
usuario@hostname:~/caminho$
```

- O til (~) representa o caminho da pasta pessoal do usuário, abreviado, que é equivalente a `/home/usuario/`. Se você estiver em uma subpasta, o caminho será exibido a partir do til, por exemplo: `~/Downloads/wallPapers/`.

- Se você estiver na raiz do sistema, o caminho será exibido como `/usr/bin/`.

- O símbolo de dólar ($) indica que você está executando o Shell como um usuário normal. Se você entrar no modo root (usuário com privilégios elevados), o símbolo de dólar será substituído por uma cerquilha (#).

## Comandos Integrados e Utilitários Externos

O Shell possui **comandos integrados (built-in)** que são parte do próprio Shell e **utilitários externos** que são programas separados. É importante dar preferência aos comandos integrados, pois eles são mais eficientes e rápidos devido à sua integração com o Shell.

Para listar os comandos integrados disponíveis, você pode usar o comando `help`:

```bash
$ help
```

Isso mostrará uma lista de todos os comandos internos do Shell. Você também pode usar o `help` com um comando específico para obter informações sobre ele.

## Identificando o Tipo de Shell

Você pode determinar o tipo de Shell que está em uso de duas maneiras:

**Método 1:** Usando o comando `echo $0`. Essa variável especial armazena o nome do programa em execução, mas tenha cuidado ao usá-la com scripts, pois mostrará o nome do script em execução, não o Shell em uso.

**Método 2:** Usando o comando `echo $SHELL`. Esta variável de ambiente armazena o Shell definido para o usuário logado e pode ser acessada de qualquer lugar.

Por fim, o comando `echo` é um comando interno do Shell que escreve argumentos na saída padrão, ou seja, o que é exibido na tela do terminal.
```
