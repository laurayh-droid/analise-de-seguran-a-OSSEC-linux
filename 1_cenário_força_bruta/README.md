# Cenário 1: Tentativa de Acesso por Força Bruta

## Descrição da Ameaça
Este cenário simula um atacante tentando adivinhar a senha de um usuário com privilégios (`sudo`) no sistema. Múltiplas tentativas de login falhas são um forte indicador de um ataque de força bruta em andamento. Em primeiro momento foi registredo uma regra genérica, o 1002 (nível 2), não representa uma ameaça, seria apenas um ruído. Logo fiz a primeira tentativa de entrar como root no sistema, um log de falha de autenticação (nível 5) foi gerado, capturado pela regra 5503, um indicativo para um ataque de força bruta. Depois de múltiplas tentativas com a senha inválida, o log gerou um alerta de nível 10, um alerta críticono OSSEC, indicando que algo sério está acontecendo, a regra acionada é a 5504, mostrando que ouve uma sequência de eventos, e nesse caso, o OSSEC detectou que o usuário fez 3 tentativas de senha incorreta em um curto período de tempo

---

## Relatório de Descoberta (Security Finding)

* **ID da Descoberta:** BRUTEFORCE-001
* **Data/Hora do Evento:** 29 de Agosto de 2025, 14:27 (Horário de Brasília)
* **Nível de Risco (OSSEC):** **Alto (Nível 10)**
* **Técnica MITRE ATT&CK:** [T1110 - Brute Force](https://attack.mitre.org/techniques/T1110/)
