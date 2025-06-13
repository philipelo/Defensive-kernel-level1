# Defensive-kernel-level1
🛡️ DefensiveKernel-Tracker-v1  Ferramenta defensiva para rastreamento e auditoria de eventos no kernel Linux.   Desenvolvido como parte do meu estudo avançado de Segurança da Informação com foco em Kernel Hardening e monitoramento de execuções.  ---  ## 📌 Objetivo  Criar um sistema de rastreamento **defensivo e em tempo real** de execuções suspeitas no kernel, utilizando:  - `auditd` para auditoria em nível de sistema - `eBPF` (em breve) - Políticas de whitelisting de comandos sensíveis - Análise de execução por horário, UID e padrão de comportamento  ---  ## 🧠 Motivação  Esse projeto nasceu do estudo contínuo de segurança de kernel no Linux, com a intenção de desenvolver ferramentas **próprias, práticas e aplicáveis** para ambientes corporativos que precisam de defesa profunda (`Deep Defense`).  ---  ## 🧪 Tecnologias e Ferramentas  - Linux (Ubuntu/Debian) - `auditd` para auditoria - Shell Script para automação - `ausearch`, `auditctl` - Planejamento futuro para uso com `bpftrace` e `LSM`  ---  ## 🚀 Funcionalidades  - Rastreamento de execuções específicas - Auditoria de comandos sensíveis (ex: `insmod`, `rmmod`, `iptables`, `ip`, `systemctl`) - Log de eventos com hora, usuário, e comando completo - Base para integração com whitelists e políticas defensivas  ---  ## 📂 Estrutura  ` 
DefensiveKernel-Tracker-v1/ ├── logs/ │   └── execs.log ├── scripts/ │   └── monitor.sh ├── README.md
 ` ---  ## 📈 Próximos passos  - [ ] Integrar eBPF para rastreamento invisível - [ ] Desenvolver uma whitelist por horário e usuário - [ ] Adicionar bloqueio automático via LSM - [ ] Converter para módulo kernel customizado  ---  ## 📎 Exemplo de uso  ```bash sudo bash monitor.sh ` 
Veja os logs gerados em `logs/execs.log` com informações completas das execuções auditadas.
  
## 🤖 Autor
 
**Phillipe Lopes Amorim** Estudante de Segurança Kernel e Linux Hardening 
#linux #kernel #defensive #infosec #auditing #syscalls #auditd #eBPF
 
