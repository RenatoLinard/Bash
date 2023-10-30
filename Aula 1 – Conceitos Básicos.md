# Introdução ao Shell

O **Shell** é uma camada essencial do sistema operacional que proporciona uma interface entre os usuários e o kernel, geralmente por meio de um console ou terminal. Antes de aprofundarmos, é importante ressaltar que o sistema operacional é composto por diversos componentes, sendo o núcleo, conhecido como *kernel*, um deles.

## Funcionalidades do Shell

O Shell desempenha duas funções principais:

1. **Interpretação de Comandos:** O Shell é um interpretador de comandos, o que significa que ele é capaz de compreender e executar comandos fornecidos pelos usuários. Esses comandos podem ser inseridos de duas maneiras principais:

   - **Entrada Padrão (Interativa):** Nesse modo, os comandos são inseridos diretamente no terminal, permitindo uma interação ativa com o sistema operacional.

   - **Arquivos/Scripts (Não-Interativa):** Os comandos podem ser armazenados em arquivos ou scripts, que são posteriormente executados pelo Shell. Isso é útil para automatizar tarefas e processos complexos.

2. **Linguagem de Programação de Alto Nível:** Além de interpretar comandos, o Shell também funciona como uma linguagem de programação de alto nível, semelhante a linguagens como JavaScript. Ele oferece recursos avançados, incluindo:

   - **Manipulação de Variáveis:** Permite a definição e manipulação de variáveis para armazenar informações temporárias.

   - **Estruturas de Controle de Fluxo:** Você pode utilizar estruturas condicionais e de repetição para controlar o fluxo de execução dos comandos.

   - **Laços de Repetições:** O Shell permite criar loops para executar um conjunto de comandos repetidamente.

## Prompt de Comando

Quando você inicia o Shell, ele segue um processo para exibir o *prompt de comando*. Primeiro, ele procura as configurações globais do sistema, depois as configurações específicas do usuário. Finalmente, ele exibe o prompt de comando, que tem o seguinte formato padrão:

```
usuario@hostname:~/caminho$
```

- O til (~) representa o caminho para a pasta pessoal do usuário, equivalente a `/home/nome_do_usuário/`.

Se você navegar para uma subpasta dentro da sua pasta pessoal, o caminho aparecerá a partir do til (~), por exemplo:

```
~/Downloads/wallPapers/
```

Entretanto, se você estiver na raiz do sistema, o caminho será exibido da seguinte maneira:

```
/usr/bin/
```

Em resumo, o Shell é uma ferramenta poderosa que desempenha um papel crucial na interação com o sistema operacional. Além de interpretar comandos, ele oferece recursos de programação de alto nível e fornece um indicador de comando personalizável, tornando-o uma ferramenta versátil para usuários e programadores.
