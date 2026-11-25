# Wazuh SOC Lab

## Objetivo 
Implementar um laboratório de monitoramento, detecção e investigação de eventos de segurança usando Wazuh, Sysmon e MITRE ATT&CK.

## Arquitetura
- VPS Ubuntu Server: Wazuh Server, Indexer e Dashboard
- Windows 11: Sysmon e Wazuh Agent
- MITRE ATT&CK: classificação das técnicas observadas

<img width="1266" height="706" alt="Arquitetura" src="https://github.com/user-attachments/assets/f61abf10-d1b4-43af-9b49-5238e6ac4b14" />

## Escopo
- Coleta e análise de eventos
- Monitoramento de atividades suspeitas
- Investigação de alertas
- Criação e validação de regras de detecção
- Documentação de casos de investigação

## Investigações
1. A definir
2. A definir
3. A definir


## Progresso do projeto

### Infraestrutura e preparação
- [x] Provisionamento da VPS Ubuntu Server
- [x] Hardening inicial do servidor
- [x] Configuração de firewall e acesso SSH
- [x] Documentação do hardening
- [x] Documentação da arquitetura planejada

### Implantação do Wazuh
- [x] Instalação All-in-One do Wazuh 4.14
- [x] Inicialização dos serviços principais
- [x] Acesso ao Wazuh Dashboard pelo Windows
- [x] Verificação inicial de recursos e serviços

### Monitoramento de endpoints
- [ ] Instalação do Wazuh Agent no Windows 11
- [ ] Integração do Sysmon
- [ ] Coleta e análise de eventos
- [ ] Investigações documentadas
- [ ] Criação e validação de regra de detecção
