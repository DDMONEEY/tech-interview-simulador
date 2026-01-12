# 👔 IA Entrevistador: Simulador de Entrevista Técnica (Backend)

> **Status:** ✅ Aprovado (Nível Pleno/Sênior)

Este projeto consiste em um simulador de entrevistas técnicas de alto nível desenvolvido com o **Google AI Studio (Gemini)**. O objetivo foi treinar para vagas de **Engenharia de Software** em grandes empresas de tecnologia (Big Techs).

## 🤖 O Prompt (System Instruction)

Configurei a IA para atuar como um **Tech Recruiter Sênior** exigente, focado em arquitetura de software, escalabilidade e cultura de engenharia.

**Regras da Simulação:**
*   Perguntas sequenciais (uma por vez).
*   Foco em resolução de problemas complexos (System Design).
*   Avaliação de Hard Skills e Soft Skills.

---

## 💬 Destaques da Simulação

Durante a entrevista, fui desafiado em cenários reais de alta performance. Abaixo, os principais tópicos abordados e minhas soluções:

### 1. Integridade de Dados e Concorrência
**Desafio:** Como evitar duplicidade de registros (race conditions) em um sistema de Sinistros com alto tráfego?
**Minha Solução:** Implementação de **Optimistic Locking** (JPA @Version) combinado com **Idempotency Keys** na API e isolamento de transações ACID.

### 2. Gestão de Conflitos (Soft Skill)
**Desafio:** Divergência técnica sobre arquitetura (Microserviços vs Monolito).
**Minha Solução:** Aplicação do princípio **YAGNI** (You Aren't Gonna Need It), defendendo uma arquitetura simples e evolutiva baseada em dados e trade-offs, evitando *over-engineering*.

### 3. System Design (O Desafio Final)
**Desafio:** Criar um Ranking Global em Tempo Real para 50 milhões de usuários com latência < 50ms.
**Minha Solução:** Arquitetura baseada em **Redis Sorted Sets (ZSET)** para ordenação em memória (complexidade O(log N)) com padrão *Write-Behind* para persistência assíncrona em banco relacional.

---

## 🏆 Feedback Final da IA

Ao final da sabatina, o Recruiter Virtual gerou o seguinte relatório:

> **VEREDITO: APROVADO**
>
> *"O candidato possui o equilíbrio necessário entre profundidade técnica em Backend e visão sistêmica de produto. Demonstrou resiliência sob pressão (...) além de dominar tecnologias modernas para problemas de escala global."*

**Pontos Fortes Citados:**
*   ✅ Domínio Arquitetural (ACID, Optimistic Locking).
*   ✅ Pragmatismo e Senioridade.
*   ✅ Resolução de Problemas de Escala (Redis ZSet).

---

## 🛠️ Tecnologias Abordadas
- **Java / Spring Boot**
- **Redis (Cache & Estruturas de Dados)**
- **SQL (Transações & Locks)**
- **Engenharia de Prompts**
