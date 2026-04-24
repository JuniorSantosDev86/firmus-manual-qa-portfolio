# Firmus Manual QA Portfolio

Projeto de portfólio em QA Manual que documenta planejamento de testes, escopo de testes, casos de teste, relatórios de bugs, execuções de teste e evidências de QA para a aplicação Firmus.

> English version: [README.md](./README.md)

---

## Visão Geral do Projeto

Este repositório apresenta um processo completo de **Quality Assurance Manual** aplicado ao **Firmus**, uma aplicação web criada para apoiar prestadores de serviço e pequenos negócios em suas rotinas operacionais.

O principal objetivo deste portfólio é demonstrar habilidades práticas de QA por meio de documentação estruturada, planejamento de testes, definição de escopo, criação de casos de teste manuais, reporte de bugs, coleta de evidências e relatórios de execução.

Este projeto faz parte de um portfólio profissional de QA com foco em práticas reais de teste de software.

---

## Sistema Sob Teste

**Firmus** é uma aplicação web B2B voltada para ajudar prestadores de serviço a gerenciar fluxos importantes do negócio, como:

- Gestão de clientes
- Orçamentos de serviço
- Visibilidade financeira
- Dashboard operacional
- Fluxos relacionados à NFSe
- Ações operacionais assistidas

A aplicação utilizada como sistema sob teste está mantida em um repositório separado.

**Repositório da Aplicação:**  
[https://github.com/JuniorSantosDev86/firmus-app](https://github.com/JuniorSantosDev86/firmus-app)

---

## Objetivo do Portfólio de QA

O objetivo deste repositório é demonstrar a capacidade de **planejar, projetar, executar e documentar** um processo de QA manual de forma profissional.

Isso inclui:

- Entender o contexto da aplicação
- Definir o escopo de testes
- Criar uma estratégia de testes
- Escrever casos de teste manuais
- Executar ciclos de teste funcionais
- Reportar bugs com clareza
- Coletar evidências de teste
- Produzir documentação de QA
- Comunicar resultados de forma objetiva

---

## Atividades de QA Cobertas

Este portfólio inclui as seguintes atividades de QA:

| Área | Descrição |
|---|---|
| Planejamento de Testes | Definição de objetivos, riscos, recursos, critérios e entregáveis |
| Escopo de Testes | Definição de módulos, fluxos e áreas cobertas pelos testes manuais |
| Estratégia de Testes | Abordagem de testes manuais e tipos de teste utilizados |
| Criação de Casos de Teste | Casos estruturados com passos, resultados esperados e status |
| Testes Funcionais | Validação dos fluxos principais da aplicação |
| Smoke Testing | Validação rápida das funcionalidades críticas |
| Regression Testing | Revalidação de fluxos existentes após mudanças |
| Exploratory Testing | Investigação de possíveis problemas além dos roteiros fixos |
| Responsive Testing | Validação básica em diferentes tamanhos de tela |
| Bug Reporting | Documentação clara de defeitos com severidade e prioridade |
| Coleta de Evidências | Screenshots e vídeos que apoiam os resultados dos testes |
| Relatório de Execução | Resumo dos testes executados e seus resultados |

---

## Módulos Testados

O escopo de QA manual cobre as principais áreas da aplicação Firmus:

- Autenticação
- Rotas protegidas
- Dashboard / Torre de Controle
- Clientes
- Orçamentos
- Visão financeira
- Base de NFSe
- Comportamento responsivo
- Usabilidade básica

---

## Estrutura do Repositório

```txt
firmus-manual-qa-portfolio/
├── README.md
├── README.pt-BR.md
├── bug-reports/
│   ├── bug-report-template.md
│   └── sample-bugs.md
├── checklists/
│   ├── exploratory-test-checklist.md
│   ├── regression-test-checklist.md
│   ├── responsive-test-checklist.md
│   └── smoke-test-checklist.md
├── docs/
│   ├── final-test-report.md
│   ├── severity-priority-guide.md
│   ├── test-plan.md
│   ├── test-scope.md
│   └── test-strategy.md
├── evidences/
│   ├── screenshots/
│   └── videos/
├── test-cases/
│   ├── authentication-test-cases.md
│   ├── clients-test-cases.md
│   ├── dashboard-test-cases.md
│   ├── financial-test-cases.md
│   ├── nfse-test-cases.md
│   └── quotes-test-cases.md
└── test-executions/
    ├── execution-cycle-01.md
    └── execution-summary.md
```

---

## Artefatos de QA

Este repositório contém os seguintes artefatos de QA:

### Documentação

- Test Plan
- Test Scope
- Test Strategy
- Severity and Priority Guide
- Final Test Report

### Design de Testes

- Casos de teste de autenticação
- Casos de teste de dashboard
- Casos de teste de clientes
- Casos de teste de orçamentos
- Casos de teste financeiros
- Casos de teste de NFSe

### Execução de Testes

- Ciclo manual de execução
- Resumo de execução
- Checklist de smoke test
- Checklist de regression test
- Checklist de responsive test
- Checklist de exploratory test

### Reporte de Bugs

- Template de bug report
- Exemplos de bug reports
- Documentação baseada em evidências

---

## Formato dos Casos de Teste

Cada caso de teste segue uma estrutura organizada:

```txt
ID do Caso de Teste
Título
Módulo
Tipo
Prioridade
Severidade em caso de falha
Pré-condições
Passos para reproduzir
Resultado esperado
Resultado atual
Status
Evidência
Observações
```

Exemplo:

```txt
TC-AUTH-001 — Login com credenciais válidas

Módulo: Authentication
Tipo: Functional
Prioridade: High
Severidade em caso de falha: Critical

Pré-condições:
- O usuário possui credenciais válidas
- A aplicação está em execução
- O usuário está na página de login

Passos:
1. Abrir a aplicação Firmus
2. Inserir um e-mail válido
3. Inserir uma senha válida
4. Clicar no botão de login

Resultado Esperado:
O usuário deve ser autenticado e redirecionado para o dashboard.

Status:
Not executed
```

---

## Formato do Bug Report

Os bug reports seguem uma estrutura profissional:

```txt
Bug ID
Título
Ambiente
Severidade
Prioridade
Pré-condições
Passos para reproduzir
Resultado atual
Resultado esperado
Evidência
Observações adicionais
```

Esse formato ajuda a garantir que cada bug report seja claro, reproduzível e útil para desenvolvedores.

---

## Severidade e Prioridade

Este projeto separa **severidade** de **prioridade**.

**Severidade** descreve o impacto do problema no sistema.

**Prioridade** descreve a urgência com que o problema deve ser corrigido.

### Severidade

| Severidade | Significado |
|---|---|
| Critical | Bloqueia um fluxo crítico ou impede o uso do sistema |
| High | Afeta uma funcionalidade importante sem workaround simples |
| Medium | Afeta uma funcionalidade, mas existe workaround |
| Low | Problema visual, textual ou pequeno problema de usabilidade |

### Prioridade

| Prioridade | Significado |
|---|---|
| High | Deve ser corrigido o quanto antes |
| Medium | Deve ser corrigido em um ciclo planejado |
| Low | Pode ser corrigido depois |

---

## Ferramentas Utilizadas

Os seguintes recursos são utilizados neste processo de QA manual:

- GitHub
- Markdown
- Browser DevTools
- Screenshots
- Evidências em vídeo
- Testes exploratórios manuais
- Ambiente local da aplicação
- Boas práticas de documentação em QA

---

## Status Atual

| Área | Status |
|---|---|
| Estrutura do repositório | Concluído |
| Documentação do README | Concluído |
| Test plan | Concluído |
| Test scope | Concluído |
| Test strategy | Concluído |
| Casos de teste | Concluído |
| Ciclo de execução | Em andamento |
| Bug reports | Pendente |
| Relatório final de QA | Pendente |

---

## Habilidades Profissionais Demonstradas

Este projeto demonstra as seguintes habilidades de QA:

- Testes manuais
- Planejamento de testes
- Definição de escopo de testes
- Criação de casos de teste
- Reporte de bugs
- Testes funcionais
- Regression testing
- Smoke testing
- Exploratory testing
- Responsive testing
- Coleta de evidências
- Documentação técnica
- Pensamento orientado à qualidade
- Comunicação de resultados

---

## Sobre o Tester

**Ademir dos Santos Junior**  
QA Analyst | Full Stack Developer

Estou construindo um portfólio profissional em QA com foco em atividades práticas de teste, documentação realista e validação manual de aplicações web.

Este repositório faz parte do meu processo de desenvolvimento profissional em Quality Assurance, combinando fundamentos de testes manuais com experiência em desenvolvimento de software.

---

## Projetos Relacionados

- [Firmus Application](https://github.com/JuniorSantosDev86/firmus-app)
- [Cypress Mini Shop QA](https://github.com/JuniorSantosDev86/cypress-mini-shop-qa)
- [Manual QA Tests — SauceDemo Login](https://github.com/JuniorSantosDev86/qa-manual-tests-saucedemo-login)

---

## Propósito do Repositório

Este repositório foi criado para mostrar um fluxo completo e organizado de QA manual aplicado a uma aplicação real.

Ele foi pensado para ser utilizado como projeto de portfólio profissional em oportunidades de QA, software testing e quality assurance.
