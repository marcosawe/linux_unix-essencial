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

## Dicas modo de texto 📑

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

### Comandos para reiniciar o sistema 