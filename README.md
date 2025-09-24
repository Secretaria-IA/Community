# Projeto Aura DBL: Plataforma Inteligente de Gestão e Vendas


Este é um ecossistema completo de software projetado para automação de processos de vendas, atendimento e gestão de negócios. A plataforma integra um CRM, um ERP e uma assistente com Inteligência Artificial (Aura) para oferecer uma solução 360° para empresas de serviço.

## Core Components

A plataforma é composta por vários sistemas que trabalham de forma integrada:

* **CRM Inteligente:** Uma aplicação web (Next.js) para a gestão inteligente de leads, com funis de venda visuais (Kanban), importação de dados, dashboards gerenciais e funcionalidades de IA para qualificação e priorização de leads.
* **ERP (Agenda Integrada):** Um sistema de gestão robusto para o controle de agendamentos, gestão financeira (contas a pagar/receber, fluxo de caixa), compras e estoque.
* **Aura - Agente IA:**
    * **Atendimento Receptivo:** Um workflow principal no n8n que atua como a "Secretária IA", atendendo leads que entram em contato via WhatsApp e outros canais, 24/7.
    * **Prospecção Ativa:** Um script Python (`executar_planos.py`) que funciona como um "Executor de Planos", buscando estratégias de abordagem no CRM e iniciando o contato com novos leads de forma automatizada e segura.
* **Base de Conhecimento (RAG):** Um banco de dados vetorial no Supabase que permite à Aura responder perguntas complexas com base em uma base de conhecimento customizada, utilizando a técnica de RAG (Retrieval-Augmented Generation).

## Arquitetura e Tecnologias

* **Frontend/Backend Principal:** Next.js, React, TypeScript
* **Banco de Dados Principal:** Firestore (Firebase)
* **Inteligência Artificial:** Google Genkit
* **Automação e Workflows:** n8n.io
* **Scripts de Prospecção:** Python
* **Banco de Dados Vetorial (RAG):** Supabase com a extensão `pgvector`
* **Plataforma de Atendimento:** Chatwoot

