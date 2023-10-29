# Entendendo Scripts no Bash

Aqui vamos relembrar o básico:

- O **shell** é como o intérprete do terminal, entende os comandos.
- **Script** é um arquivo de texto com comandos que você usaria no terminal.
- Quando você digita no terminal, é interativo. Scripts são "não interativos".
- A principal vantagem dos scripts é executar vários comandos de uma vez.

Por exemplo, digamos que você queira rodar esses comandos:

```bash
$ whoami
$ hostname
$ uptime -p
$ uname -rms
```

Eles retornam:

- `whoami` - nome de usuário
- `hostname` - nome do host (máquina)
- `uptime` - tempo que o sistema está ligado
- `uname` - informações do kernel do sistema

Poderia aparecer algo assim:

```bash
$ whoami
arthur
$ hostname
excalibur
$ uptime -p
up 2 weeks, 3 days, 19 hours, 42 minutes
$ uname -rms
Linux 4.19.0-6-amd64 x86_64
```

Para simplificar, crie um **script** com esses comandos:

```bash
#!/usr/bin/env bash

whoami
hostname
uptime -p
uname -rms
```

E execute assim:

```bash
$ ./infos
```

O script faz o trabalho por você.

## 2.2 – Executando Scripts

Quando você executa um script, use `./` se o script estiver na mesma pasta:

```bash
$ ./infos
```

Se o script estiver em outro lugar, forneça o caminho completo ou use o $PATH (falaremos disso depois).

## 2.3 – Cuidados e Boas Práticas

Vamos falar de segurança e organização:

### 2.3.1 – Entenda o que faz

Nunca execute comandos ou scripts sem saber o que eles fazem. Comandos podem ser perigosos. Scripts desconhecidos podem causar problemas. Peça ajuda se necessário.

### 2.3.2 – Preste atenção ao prompt

O símbolo no prompt indica se você está como usuário normal ($) ou administrativo (#). Administrativo pode causar danos. Use o `sudo` com cuidado.

### 2.3.3 – Seja organizado

Crie pastas para seus testes e experimentos. Evite criar scripts em qualquer lugar. Isso mantém as coisas organizadas e evita problemas.

### 2.3.4 – Escolha nomes cuidadosamente

Verifique se os nomes dos scripts não conflitam com comandos existentes. Ao compartilhar scripts, coloque-os nas pastas certas.

### 2.3.5 – Não inclua sua pasta de testes no $PATH

Nunca coloque sua pasta de testes no $PATH. Scripts de testes podem conter erros. Mova-os para um local definitivo quando estiverem prontos.
