# Software Design Document (SDD) - Sistema Simples

## 1. Visão Geral
API REST simples desenvolvida em Python (Flask), containerizada com Docker e implantada na AWS EC2 através de uma pipeline de CI/CD automatizada com análise estática de segurança.

## 2. Componentes da Arquitetura
- **Aplicação:** Python 3.10 com Flask na porta 5000 (redirecionada para a porta 80).
- **Scanner SAST:** SonarCloud / SonarQube para análise de segurança no código.
- **Infraestrutura Cloud:** Instância AWS EC2 (Ubuntu 26.04 LTS) executando Docker.
- **Pipeline CI/CD:** GitHub Actions com deploy automático via SSH.
