# Cenário 2: Modificação de Arquivo de Sistema Crítico

## Descrição da Ameaça
Este cenário simula um atacante ou malware que obteve acesso privilegiado e está modificando arquivos de configuração críticos para manter persistência, redirecionar tráfego ou desabilitar defesas. O monitoramento de integridade de arquivos (FIM - File Integrity Monitoring) é uma defesa essencial contra esse tipo de atividade. Simulei esse mesmo ataque duas veses para que o log conseguisse analisar,tive que forçar a verificação para saber se o syscheck estava rodando.

---

## Relatório de Descoberta (Security Finding)

* **ID da Descoberta:** FIM-001
* **Data/Hora do Evento:** 29 de Agosto de 2025, 16:09 (Horário de Brasília)
* **Nível de Risco (OSSEC):** **Alto (Nível 7)**
* **Técnica MITRE ATT&CK:** [T1574.006 - Hijack Execution Flow: Dynamic Linker Hijacking](https://attack.mitre.org/techniques/T1574/006) (um exemplo relacionado a modificação de arquivos de sistema).


