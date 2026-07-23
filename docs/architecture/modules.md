# Hubyn Modules

## Missão

Os Hubyn Modules representam os produtos de negócio da plataforma.

Cada módulo possui uma responsabilidade específica, podendo operar de forma independente ou integrado aos demais componentes do ecossistema Hubyn.

---

## Responsabilidades

Cada módulo é responsável por:

- Implementar suas próprias regras de negócio;
- Gerenciar seus próprios dados;
- Expor funcionalidades específicas do produto;
- Consumir serviços disponibilizados pelo Core, Connect, Capabilities e AI quando necessário.

---

## O que os Modules NÃO fazem

Os módulos não:

- Compartilham banco de dados entre si;
- Implementam serviços que pertencem ao Core;
- Duplicam capacidades compartilhadas;
- Dependem diretamente de outros módulos para funcionar.

Toda comunicação entre módulos deve ocorrer por interfaces padronizadas.

---

## Módulos previstos

A arquitetura inicial contempla os seguintes produtos:

- ChatBot Lite
- ChatBot Pro
- CRM
- Financeiro
- Faculdade
- Imobiliária

Novos módulos poderão ser adicionados sem necessidade de alterações na arquitetura da plataforma.

---

## Relação com os demais componentes

```text
                 HUBYN CORE
                      │
     ┌────────────────┼────────────────┐
     ▼                ▼                ▼
 Connect       Capabilities           AI
     │                │                │
     └────────────────┼────────────────┘
                      │
                      ▼
                 Hubyn Modules
```

Os módulos utilizam os serviços disponibilizados pela plataforma, mantendo baixo acoplamento e independência entre si.

---

## Princípios

- Independência entre módulos.
- Responsabilidade única.
- Baixo acoplamento.
- Alta coesão.
- Evolução independente.
- Produtos comercializáveis individualmente.

---

## Observações

Este documento define a responsabilidade dos módulos de negócio da Hubyn.

Cada produto possuirá sua própria documentação funcional e técnica, mantendo esta especificação focada exclusivamente na arquitetura da plataforma.
