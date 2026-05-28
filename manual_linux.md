🐧 Manual Linux - Comandos e Diretórios
⚡ Controle do Sistema
🖥️ Gerenciamento de Energia
Desligar o computador: shutdown -h now ⏻

Reiniciar: shutdown -r now ou <CTRL> + <ALT> + <DEL> 🔄

⌨️ COMANDOS BÁSICOS
📁 Navegação e Visualização
ls -a - Mostrar arquivos ocultos 🕵️

ls - Listar arquivos do diretório 📋

cd - Mudar de diretório 📂

cd ~ voltar para a pasta home

ls -l - Mostrar detalhes (dono, grupo, tamanho) 📊

📊 Tabela de Tamanhos de Arquivos
Símbolo	10^	2^	Nome
K	3	10	Quilo
M	6	20	Mega
G	9	30	Giga
T	12	40	Tera
P	15	50	Peta
E	18	60	Eta
Z	21	70	Zetta
Y	24	80	Yotta
📂 SISTEMA DE DIRETÓRIOS
🛠️ Comandos de Diretórios
mkdir - Criar diretórios 📁

cd / - Acessar diretório raiz 🏠

pwd - Ver diretório atual 📍

ls ~ - Ver diretório home 🏡

- - Voltar ao diretório anterior ↩️

🗂️ TIPOS DE DIRETÓRIOS
/bin 🗃️
Contém arquivos programas do sistema que são usados com freqüência pelos usuários.

/boot 🔰
Contém arquivos necessários para a inicialização do sistema.

/cdrom 💿
Ponto de montagem da unidade de CD-ROM.

/media 📀
Ponto de montagem de dispositivos diversos do sistema (rede, pen-drives, CD-ROM em distribuições mais novas).

/dev 🔧
Contém arquivos usados para acessar dispositivos (periféricos) existentes no computador.

/etc ⚙️
Arquivos de configuração de seu computador local.

/floppy 💾
Ponto de montagem de unidade de disquetes

/home 🏠
Diretórios contendo os arquivos dos usuários.

/lib 📚
Bibliotecas compartilhadas pelos programas do sistema e módulos do kernel.

/lost+found 🔍
Local para a gravação de arquivos/diretórios recuperados pelo utilitário fsck.ext2. Cada partição possui seu próprio diretório lost+found.

/mnt 📌
Ponto de montagem temporário.

/proc 🧠
Sistema de arquivos do kernel. Este diretório não existe em seu disco rígido, ele é colocado lá pelo kernel e usado por diversos programas que fazem sua leitura, verificam configurações do sistema ou modificar o funcionamento de dispositivos do sistema através da alteração em seus arquivos.

/sys 🔩
Sistema de arquivos do kernel. Este diretório não existe em seu disco rígido, ele é colocado lá pelo kernel e usado por diversos programas que fazem sua leitura, verificam configurações do sistema ou modificar o funcionamento de dispositivos do sistema através da alteração em seus arquivos.

/root 👑
Diretório do usuário root.

/sbin 🛠️
Diretório de programas usados pelo superusuário (root) para administração e controle do funcionamento do sistema.

/tmp 🗑️
Diretório para armazenamento de arquivos temporários criados por programas.

/usr 📦
Contém maior parte de seus programas. Normalmente acessível somente como leitura.

/var 📨
Contém maior parte dos arquivos que são gravados com freqüência pelos programas do sistema, e-mails, spool de impressora, cache, etc.

⚡ EXECUÇÃO DE PROGRAMAS
📍 Nomear diretórios (duas opções):
1 - Mudar o diretório padrão para /etc com o comando cd /etc e usar o comando cat hosts

2 - Usar o comando "cat" especificando o caminho completo na estrutura de diretórios e o nome de arquivo: cat /etc/hosts.

🔄 Comandos Internos
Exemplos de comandos internos são: cd, exit, echo, bg, fg, source, help

🔄 Executar dois programas juntos:
Para iniciar um programa em primeiro plano, basta digitar seu nome normalmente. Para iniciar um programa em segundo plano, acrescente o caracter "&" após o final do comando.

O programa executado em background continua sendo executado internamente. Após ser concluído, o sistema retorna uma mensagem de pronto acompanhado do número PID do processo que terminou.

OBS: Mesmo que um usuário execute um programa em segundo plano e saia do sistema, o programa continuará sendo executado até que seja concluído ou finalizado pelo usuário que iniciou a execução (ou pelo usuário root).

Exemplo: find / -name boot.b &

O comando será executado em segundo plano e deixará o sistema livre para outras tarefas. Após o comando find terminar, será mostrada uma mensagem.

🔗 Executando programas em seqüência:
Os comandos podem ser executados em seqüência (um após o término do outro) se os separarmos com ";".

Por exemplo: echo primeiro;echo segundo;echo terceiro
