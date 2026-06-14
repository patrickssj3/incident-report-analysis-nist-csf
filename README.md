# Análise de Relatório de Incidente — Ataque DoS (ICMP Flood)

## Sobre este projeto

Este documento faz parte de uma atividade prática de segurança cibernética, na qual um incidente de rede é analisado utilizando a **Estrutura de Segurança Cibernética (CSF) do NIST** (National Institute of Standards and Technology). O objetivo é demonstrar uma abordagem proativa à segurança, aplicando as cinco funções principais do CSF — **Identificar, Proteger, Detectar, Responder e Recuperar** — para avaliar um incidente real e propor melhorias na segurança da rede.

Este relatório pode ser usado como peça de portfólio de segurança cibernética.

## Cenário do incidente

Uma empresa de multimídia (serviços de Web design, design gráfico e marketing em mídias sociais) sofreu um **ataque de negação de serviço (DoS)** que comprometeu a rede interna por aproximadamente **duas horas**.

- **Causa:** um firewall mal configurado permitiu a entrada de um grande volume de pacotes ICMP (ping flood).
- **Impacto:** os serviços de rede pararam de responder; usuários internos não conseguiram acessar nenhum recurso.
- **Resposta inicial:** bloqueio da entrada de pacotes ICMP, suspensão de serviços não críticos e restauração dos serviços críticos.
- **Medidas implementadas após o incidente:**
  - Regra de firewall para limitar a taxa de pacotes ICMP de entrada
  - Verificação do IP de origem (anti-spoofing)
  - Software de monitoramento de rede
  - Sistema IDS/IPS para filtrar tráfego ICMP suspeito

## Estrutura do relatório (NIST CSF)

O relatório está organizado nas seguintes seções:

1. **Resumo** — visão geral do evento, causa, impacto e resposta.
2. **Identificar** — tipo de ataque, sistemas afetados, origem e impacto estimado.
3. **Proteger** — políticas, procedimentos e ferramentas para mitigar ameaças futuras.
4. **Detectar** — monitoramento contínuo de tráfego, sistemas e contas de usuário.
5. **Responder** — plano de contenção, neutralização, análise e melhoria de processos.
6. **Recuperar** — restauração de sistemas, dados e processos afetados.

## Como usar este material

- Preencha cada seção com base no incidente analisado, seguindo as perguntas-guia da atividade.
- Use este relatório como modelo para futuras análises de incidentes, adaptando o conteúdo a outros cenários.
- Inclua este documento em seu portfólio de segurança cibernética como exemplo de aplicação prática do NIST CSF.
