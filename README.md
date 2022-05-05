# Guia de Comando Línux Essencial 🐧

## Diferenças entre usuários 🧑
- `$` Usuário comum
- `#` Super Usuário
## Diretórios do Línux FSH (File System Hierachy Standart) 🎯
- `/` Raiz do Sistema Operacional
- `/boot` Contém arquivos necessários para a `iniciação do sistema`.
- `/etc` Arquivos de `configuração do sistema` e de `serviços de redes` (pacotes) `instalados` (por padrão).
- `/bin` Contém os programas/comandos básicos do sistema para uso dos usuários. 
- `/sbin` Contém os `programas` /` comandos acessíveis` pelo `superusuário` (root) para a `administração do sistema`. 
- `/var` Contém os `logs do sistema` e `dados de spool` de empressora e cache.
- `/root` Diretório do `usuário root`, o `administrador de sistema`.
- `/home` Diretório que contém os `subdiretórios` de cada `usuário`.
- `/dev`  Permite o acesso aos `dispositivos de sistema`.
- `/lib` Bibliotecas Compartilhadas pelos `programas do sistema` e `módulos do Kernel`.
- `/proc` Sistemas de arquivos do `Kernel`. Esse diretório `não existe` em seu disco rígido, ele é `criado` pelo `Kernel` e usado em diversos programas que fazem a sua `leitura`. Através do seu conteúdo podemos verificar `configurações do sistema` ou `modificar o funcionamento` de `dispositivos` através de alterações em seus `arquivos`.
- `/usr` Contém arquivos e aplicativos de `usuários do sistema`, `documentações do sistema` entre outros tipo de arquivo.

## Formatação do teclado para o padrão adotado no Brasil 🧐

- `loadkeys br -abnt2`

## Comandos de movimentação e interação com os diretórios 🚶

- `cd /` Utilizado para `navegar entre diretórios`.
- `cd ..` Utilizamos para retrair ao `diretório anterior`.
- `TAB` Alto completa comandos.
- `pwd` utilimos para saber em `qual diretório estmos`.
- `ls` Utilizamos para `listar arquivos`.
- `history` Utilizamos para acessar o `histórico`.
- `CTRL + R` Executa uma busca de `comandos já executados`.
- `~` Diretório pessoal do `usuário`.
- `CTRL +L` Limpa a tela do termina.

## Dicas modo de texto 📑

### GUI vs CLI 🖥️
- GUI - Graphical User Interface  
- CLI - Command Line Interface  

### Alterar entre terminais de texto ⌨️
- `ALT + F1-F6` Terminais no modo texto.
- `ALT F7*` Teminal no modo gráfico.

### Alterar do terminal gráfico para o modo texto 👨‍💻
- `exit`
- `logout`
- `CTRL + D`

### Comandos para desligar o sistema 🔌
- `shutdown -h now`
- `init 0`
- `halt`
- `poweroff`

### Comandos para reiniciar o sistema 🔄
- `rebooy`
- `init 6`
- `CTRL + ALT + DEL`

## GNU / Linux - SHELL ⬛

Os comandos do interpretador `Bash`, possuem características parecidas, das quais podemos ressaltar:
- Sintaxe `comando <opção> <argumento>`
- Exemplo: `ls -l /etc`
- Shell Script é uma linguagem Case Sensitive (Tem diferenças entre maiúsculas e minúsculas), e na maioria dos casos as sintaxes são minúsculas.

 ## Comandos de orientação e ajuda 🆘
 - `man` Exibe um manual sobre o comando desejado.
 - `--help` Normalmente utilizado como parâmetro, e discreve mais atentamente sobre o comando desejado.
 - `info` Varia com a distribuição utilizada porém funciona da mesma forma que o man.

 ## Manipulação de data e hora 📅
- `cal` Exibe o calendário de um mês/ano desejado.
- `date` Exibe ou altera a data e a hora do sistema.

## Privilégios do usuário 👨‍🎓
- `sudo` - Permite executar programas c/ privilégios de outro usuário - (por padrão, como o root). 
`sudo` significa "substitute user do" (usuário 
  substituto faça)  

## Listagem e manipulação de diretórios 🗂️

- `cd` - change directory
  - `.` - diretório atual
  - `..` - diretório acima
  - `/` - o diretório root ou a separação de diretórios
  - `~` - home (cd sem nada vai para a home)
  - `-` menos - volta para o diretório que anterior 
- `ls` Lista o conteúdo de um diretório
    - `-a` - inclui entradas que o nome começa com ponto (arquivos ou diretórios ocultos)  
  - `-l` - lista em formato longo  
  - `-h` - com -l, é um sufixo de tamanho para facilitar a leitura   
  - `-@` - mostra atributos estendidos  
- `cp` - copia arquivos ou diretórios  
  - `-R` - copia o diretório em modo recursivo  
  <sub><sup>**Obs.:** Segundo o `man` (manual) do `cp`, se tiver uma barra (/) no final do diretório original, `cp` pode copiar apenas o conteúdo do diretório e não o diretório em si (eu não vi isso ocorrer em testes).</sup></sub>  
- `mv` - move arquivos ou diretórios (com mv você pode renomear arquivos ou diretórios)  
- `mkdir` - cria um diretório (use aspas ou barra invertida para separar caracteres inválidos)  
  - `-p` - cria uma estrutura inteira sem gerar erros  
  <sub><sup>Obs.: você pode usar chaves para criar múltiplos sub-diretórios.</sup></sub>  
- `rm` - apaga arquivos e diretórios  
  - `-R` - modo recursivo para diretórios  
  - `-f` - modo forçado e silencioso  
- `touch` - muda os tempos de acesso e modificação de um arquivo. Grande parte dos casos, usamos este comando para criar um arquivo vazio.

## Alguns símbolos e operadores úteis 👌
- `;` - permite executar vários comandos na mesma linha. Roda todos os comandos, mesmo se ocorrer algum erro.
- `&&` - permite executar vários comandos na mesma linha. Se o comando anterior não gerar nenhum erro, continua a corrente de comandos, do contrário, para no momento que ocorrer um erro.  
- `||` - permite executar vários comandos na mesma linha. Ele funciona de maneira oposta ao anterior, ou seja, se ocorrer algum erro no comando anterior, executa o próximo comando, do contrário, para no primeiro comando que **NÃO** gerar um erro.  
- `|` - Joga a saída (output) de um comando para a entrada (input) de outro.
- `>` - Joga a saída de um comando e redireciona para um arquivo. Apaga o arquivo todo e substitui seu conteúdo.
- `>>` - Joga a saída de um comando e redireciona para um arquivo. Não apaga o que estiver no arquivo, apenas adiciona o novo conteúdo na última linha.
- `&` - Joga para o background. Veja `jobs` e `fg` para complementar
## Background e Foreground ☢️
- `jobs` - mostra trabalhos em execução  
- `fg %n` - leva o que estiver em background para o foreground  
- `bg %n` - continua um job em background  
- `kill %n` - mata um job
## Outros comandos 👀
- `nano` - editor de textos  
- `file` - mostra o tipo do arquivo   
- `pkill` - mata processos
- `whoami` - mostra seu usuário
- `hostname` - mostra o nome do seu computador
- `uname` - mostra dados sobre o sistema
- `ps aux` - mostra todos os processos rodando no sistema no momento da execução