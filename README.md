# 🛡️ Laboratório de Análise de Segurança em Linux com OSSEC

![Status do Projeto](https://img.shields.io/badge/Status-Em%20Andamento-green)
![OS](https://img.shields.io/badge/OS-Linux-blue)
![HIDS](https://img.shields.io/badge/HIDS-OSSEC-lightgrey)

Este repositório documenta uma série de laboratórios práticos de segurança ("Security Labs") realizados em um ambiente Linux monitorado pelo **OSSEC HIDS**. O objetivo é simular ameaças comuns, analisar os alertas gerados e documentar as descobertas, criando um portfólio de detecção e resposta a incidentes.

---

## 🎯 Objetivo do Projeto

O principal objetivo deste projeto é demonstrar de forma prática a capacidade de um Sistema de Detecção de Intrusão Baseado em Host (HIDS) como o OSSEC para identificar atividades maliciosas e anômalas em um sistema operacional Linux. Cada cenário representa uma técnica que poderia ser utilizada por um ator mal-intencionado.

---

## 🛠️ Ferramentas e Tecnologias

* **Sistema Operacional:** Linux (Ubuntu 22.04 LTS)
* **HIDS/SIEM:** OSSEC 4.0.0
* **Análise e Documentação:** Terminal Linux, Bash Script

---

## 🔬 Cenários de Ameaça Simulados

Abaixo está a lista dos laboratórios documentados neste repositório. Cada pasta contém um `README.md` com a análise detalhada da ameaça, a evidência coletada e o plano de resposta sugerido.

1.  **[Cenário 1: Tentativa de Força Bruta](./1_cenario_forca_bruta/)**
    * *Simulação e detecção de falhas consecutivas de autenticação ao tentar escalar privilégios com `sudo`.*

2.  **[Cenário 2: Alteração de Integridade de Arquivo](./2_cenario_alteracao_integridade/)**
    * *Detecção de modificações não autorizadas em arquivos críticos do sistema, como `/etc/passwd`, utilizando o módulo `syscheck`.*

3.  **[Cenário 3: Criação de Usuário Suspeito](./3_cenario_novo_usuario/)**
    * *Identificação de uma técnica de persistência comum, onde um novo usuário é adicionado ao sistema para garantir acesso futuro.*

4.  **[Cenário 4: Detecção de Rootkit](./4_cenario_deteccao_rootkit/)**
    * *Utilização do módulo `rootcheck` para escanear o sistema em busca de anomalias e malwares conhecidos que se escondem no sistema.*

*(Mais cenários serão adicionados...)*

---

## 🚀 Como Replicar este Laboratório

Para recriar este ambiente e executar os testes, você precisará de:

1.  Uma máquina virtual com uma distribuição Linux (preferencialmente baseada em Debian, como o Ubuntu).
2.  O OSSEC HIDS instalado a partir do código-fonte.
3.  Acesso de superusuário (`sudo`) para executar os comandos de simulação.
4.  Seguir os passos detalhados em cada um dos `README.md` dos cenários.

---

## 👨‍💻 Autor

* **[Seu Nome Completo]**
* [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/seu-perfil/)
* [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/seu-usuario)

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

