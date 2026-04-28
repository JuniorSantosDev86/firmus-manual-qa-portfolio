# Portfólio de QA Manual — Firmus

Este repositório documenta um processo profissional de QA Manual aplicado ao **Firmus**, um copilot operacional para prestadores de serviços e pequenos negócios.

O objetivo é demonstrar planejamento, estratégia, cobertura funcional, BDD/Gherkin, casos de teste manuais, execução real, bug reports, evidências e relatórios de QA em PT-BR.

## Sistema sob teste

O Firmus apoia a operação diária com dashboard, perfil da empresa, clientes, plano, prontidão do MVP, serviços, orçamentos, cobranças, DAS, NFSe, lembretes, logs de atividade, radar de reativação, modelos, entrada assistida, sugestões, regras de automação, resumo semanal e visão financeira.

Este repositório **não contém o código-fonte do produto**. Ele contém documentação de QA Manual para portfólio profissional.

## Papel do QA

Documentação, desenho de cenários, execução manual e reporte realizados por **Ademir dos Santos Junior**, com foco em clareza, rastreabilidade e comunicação objetiva para times de produto, desenvolvimento e QA.

## Estrutura

```txt
bdd/funcionalidades/        Cenários BDD/Gherkin planejados em PT-BR
bug-reports/                Bugs reais preservados e template profissional
checklists/                 Checklists de smoke, regressão, responsivo, exploratório, BDD, bug e evidências
docs/                       Plano, estratégia, escopo e guia de severidade/prioridade
evidences/                  Evidências reais preservadas em screenshots e vídeos
reports/                    Relatórios, matrizes de cobertura e risco
test-cases/                 Casos de teste manuais planejados por módulo
test-executions/            Execuções reais e resumos de ciclo
```

## Destaques

- Conteúdo padronizado em PT-BR.
- BDD/Gherkin em português com cenários planejados para todos os módulos visíveis.
- Separação explícita entre casos planejados, execução real, bugs e evidências.
- Bugs reais `BUG-001` a `BUG-006` preservados com evidências existentes.
- Matrizes de cobertura e risco para leitura executiva.
- Relatório final adequado para GitHub, LinkedIn e avaliação técnica.

## Como navegar

1. Leia o [Plano de Testes](./docs/test-plan.md).
2. Consulte o [Escopo de Testes](./docs/test-scope.md) e a [Estratégia de Testes](./docs/test-strategy.md).
3. Revise os [cenários BDD](./bdd/funcionalidades/dashboard.feature) e os [casos de teste](./test-cases/dashboard.md).
4. Verifique a [execução real do ciclo 01](./test-executions/execution-cycle-01.md).
5. Consulte os [bugs reportados](./bug-reports/) e as [evidências](./evidences/README.md).
6. Leia o [relatório final](./reports/relatorio-final-qa-manual.md).

## Observação sobre execução

Os novos cenários BDD e casos de teste adicionados nesta organização estão como **Planejado** e **Não Executado**. Somente o ciclo 01 registra execução real, com resultados preservados para Autenticação, Dashboard, Clientes, Orçamentos, Visão Financeira e NFSe.

## Próximos passos

- Executar ciclos manuais adicionais para os módulos ainda planejados.
- Reexecutar os bugs após correção.
- Atualizar evidências apenas quando houver nova execução real.
- Expandir testes de acessibilidade e API em ciclos específicos, se entrarem no escopo.
