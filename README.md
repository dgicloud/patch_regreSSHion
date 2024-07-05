#Correção e Atualização do OpenSSH para CVE-2024-6387
Este repositório contém um script Bash para corrigir e atualizar o pacote OpenSSH, endereçando a vulnerabilidade CVE-2024-6387. A vulnerabilidade permite a execução remota de código não autenticado, representando um risco significativo para a segurança.

#Descrição do Script
O script realiza as seguintes ações:

Backup do arquivo de configuração: Cria um backup do arquivo de configuração sshd_config para garantir que as configurações originais possam ser restauradas.
Verificação da versão do SSH: Checa e exibe a versão atual do SSH instalada no sistema.
Atualização do Sistema: Atualiza a lista de pacotes do sistema.
Instalação de Pacotes Necessários: Instala todos os pacotes necessários para compilar e instalar o OpenSSH.
Download do OpenSSH: Baixa a versão corrigida do OpenSSH.
Descompactação e Configuração: Descompacta o arquivo baixado e configura o ambiente para compilação.
Compilação e Instalação: Compila e instala o OpenSSH.
Backup e Substituição do binário do SSHD: Cria um backup do binário antigo do sshd e cria um link simbólico para o novo binário.
Restauração do arquivo de configuração: Restaura o arquivo de configuração original.
Reinício do Serviço SSH: Reinicia o serviço SSH para aplicar as mudanças.
Verificação Final da Versão do SSH: Checa e exibe a versão atualizada do SSH para confirmar a aplicação do patch.
Instruções de Uso
Clone este repositório:

bash
Copiar código
git clone https://github.com/seu-usuario/repo-correção-openssh.git
cd repo-correção-openssh
Dê permissão de execução ao script:

bash
Copiar código
chmod +x atualizar_openssh.sh
Execute o script como root:

bash
Copiar código
sudo ./atualizar_openssh.sh
Requisitos
Sistema operacional baseado em Debian (por exemplo, Ubuntu)
Acesso root ou privilégios sudo
Aviso
Este script realiza operações críticas no sistema. Certifique-se de testá-lo em um ambiente de desenvolvimento antes de aplicá-lo em produção. Mantenha backups atualizados de todos os arquivos e configurações importantes.

Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

Licença
Este projeto está licenciado sob a Licença MIT.
