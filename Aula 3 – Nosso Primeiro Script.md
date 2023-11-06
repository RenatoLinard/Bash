# Nosso Primeiro Script

## A Criação de um Script no Bash

A criação de um arquivo script no Bash envolve basicamente três etapas: criação, edição e tornar o arquivo executável.

1. **Criação do Arquivo:**

    - O nome do arquivo deve obedecer a algumas regras básicas para evitar problemas durante a criação e execução. São elas:

        - Utilize apenas caracteres minúsculos de "a" a "z" sem acentuação.

        - Os únicos caracteres especiais permitidos são o hífen (-), o sublinhado (_) e o ponto (.).

        - Evite criar nomes de scripts com espaços entre palavras.

        - Extensões no final do nome do arquivo não possuem finalidade no shell. Se desejar usar uma extensão, isso não afetará a execução do script.

        - Seja organizado ao criar seus scripts de testes. Crie pastas e subpastas para cada assunto em estudo.

        - Caso a pasta onde o script está localizado não esteja configurada no PATH, lembre-se de chamá-los com o caminho completo. Por exemplo, se o script estiver no diretório onde você se encontra, utilize apenas `./meu_script`. Se estiver em um diretório diferente, use `~/Bash/meu_script`.

        - Se desejar atribuir o diretório no PATH, basta reescrever a variável PATH da seguinte forma: `PATH=$PATH:~/Bash/meu_script`. No entanto, lembre-se de que essa atribuição será temporária e será perdida quando a sessão do shell for encerrada. Para torná-la permanente, você deve configurar o PATH diretamente no arquivo `.bashrc` ou `.bash_profile` da seguinte maneira:

        ```bash
        export PATH=$PATH:~/Bash/meu_script
        ```

    - Para criar o arquivo, você pode utilizar o redirecionamento de saída da seguinte forma: `> meu_script`, onde basicamente você está direcionando a saída de um comando para dentro de um arquivo. Neste caso, não estamos definindo nenhum comando, portanto o arquivo é criado vazio.
