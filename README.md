# Portfólio de QA · Testes Manuais em demoblaze.com

-**Autor:** Luiz Vinicius Cunha Maciel
-**Projeto:** Portfólio pessoal de QA
-**Aplicação sob teste:** [demoblaze.com](https://www.demoblaze.com) — e-commerce fictício de eletrônicos
-**Ciclo de referência:** Ciclo 1 · 27–28/07/2026

---

## Sobre este projeto

Este repositório reúne o ciclo completo de um processo de testes manuais aplicado ao Demoblaze, um e-commerce de demonstração usado como ambiente de prática para QA. O objetivo foi simular todas as etapas de um ciclo de testes: planejamento, design de casos, execução, registro de defeitos e encerramento com recomendação de release.

Foram planejadas e executadas **21 casos de teste** cobrindo **9 funcionalidades** do sistema (navegação, cadastro, login, carrinho, checkout, contato e responsividade), resultando na abertura de **4 defeitos**, sendo **2 de severidade Alta**.

---

## Como navegar pelos documentos

Os documentos foram escritos na ordem em que normalmente são produzidos em um ciclo de testes real:

| # | Documento | O que contém |
|---|-----------|---------------|
| 1 | **Plano_de_Testes.pdf** | Escopo, tipos de teste, estratégia, técnicas de design de caso, critérios de entrada/saída, ferramentas e papéis. Ponto de partida do ciclo. |
| 2 | **Casos_de_Teste.docx** | 21 casos de teste detalhados (CT-01 a CT-21), com pré-condições, dados de teste, passos, resultado esperado, prioridade e tipo de teste. |
| 3 | **Matriz_Execucao.xlsx** | Planilha de execução do Ciclo 1: status de cada caso (Passou/Falhou), data, executor, evidências e observações. |
| 4 | **Relatorio_de_Bugs.docx** | Os 4 defeitos encontrados na execução, com severidade, prioridade, passos para reproduzir, resultado esperado x obtido e evidências. |
| 5 | **Test_Summary_Report.docx** | Report do Ciclo 1: métricas, verificação dos critérios de saída, riscos residuais e recomendação final de release. |

---

## Resultados do Ciclo 1

| Métrica | Valor |
|---|---|
| Casos planejados / executados | 21 / 21 (100%) |
| Casos aprovados | 17 (81%) |
| Casos reprovados | 4 (19%) |
| Casos de prioridade Alta executados | 10/10 (100%) |
| Defeitos abertos | 4 (2 Alta · 1 Média · 1 Baixa) |
| Cobertura de funcionalidades em escopo | 9/9 (100%) |

**Recomendação final do ciclo:** não publicar novas alterações até a correção dos defeitos de severidade Alta (BUG-02 — checkout aceita cartão inválido; BUG-04 — checkout sem login), por comprometerem a integridade do fluxo de compra. BUG-01 e BUG-03 podem ser tratados no próximo ciclo sem bloquear entrega.

---

## Técnicas e abordagem aplicadas

- Testes funcionais, exploratórios, de campo/negativo e smoke test
- Particionamento de equivalência e análise de valor limite (ex.: cálculo de total do carrinho)
- Rastreabilidade requisito → caso de teste → execução → defeito
- Encerramento de ciclo com verificação formal dos critérios de saída e recomendação de release baseada em risco

---

## Ferramentas utilizadas

Word e Excel para gestão de casos de teste e defeitos · Chrome/Edge como navegadores alvo · 
---

## Próximos passos

- Avaliação de automação dos fluxos críticos (login, carrinho, checkout) como evolução do portfólio
