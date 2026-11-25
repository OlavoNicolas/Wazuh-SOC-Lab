# Hardening da VPS

## 1. Objetivo

Realizar a configuração inicial de segurança do servidor Linux que hospedará a infraestrutura central do laboratório SOC com Wazuh.

O objetivo é reduzir a superfície de ataque, restringir acessos administrativos e estabelecer uma configuração inicial segura antes da implantação dos componentes do SIEM.

## 2. Controle de acesso

- Criação de usuário administrativo dedicado: `labSocOlavo`.
- Utilização de `sudo` para operações privilegiadas.
- Autenticação SSH por chave Ed25519.
- Desabilitação do login SSH direto do root.
- Desabilitação da autenticação SSH por senha após validação do acesso por chave.
- Proteção da chave privada.

## 3. Controle de rede

- Configuração do UFW com política de bloqueio de conexões de entrada.
- Liberação das portas necessárias ao gerenciamento da VPS.
- Configuração complementar do firewall disponibilizado pela Hostinger.
- Restrição das portas destinadas aos serviços administrativos e de monitoramento.

## 4. Proteção do sistema operacional

- Instalação e configuração do Fail2ban para proteção contra tentativas repetidas de autenticação.
- Instalação do `unattended-upgrades` para automatização de atualizações de segurança.
- Instalação de ferramentas administrativas: OpenSSH, curl, wget, nano e htop.
- Utilização de atualizações periódicas do sistema operacional.

## 5. Backup e recuperação

- Configuração de backups semanais disponibilizados pela Hostinger.
- Criação de snapshot após a conclusão das configurações iniciais de hardening.

## 6. Segurança da conta do provedor

- Ativação da autenticação de dois fatores (2FA) na conta Hostinger.
- Utilização de senha forte e exclusiva.
- Armazenamento seguro dos códigos de recuperação.

## 7. Validação

Foram realizadas verificações dos seguintes componentes:

- Estado e regras do UFW.
- Parâmetros efetivos de configuração do SSH.
- Estado do serviço Fail2ban e da proteção SSH.
- Estado do mecanismo de atualizações automáticas.
- Disponibilidade de memória, armazenamento e processamento.

## 8. Próxima etapa

Após a preparação e validação da infraestrutura, será realizada a implantação do Wazuh All-in-One, incluindo Wazuh Server, Indexer e Dashboard.

**Observação:** este documento registra a configuração inicial de segurança da infraestrutura. As configurações poderão ser revisadas e aprimoradas durante a evolução do laboratório.
