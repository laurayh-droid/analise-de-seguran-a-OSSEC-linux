# Cenário 3: Criação de Usuário Suspeito

## Descrição da Ameaça
Este cenário simula uma das técnicas de persistência mais comuns, onde um invasor, após obter acesso inicial, cria uma nova conta de usuário. Esta conta "backdoor" garante que o atacante possa retornar ao sistema comprometido no futuro, mesmo que a vulnerabilidade original seja corrigida. O OSSEC também detectou a mudança do arquivo que gerencia os grupos de usuário no sistema(nível 7).

---

## Relatório de Descoberta (Security Finding)

* **ID da Descoberta:** PERSISTENCE-001
* **Data/Hora do Evento:** 29 de Agosto de 2025, 14:37 (Horário de Brasília)
* **Nível de Risco (OSSEC):** **Alto (Nível 8)**
* **Técnica MITRE ATT&CK:** [T1136.001 - Create Account: Local Account](https://attack.mitre.org/techniques/T1136/001/)
