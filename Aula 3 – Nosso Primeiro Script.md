# Aula 3 - Nosso Primeiro Script

Aqui estão algumas anotações pessoais sobre a terceira aula do curso básico de bash.

## Etapas para Criar um Script

### 1. **Crie o Arquivo do Script**

   - Comece criando um arquivo de texto simples.
   - Não use espaços, acentos ou caracteres especiais no nome do arquivo.
   - Opcionalmente, adicione a extensão .sh para indicar que é um script.
   
### 2. **Edite o Arquivo do Script**

   - Abra o arquivo em um editor de texto ou use o comando `nano`.
   - Aqui é onde você escreverá o código do seu script.

### 3. **Torne o Arquivo Executável**

   - Use o comando `chmod +x nome_do_arquivo` para tornar o arquivo executável.

## Nome e Diretório

- Pense bem no nome do arquivo, pois ele é crucial.
- Evite usar espaços ou caracteres especiais no nome.
- Extensões, como .sh, são úteis para identificar scripts.
- Considere onde deseja criar o arquivo, preferencialmente em pastas no seu PATH ou caminhos personalizados.

## Criação de Arquivo pelo Terminal

- Você pode criar um arquivo diretamente no terminal usando comandos de redirecionamento.
- Utilize `>` para criar um novo arquivo ou sobrescrever se já existir.
- Use `>>` para acrescentar ao final de um arquivo existente.

## Escrevendo o Conteúdo do Script

- A primeira linha deve conter o interpretador de comandos, geralmente `#!/usr/bin/env bash`.
- Definir o interpretador é fundamental para evitar erros.
- Use comandos como `echo` para produzir saídas e executar tarefas.

## Tornando o Arquivo Executável

- Garanta que seu arquivo seja executável usando `chmod +x nome_do_arquivo`.
- Verifique as permissões com `ls -l nome_do_arquivo`.

## Verificando se o Arquivo é Executável

- Use o comando `test -x nome_do_arquivo; echo $?` para verificar a executabilidade.
- Se for executável, o resultado será 0; caso contrário, será um número diferente.

## Criando um Script para Criar Scripts

- Você pode simplificar o processo de criação de scripts criando um script para isso.
- Evite sobrescrever acidentalmente arquivos existentes.
- Certifique-se de que há exatamente um argumento para o nome do arquivo.
- Use `$#` para contar os argumentos passados.
- Utilize `[[ -f $1 ]]` para verificar se o arquivo já existe.

Sendo assim, vamos incluir mais uma linha antes das outras no nosso script:

```bash
#!/usr/bin/env bash

[[ $# -ne 1 ]] && echo "Digite o nome de apenas um arquivo! Saindo..." && exit 1

[[ -f $1 ]] && echo "Arquivo já existe! Saindo..." && exit 1

echo '#!/usr/bin/env bash' >> $1
chmod +x $1
nano $1
```

Agora você tem as bases para começar a criar e gerenciar scripts em Bash. Divirta-se automatizando tarefas e simplificando seu trabalho! 😄🚀
