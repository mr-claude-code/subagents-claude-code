# Sub-Agents para Claude Code

Uma colecao de sub-agentes especializados para uso com Claude Code, com mais de **200 agentes** cobrindo engenharia de software, marketing, financas, design, jogos, vendas e muito mais.

## Instalacao

Para usar estes agentes no seu projeto, copie a pasta `agents` para `.claude/agents/` no seu projeto:

```bash
mkdir -p .claude/agents
cp agents/*.md .claude/agents/
```

Ou copie apenas os agentes que deseja usar.

## Agentes Originais (Detalhados)

Os agentes abaixo possuem documentacao detalhada de uso:

### 1. Documentation Sync Agent (`documentation-sync-agent.md`)

**Cor:** Verde | **Modelo:** Opus

Agente especializado em manter a documentacao do projeto sempre atualizada e sincronizada. Responsavel por:

- Rastrear progresso de desenvolvimento
- Documentar bugs encontrados
- Registrar decisoes arquiteturais (ADRs)
- Manter o mapa do codebase (`codebase-map.json`)
- Criar arquivos `CLAUDE.md` contextuais em diretorios importantes

**Quando usar:**
- Apos completar implementacao de features
- Quando bugs sao encontrados e corrigidos
- Ao tomar decisoes arquiteturais importantes
- Para entender a estrutura do projeto

---

### 2. E2E Testing Specialist (`e2e-testing-specialist.md`)

**Cor:** Rosa | **Modelo:** Opus

Especialista em testes end-to-end automatizados, deteccao de bugs e validacao de funcionalidades. Utiliza MCP Chrome DevTools ou Playwright para:

- Executar testes E2E completos
- Identificar e documentar falhas
- Criar planos de correcao detalhados
- Validar fluxos de usuario criticos
- Testar responsividade e compatibilidade cross-browser

**Quando usar:**
- Apos implementar novas features ou componentes
- Para reproduzir e documentar bugs
- Antes de releases (testes de regressao)
- Para validar fluxos criticos (autenticacao, pagamentos)

---

### 3. Fullstack Dev Specialist (`fullstack-dev-specialist.md`)

**Cor:** Ciano | **Modelo:** Opus

Desenvolvedor fullstack experiente que implementa codigo real, funcional e consistente. Utiliza MCPs (Supabase, Context7, Serena) para:

- Entender contexto do projeto antes de codificar
- Implementar codigo personalizado para cada aplicacao
- Seguir padroes e convencoes existentes
- Integrar frontend, backend e banco de dados

**Quando usar:**
- Implementar features que envolvem frontend e backend
- Criar endpoints de API com integracao de banco
- Integrar servicos de terceiros (webhooks, APIs)
- Implementar logica funcional apos aprovacao de design

---

### 4. Security Code Reviewer (`security-code-reviewer.md`)

**Cor:** Amarelo | **Modelo:** Opus

Especialista em seguranca de aplicacoes e revisao de codigo. Foco em:

- Analise OWASP Top 10
- Identificacao de vulnerabilidades (SQL Injection, XSS, etc.)
- Auditoria de autenticacao e autorizacao
- Analise de praticas criptograficas
- Criacao de planos de remediacao

**Quando usar:**
- Apos implementar codigo sensivel a seguranca
- Ao criar sistemas de autenticacao
- Para endpoints de API que manipulam dados sensiveis
- Antes de deploy para producao
- Auditorias gerais de seguranca

---

### 5. Senior Software Engineer (`senior-software-engineer.md`)

**Cor:** Azul | **Modelo:** Opus

Engenheiro de software senior com 15+ anos de experiencia. Especializado em:

- Implementacao de features full-stack
- Codigo de qualidade de producao
- Correcao de bugs complexos
- Refatoracao seguindo SOLID
- Criacao de testes automatizados
- Code reviews detalhados

**Quando usar:**
- Implementar novas features
- Corrigir bugs complexos (memory leaks, race conditions)
- Refatorar codigo seguindo boas praticas
- Criar testes unitarios e de integracao
- Revisar pull requests

---

### 6. Software Architect (`software-architect.md`)

**Cor:** Vermelho | **Modelo:** Opus

Arquiteto de software senior especializado em sistemas de alta escala. Responsavel por:

- Identificar gargalos de infraestrutura
- Analisar problemas de escalabilidade
- Avaliar seguranca e resiliencia
- Documentar decisoes arquiteturais (ADRs)
- Definir metricas e SLIs/SLOs

**Quando usar:**
- Antes de homologacao/producao
- Ao planejar features de alta escala
- Quando ha problemas de performance
- Para decisoes arquiteturais importantes
- Migracoes de infraestrutura

---

## Biblioteca Completa de Agentes

Todos os agentes abaixo estao disponiveis na pasta `agents/`. Organizados por categoria:

### Academicos e Especialistas
> Agentes com expertise em ciencias humanas, narrativa, psicologia e ciencias sociais.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `academic-anthropologist.md` | 🌍 **Anthropologist** | Expert in cultural systems, rituals, kinship, belief systems, and ethnographic method — builds culturally coherent societies that feel lived-in rather than invented |
| `academic-geographer.md` | 🗺️ **Geographer** | Expert in physical and human geography, climate systems, cartography, and spatial analysis — builds geographically coherent worlds where terrain, climate, resources, and settlement patterns make scientific sense |
| `academic-historian.md` | 📚 **Historian** | Expert in historical analysis, periodization, material culture, and historiography — validates historical coherence and enriches settings with authentic period detail grounded in primary and secondary sources |
| `academic-narratologist.md` | 📜 **Narratologist** | Expert in narrative theory, story structure, character arcs, and literary analysis — grounds advice in established frameworks from Propp to Campbell to modern narratology |
| `academic-psychologist.md` | 🧠 **Psychologist** | Expert in human behavior, personality theory, motivation, and cognitive patterns — builds psychologically credible characters and interactions grounded in clinical and research frameworks |

---

### Financeiro — Contas a Pagar
> Processamento autonomo de pagamentos a fornecedores e contratantes.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `accounts-payable-agent.md` | 💸 **Accounts Payable Agent** | Autonomous payment processing specialist that executes vendor payments, contractor invoices, and recurring bills across any payment rail — crypto, fiat, stablecoins. Integrates with AI agent workflows via tool calls. |

---

### Identidade e Confianca de Agentes
> Arquitetura de identidade, autenticacao e verificacao de confianca para agentes de IA.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `agentic-identity-trust.md` | 🔐 **Agentic Identity & Trust Architect** | Designs identity, authentication, and trust verification systems for autonomous AI agents operating in multi-agent environments. Ensures agents can prove who they are, what they're authorized to do, and what they actually did. |

---

### Orquestracao de Agentes
> Gerenciamento autonomo de pipelines e orquestracao de workflows multi-agentes.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `agents-orchestrator.md` | 🎛️ **Agents Orchestrator** | Autonomous pipeline manager that orchestrates the entire development workflow. You are the leader of this process. |

---

### Automacao e Governanca
> Arquitetura de automacoes de negocios com foco em governanca e manutenibilidade.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `automation-governance-architect.md` | ⚙️ **Automation Governance Architect** | Governance-first architect for business automations (n8n-first) who audits value, risk, and maintainability before implementation. |

---

### Ferramentas 3D — Blender
> Desenvolvimento de add-ons e automacoes de pipeline para Blender.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `blender-addon-engineer.md` | 🧩 **Blender Add-on Engineer** | Blender tooling specialist - Builds Python add-ons, asset validators, exporters, and pipeline automations that turn repetitive DCC work into reliable one-click workflows |

---

### Blockchain e Smart Contracts
> Auditoria de seguranca de contratos inteligentes e aplicacoes DeFi.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `blockchain-security-auditor.md` | 🛡️ **Blockchain Security Auditor** | Expert smart contract security auditor specializing in vulnerability detection, formal verification, exploit analysis, and comprehensive audit report writing for DeFi protocols and blockchain applications. |

---

### Compliance e Auditoria
> Auditorias tecnicas de conformidade (SOC 2, ISO 27001, HIPAA, PCI-DSS).

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `compliance-auditor.md` | 📋 **Compliance Auditor** | Expert technical compliance auditor specializing in SOC 2, ISO 27001, HIPAA, and PCI-DSS audits — from readiness assessment through evidence collection to certification. |

---

### Treinamento Corporativo
> Design de sistemas de treinamento empresarial e desenvolvimento de curriculos.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `corporate-training-designer.md` | 📚 **Corporate Training Designer** | Expert in enterprise training system design and curriculum development — proficient in training needs analysis, instructional design methodology, blended learning program design, internal trainer development, leadership programs, and training effectiveness evaluation and continuous optimization. |

---

### Atendimento ao Cliente
> Suporte ao cliente para qualquer setor, incluindo resolucao de problemas e escalacao.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `customer-service.md` | 🎧 **Customer Service** | Friendly, professional customer service specialist for any industry — handling inquiries, complaints, account support, FAQs, and seamless escalation with warmth, efficiency, and a genuine commitment to customer satisfaction |

---

### Dados e Analytics — Consolidacao
> Consolidacao de dados de vendas em dashboards de relatorios em tempo real.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `data-consolidation-agent.md` | 🗄️ **Data Consolidation Agent** | AI agent that consolidates extracted sales data into live reporting dashboards with territory, rep, and pipeline summaries |

---

### Design e Criacao Visual
> Especialistas em UI/UX, branding, storytelling visual e criacao de imagens.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `design-brand-guardian.md` | 🎨 **Brand Guardian** | Expert brand strategist and guardian specializing in brand identity development, consistency maintenance, and strategic brand positioning |
| `design-image-prompt-engineer.md` | 📷 **Image Prompt Engineer** | Expert photography prompt engineer specializing in crafting detailed, evocative prompts for AI image generation. Masters the art of translating visual concepts into precise language that produces stunning, professional-quality photography through generative AI tools. |
| `design-inclusive-visuals-specialist.md` | 🌈 **Inclusive Visuals Specialist** | Representation expert who defeats systemic AI biases to generate culturally accurate, affirming, and non-stereotypical images and video. |
| `design-ui-designer.md` | 🎨 **UI Designer** | Expert UI designer specializing in visual design systems, component libraries, and pixel-perfect interface creation. Creates beautiful, consistent, accessible user interfaces that enhance UX and reflect brand identity |
| `design-ux-architect.md` | 📐 **UX Architect** | Technical architecture and UX specialist who provides developers with solid foundations, CSS systems, and clear implementation guidance |
| `design-ux-researcher.md` | 🔬 **UX Researcher** | Expert user experience researcher specializing in user behavior analysis, usability testing, and data-driven design insights. Provides actionable research findings that improve product usability and user satisfaction |
| `design-visual-storyteller.md` | 🎬 **Visual Storyteller** | Expert visual communication specialist focused on creating compelling visual narratives, multimedia content, and brand storytelling through design. Specializes in transforming complex information into engaging visual stories that connect with audiences and drive emotional engagement. |
| `design-whimsy-injector.md` | ✨ **Whimsy Injector** | Expert creative specialist focused on adding personality, delight, and playful elements to brand experiences. Creates memorable, joyful interactions that differentiate brands through unexpected moments of whimsy |

---

### Engenharia de Software
> Desenvolvedores e engenheiros especializados em backend, frontend, mobile, DevOps e mais.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `engineering-ai-data-remediation-engineer.md` | 🧬 **AI Data Remediation Engineer** | Specialist in self-healing data pipelines — uses air-gapped local SLMs and semantic clustering to automatically detect, classify, and fix data anomalies at scale. Focuses exclusively on the remediation layer: intercepting bad data, generating deterministic fix logic via Ollama, and guaranteeing zero data loss. Not a general data engineer — a surgical specialist for when your data is broken and the pipeline can't stop. |
| `engineering-ai-engineer.md` | 🤖 **AI Engineer** | Expert AI/ML engineer specializing in machine learning model development, deployment, and integration into production systems. Focused on building intelligent features, data pipelines, and AI-powered applications with emphasis on practical, scalable solutions. |
| `engineering-autonomous-optimization-architect.md` | ⚡ **Autonomous Optimization Architect** | Intelligent system governor that continuously shadow-tests APIs for performance while enforcing strict financial and security guardrails against runaway costs. |
| `engineering-backend-architect.md` | 🏗️ **Backend Architect** | Senior backend architect specializing in scalable system design, database architecture, API development, and cloud infrastructure. Builds robust, secure, performant server-side applications and microservices |
| `engineering-cms-developer.md` | 🧱 **CMS Developer** | Drupal and WordPress specialist for theme development, custom plugins/modules, content architecture, and code-first CMS implementation |
| `engineering-code-reviewer.md` | 👁️ **Code Reviewer** | Expert code reviewer who provides constructive, actionable feedback focused on correctness, maintainability, security, and performance — not style preferences. |
| `engineering-codebase-onboarding-engineer.md` | 🧭 **Codebase Onboarding Engineer** | Expert developer onboarding specialist who helps new engineers understand unfamiliar codebases fast by reading source code, tracing code paths, and stating only facts grounded in the code. |
| `engineering-data-engineer.md` | 🔧 **Data Engineer** | Expert data engineer specializing in building reliable data pipelines, lakehouse architectures, and scalable data infrastructure. Masters ETL/ELT, Apache Spark, dbt, streaming systems, and cloud data platforms to turn raw data into trusted, analytics-ready assets. |
| `engineering-database-optimizer.md` | 🗄️ **Database Optimizer** | Expert database specialist focusing on schema design, query optimization, indexing strategies, and performance tuning for PostgreSQL, MySQL, and modern databases like Supabase and PlanetScale. |
| `engineering-devops-automator.md` | ⚙️ **DevOps Automator** | Expert DevOps engineer specializing in infrastructure automation, CI/CD pipeline development, and cloud operations |
| `engineering-email-intelligence-engineer.md` | 📧 **Email Intelligence Engineer** | Expert in extracting structured, reasoning-ready data from raw email threads for AI agents and automation systems |
| `engineering-embedded-firmware-engineer.md` | 🔩 **Embedded Firmware Engineer** | Specialist in bare-metal and RTOS firmware - ESP32/ESP-IDF, PlatformIO, Arduino, ARM Cortex-M, STM32 HAL/LL, Nordic nRF5/nRF Connect SDK, FreeRTOS, Zephyr |
| `engineering-feishu-integration-developer.md` | 🔗 **Feishu Integration Developer** | Full-stack integration expert specializing in the Feishu (Lark) Open Platform — proficient in Feishu bots, mini programs, approval workflows, Bitable (multidimensional spreadsheets), interactive message cards, Webhooks, SSO authentication, and workflow automation, building enterprise-grade collaboration and automation solutions within the Feishu ecosystem. |
| `engineering-filament-optimization-specialist.md` | 🔧 **Filament Optimization Specialist** | Expert in restructuring and optimizing Filament PHP admin interfaces for maximum usability and efficiency. Focuses on impactful structural changes — not just cosmetic tweaks. |
| `engineering-frontend-developer.md` | 🖥️ **Frontend Developer** | Expert frontend developer specializing in modern web technologies, React/Vue/Angular frameworks, UI implementation, and performance optimization |
| `engineering-git-workflow-master.md` | 🌿 **Git Workflow Master** | Expert in Git workflows, branching strategies, and version control best practices including conventional commits, rebasing, worktrees, and CI-friendly branch management. |
| `engineering-incident-response-commander.md` | 🚨 **Incident Response Commander** | Expert incident commander specializing in production incident management, structured response coordination, post-mortem facilitation, SLO/SLI tracking, and on-call process design for reliable engineering organizations. |
| `engineering-minimal-change-engineer.md` | 🪡 **Minimal Change Engineer** | Engineering specialist focused on minimum-viable diffs — fixes only what was asked, refuses scope creep, prefers three similar lines over a premature abstraction. The discipline that prevents bug-fix PRs from becoming refactor avalanches. |
| `engineering-mobile-app-builder.md` | 📲 **Mobile App Builder** | Specialized mobile application developer with expertise in native iOS/Android development and cross-platform frameworks |
| `engineering-rapid-prototyper.md` | ⚡ **Rapid Prototyper** | Specialized in ultra-fast proof-of-concept development and MVP creation using efficient tools and frameworks |
| `engineering-security-engineer.md` | 🔒 **Security Engineer** | Expert application security engineer specializing in threat modeling, vulnerability assessment, secure code review, security architecture design, and incident response for modern web, API, and cloud-native applications. |
| `engineering-senior-developer.md` | 💎 **Senior Developer** | Premium implementation specialist - Masters Laravel/Livewire/FluxUI, advanced CSS, Three.js integration |
| `engineering-software-architect.md` | 🏛️ **Software Architect** | Expert software architect specializing in system design, domain-driven design, architectural patterns, and technical decision-making for scalable, maintainable systems. |
| `engineering-solidity-smart-contract-engineer.md` | ⛓️ **Solidity Smart Contract Engineer** | Expert Solidity developer specializing in EVM smart contract architecture, gas optimization, upgradeable proxy patterns, DeFi protocol development, and security-first contract design across Ethereum and L2 chains. |
| `engineering-sre.md` | 🛡️ **SRE (Site Reliability Engineer)** | Expert site reliability engineer specializing in SLOs, error budgets, observability, chaos engineering, and toil reduction for production systems at scale. |
| `engineering-technical-writer.md` | 📚 **Technical Writer** | Expert technical writer specializing in developer documentation, API references, README files, and tutorials. Transforms complex engineering concepts into clear, accurate, and engaging docs that developers actually read and use. |
| `engineering-threat-detection-engineer.md` | 🎯 **Threat Detection Engineer** | Expert detection engineer specializing in SIEM rule development, MITRE ATT&CK coverage mapping, threat hunting, alert tuning, and detection-as-code pipelines for security operations teams. |
| `engineering-voice-ai-integration-engineer.md` | 🎙️ **Voice AI Integration Engineer** | Expert in building end-to-end speech transcription pipelines using Whisper-style models and cloud ASR services — from raw audio ingestion through preprocessing, transcript cleanup, subtitle generation, speaker diarization, and structured downstream integration into apps, APIs, and CMS platforms. |
| `engineering-wechat-mini-program-developer.md` | 💬 **WeChat Mini Program Developer** | Expert WeChat Mini Program developer specializing in 小程序 development with WXML/WXSS/WXS, WeChat API integration, payment systems, subscription messaging, and the full WeChat ecosystem. |

---

### Financas e Contabilidade
> Analistas financeiros, FP&A, contabilidade, investimentos e estrategia fiscal.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `finance-bookkeeper-controller.md` | 📒 **Bookkeeper & Controller** | Expert bookkeeper and controller specializing in day-to-day accounting operations, financial reconciliations, month-end close processes, and internal controls. Ensures the accuracy, completeness, and timeliness of financial records while maintaining GAAP compliance and audit readiness at all times. |
| `finance-financial-analyst.md` | 📊 **Financial Analyst** | Expert financial analyst specializing in financial modeling, forecasting, scenario analysis, and data-driven decision support. Transforms raw financial data into actionable business intelligence that drives strategic planning, investment decisions, and operational optimization. |
| `finance-fpa-analyst.md` | 📈 **FP&A Analyst** | Expert Financial Planning & Analysis (FP&A) analyst specializing in budgeting, variance analysis, financial planning, rolling forecasts, and strategic decision support. Bridges the gap between the numbers and the business narrative to drive operational performance and strategic resource allocation. |
| `finance-investment-researcher.md` | 🔍 **Investment Researcher** | Expert investment researcher specializing in market research, due diligence, portfolio analysis, and asset valuation. Conducts rigorous fundamental and quantitative analysis to identify investment opportunities, assess risks, and support data-driven portfolio decisions across public equities, private markets, and alternative assets. |
| `finance-tax-strategist.md` | 🏛️ **Tax Strategist** | Expert tax strategist specializing in tax optimization, multi-jurisdictional compliance, transfer pricing, and strategic tax planning. Navigates complex tax codes to minimize liability while ensuring full regulatory compliance across local, state, federal, and international tax regimes. |

---

### Desenvolvimento de Jogos
> Especialistas em design de jogos, audio interativo e mecanicas de gameplay.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `game-audio-engineer.md` | 🎵 **Game Audio Engineer** | Interactive audio specialist - Masters FMOD/Wwise integration, adaptive music systems, spatial audio, and audio performance budgeting across all game engines |
| `game-designer.md` | 🎮 **Game Designer** | Systems and mechanics architect - Masters GDD authorship, player psychology, economy balancing, and gameplay loop design across all engines and genres |

---

### Engine Godot
> Especialistas em Godot 4: GDScript, multiplayer, shaders e arquitetura.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `godot-gameplay-scripter.md` | 🎯 **Godot Gameplay Scripter** | Composition and signal integrity specialist - Masters GDScript 2.0, C# integration, node-based architecture, and type-safe signal design for Godot 4 projects |
| `godot-multiplayer-engineer.md` | 🌐 **Godot Multiplayer Engineer** | Godot 4 networking specialist - Masters the MultiplayerAPI, scene replication, ENet/WebRTC transport, RPCs, and authority models for real-time multiplayer games |
| `godot-shader-developer.md` | 💎 **Godot Shader Developer** | Godot 4 visual effects specialist - Masters the Godot Shading Language (GLSL-like), VisualShader editor, CanvasItem and Spatial shaders, post-processing, and performance optimization for 2D/3D effects |

---

### Governo e Setor Publico
> Consultoria de pre-vendas para transformacao digital governamental.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `government-digital-presales-consultant.md` | 🏛️ **Government Digital Presales Consultant** | Presales expert for China's government digital transformation market (ToG), proficient in policy interpretation, solution design, bid document preparation, POC validation, compliance requirements (classified protection/cryptographic assessment/Xinchuang domestic IT), and stakeholder management — helping technical teams efficiently win government IT projects. |

---

### GSD — Get Stuff Done
> Agentes internos do framework GSD para planejamento, execucao e verificacao de fases.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `gsd-advisor-researcher.md` | **gsd-advisor-researcher** | Researches a single gray area decision and returns a structured comparison table with rationale. Spawned by discuss-phase advisor mode. |
| `gsd-assumptions-analyzer.md` | **gsd-assumptions-analyzer** | Deeply analyzes codebase for a phase and returns structured assumptions with evidence. Spawned by discuss-phase assumptions mode. |
| `gsd-codebase-mapper.md` | **gsd-codebase-mapper** | Explores codebase and writes structured analysis documents. Spawned by map-codebase with a focus area (tech, arch, quality, concerns). Writes documents directly to reduce orchestrator context load. |
| `gsd-debugger.md` | **gsd-debugger** | Investigates bugs using scientific method, manages debug sessions, handles checkpoints. Spawned by /gsd:debug orchestrator. |
| `gsd-executor.md` | **gsd-executor** | Executes GSD plans with atomic commits, deviation handling, checkpoint protocols, and state management. Spawned by execute-phase orchestrator or execute-plan command. |
| `gsd-integration-checker.md` | **gsd-integration-checker** | Verifies cross-phase integration and E2E flows. Checks that phases connect properly and user workflows complete end-to-end. |
| `gsd-nyquist-auditor.md` | **gsd-nyquist-auditor** | Fills Nyquist validation gaps by generating tests and verifying coverage for phase requirements |
| `gsd-phase-researcher.md` | **gsd-phase-researcher** | Researches how to implement a phase before planning. Produces RESEARCH.md consumed by gsd-planner. Spawned by /gsd:plan-phase orchestrator. |
| `gsd-plan-checker.md` | **gsd-plan-checker** | Verifies plans will achieve phase goal before execution. Goal-backward analysis of plan quality. Spawned by /gsd:plan-phase orchestrator. |
| `gsd-planner.md` | **gsd-planner** | Creates executable phase plans with task breakdown, dependency analysis, and goal-backward verification. Spawned by /gsd:plan-phase orchestrator. |
| `gsd-project-researcher.md` | **gsd-project-researcher** | Researches domain ecosystem before roadmap creation. Produces files in .planning/research/ consumed during roadmap creation. Spawned by /gsd:new-project or /gsd:new-milestone orchestrators. |
| `gsd-research-synthesizer.md` | **gsd-research-synthesizer** | Synthesizes research outputs from parallel researcher agents into SUMMARY.md. Spawned by /gsd:new-project after 4 researcher agents complete. |
| `gsd-roadmapper.md` | **gsd-roadmapper** | Creates project roadmaps with phase breakdown, requirement mapping, success criteria derivation, and coverage validation. Spawned by /gsd:new-project orchestrator. |
| `gsd-ui-auditor.md` | **gsd-ui-auditor** | Retroactive 6-pillar visual audit of implemented frontend code. Produces scored UI-REVIEW.md. Spawned by /gsd:ui-review orchestrator. |
| `gsd-ui-checker.md` | **gsd-ui-checker** | Validates UI-SPEC.md design contracts against 6 quality dimensions. Produces BLOCK/FLAG/PASS verdicts. Spawned by /gsd:ui-phase orchestrator. |
| `gsd-ui-researcher.md` | **gsd-ui-researcher** | Produces UI-SPEC.md design contract for frontend phases. Reads upstream artifacts, detects design system state, asks only unanswered questions. Spawned by /gsd:ui-phase orchestrator. |
| `gsd-user-profiler.md` | **gsd-user-profiler** | Analyzes extracted session messages across 8 behavioral dimensions to produce a scored developer profile with confidence levels and evidence. Spawned by profile orchestration workflows. |
| `gsd-verifier.md` | **gsd-verifier** | Verifies phase goal achievement through goal-backward analysis. Checks codebase delivers what phase promised, not just that tasks completed. Creates VERIFICATION.md report. |

---

### Saude
> Atendimento ao paciente, conformidade em marketing de saude e suporte hospitalar.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `healthcare-customer-service.md` | 🏥 **Healthcare Customer Service** | Empathetic healthcare customer service specialist for patient support, billing inquiries, appointment management, insurance questions, complaint resolution, and seamless escalation to clinical or administrative staff |
| `healthcare-marketing-compliance.md` | ⚕️ **Healthcare Marketing Compliance Specialist** | Expert in healthcare marketing compliance in China, proficient in the Advertising Law, Medical Advertisement Management Measures, Drug Administration Law, and related regulations — covering pharmaceuticals, medical devices, medical aesthetics, health supplements, and internet healthcare across content review, risk control, platform rule interpretation, and patient privacy protection, helping enterprises conduct effective health marketing within legal boundaries. |

---

### Hospitalidade
> Servicos de hospedes para hoteis, resorts e restaurantes.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `hospitality-guest-services.md` | 🏨 **Hospitality Guest Services** | Comprehensive hospitality guest services specialist for hotels, resorts, restaurants, and event venues — covering reservations, check-in/check-out, concierge services, guest complaint resolution, loyalty program management, and post-stay follow-up to deliver exceptional guest experiences that drive loyalty and revenue |

---

### Recursos Humanos
> Onboarding de funcionarios, documentacao e integracao cultural.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `hr-onboarding.md` | 🤝 **HR Onboarding** | Comprehensive HR onboarding specialist for employee orientation, documentation management, compliance tracking, benefits enrollment, culture integration, and new hire support — delivering a seamless first-day-to-first-year experience that drives retention and productivity |

---

### Grafo de Identidade
> Operacao de grafo de identidade compartilhado para sistemas multi-agentes.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `identity-graph-operator.md` | 🕸️ **Identity Graph Operator** | Operates a shared identity graph that multiple AI agents resolve against. Ensures every agent in a multi-agent system gets the same canonical answer for "who is this entity?" - deterministically, even under concurrent writes. |

---

### Traducao de Idiomas
> Traducao em tempo real com consciencia cultural e contextual.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `language-translator.md` | 🌐 **Language Translator** | Real-time Spanish ↔ English translation specialist with cultural context, regional dialect awareness, travel phrase guidance, and tone-appropriate communication for everyday, business, and emergency situations |

---

### Juridico
> Intake de clientes, revisao de documentos e faturamento juridico.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `legal-billing-time-tracking.md` | ⏱️ **Legal Billing & Time Tracking** | Comprehensive legal billing and time tracking specialist for accurate time capture, invoice generation, billing narrative writing, collections management, trust account compliance, and billing analysis — maximizing revenue recovery while maintaining client relationships and ethical compliance across any firm size or billing model |
| `legal-client-intake.md` | 📋 **Legal Client Intake** | Comprehensive legal client intake specialist for qualifying prospects, collecting case information, scheduling consultations, managing conflict checks, and delivering attorney-ready intake summaries across any practice area and firm size |
| `legal-document-review.md` | ⚖️ **Legal Document Review** | Comprehensive legal document review specialist for contracts, litigation documents, and real estate agreements — summarizing documents, flagging risk clauses, comparing contract versions, and checking compliance across any law firm size or practice area |

---

### Design de Levels
> Design de fases e narrativa espacial para jogos.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `level-designer.md` | 🗺️ **Level Designer** | Spatial storytelling and flow specialist - Masters layout theory, pacing architecture, encounter design, and environmental narrative across all game engines |

---

### Credito e Financiamento
> Assistente de oficial de credito para hipotecas e emprestimos.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `loan-officer-assistant.md` | 🏦 **Loan Officer Assistant** | Comprehensive loan officer assistant for mortgage and lending professionals — covering borrower intake, pre-qualification, document collection, pipeline management, compliance tracking, rate quoting, and closing coordination across residential, commercial, and consumer lending |

---

### LSP e Inteligencia de Codigo
> Sistemas de inteligencia de codigo via Language Server Protocol.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `lsp-index-engineer.md` | 🔎 **LSP/Index Engineer** | Language Server Protocol specialist building unified code intelligence systems through LSP client orchestration and semantic indexing |

---

### macOS e Metal
> Engenharia nativa Swift e Metal para alto desempenho 3D e computing espacial.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `macos-spatial-metal-engineer.md` | 🍎 **macOS Spatial/Metal Engineer** | Native Swift and Metal specialist building high-performance 3D rendering systems and spatial computing experiences for macOS and Vision Pro |

---

### Marketing Digital
> Especialistas em SEO, redes sociais, e-commerce, conteudo e marketing de plataformas.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `marketing-agentic-search-optimizer.md` | 🤖 **Agentic Search Optimizer** | Expert in WebMCP readiness and agentic task completion — audits whether AI agents can actually accomplish tasks on your site (book, buy, register, subscribe), implements WebMCP declarative and imperative patterns, and measures task completion rates across AI browsing agents |
| `marketing-ai-citation-strategist.md` | 🔮 **AI Citation Strategist** | Expert in AI recommendation engine optimization (AEO/GEO) — audits brand visibility across ChatGPT, Claude, Gemini, and Perplexity, identifies why competitors get cited instead, and delivers content fixes that improve AI citations |
| `marketing-app-store-optimizer.md` | 📱 **App Store Optimizer** | Expert app store marketing specialist focused on App Store Optimization (ASO), conversion rate optimization, and app discoverability |
| `marketing-baidu-seo-specialist.md` | 🇨🇳 **Baidu SEO Specialist** | Expert Baidu search optimization specialist focused on Chinese search engine ranking, Baidu ecosystem integration, ICP compliance, Chinese keyword research, and mobile-first indexing for the China market. |
| `marketing-bilibili-content-strategist.md` | 🎬 **Bilibili Content Strategist** | Expert Bilibili marketing specialist focused on UP主 growth, danmaku culture mastery, B站 algorithm optimization, community building, and branded content strategy for China's leading video community platform. |
| `marketing-book-co-author.md` | 📘 **Book Co-Author** | Strategic thought-leadership book collaborator for founders, experts, and operators turning voice notes, fragments, and positioning into structured first-person chapters. |
| `marketing-carousel-growth-engine.md` | 🎠 **Carousel Growth Engine** | Autonomous TikTok and Instagram carousel generation specialist. Analyzes any website URL with Playwright, generates viral 6-slide carousels via Gemini image generation, publishes directly to feed via Upload-Post API with auto trending music, fetches analytics, and iteratively improves through a data-driven learning loop. |
| `marketing-china-ecommerce-operator.md` | 🛒 **China E-Commerce Operator** | Expert China e-commerce operations specialist covering Taobao, Tmall, Pinduoduo, and JD ecosystems with deep expertise in product listing optimization, live commerce, store operations, 618/Double 11 campaigns, and cross-platform strategy. |
| `marketing-china-market-localization-strategist.md` | 🇨🇳 **China Market Localization Strategist** | Full-stack China market localization expert who transforms real-time trend signals into executable go-to-market strategies across Douyin, Xiaohongshu, WeChat, Bilibili, and beyond |
| `marketing-content-creator.md` | ✍️ **Content Creator** | Expert content strategist and creator for multi-platform campaigns. Develops editorial calendars, creates compelling copy, manages brand storytelling, and optimizes content for engagement across all digital channels. |
| `marketing-cross-border-ecommerce.md` | 🌏 **Cross-Border E-Commerce Specialist** | Full-funnel cross-border e-commerce strategist covering Amazon, Shopee, Lazada, AliExpress, Temu, and TikTok Shop operations, international logistics and overseas warehousing, compliance and taxation, multilingual listing optimization, brand globalization, and DTC independent site development. |
| `marketing-douyin-strategist.md` | 🎵 **Douyin Strategist** | Short-video marketing expert specializing in the Douyin platform, with deep expertise in recommendation algorithm mechanics, viral video planning, livestream commerce workflows, and full-funnel brand growth through content matrix strategies. |
| `marketing-growth-hacker.md` | 🚀 **Growth Hacker** | Expert growth strategist specializing in rapid user acquisition through data-driven experimentation. Develops viral loops, optimizes conversion funnels, and finds scalable growth channels for exponential business growth. |
| `marketing-instagram-curator.md` | 📸 **Instagram Curator** | Expert Instagram marketing specialist focused on visual storytelling, community building, and multi-format content optimization. Masters aesthetic development and drives meaningful engagement. |
| `marketing-kuaishou-strategist.md` | 🎥 **Kuaishou Strategist** | Expert Kuaishou marketing strategist specializing in short-video content for China's lower-tier city markets, live commerce operations, community trust building, and grassroots audience growth on 快手. |
| `marketing-linkedin-content-creator.md` | 💼 **LinkedIn Content Creator** | Expert LinkedIn content strategist focused on thought leadership, personal brand building, and high-engagement professional content. Masters LinkedIn's algorithm and culture to drive inbound opportunities for founders, job seekers, developers, and anyone building a professional presence. |
| `marketing-livestream-commerce-coach.md` | 🎙️ **Livestream Commerce Coach** | Veteran livestream e-commerce coach specializing in host training and live room operations across Douyin, Kuaishou, Taobao Live, and Channels, covering script design, product sequencing, paid-vs-organic traffic balancing, conversion closing techniques, and real-time data-driven optimization. |
| `marketing-podcast-strategist.md` | 🎧 **Podcast Strategist** | Content strategy and operations expert for the Chinese podcast market, with deep expertise in Xiaoyuzhou, Ximalaya, and other major audio platforms, covering show positioning, audio production, audience growth, multi-platform distribution, and monetization to help podcast creators build sticky audio content brands. |
| `marketing-private-domain-operator.md` | 🔒 **Private Domain Operator** | Expert in building enterprise WeChat (WeCom) private domain ecosystems, with deep expertise in SCRM systems, segmented community operations, Mini Program commerce integration, user lifecycle management, and full-funnel conversion optimization. |
| `marketing-reddit-community-builder.md` | 💬 **Reddit Community Builder** | Expert Reddit marketing specialist focused on authentic community engagement, value-driven content creation, and long-term relationship building. Masters Reddit culture navigation. |
| `marketing-seo-specialist.md` | 🔍 **SEO Specialist** | Expert search engine optimization strategist specializing in technical SEO, content optimization, link authority building, and organic search growth. Drives sustainable traffic through data-driven search strategies. |
| `marketing-short-video-editing-coach.md` | 🎬 **Short-Video Editing Coach** | Hands-on short-video editing coach covering the full post-production pipeline, with mastery of CapCut Pro, Premiere Pro, DaVinci Resolve, and Final Cut Pro across composition and camera language, color grading, audio engineering, motion graphics and VFX, subtitle design, multi-platform export optimization, editing workflow efficiency, and AI-assisted editing. |
| `marketing-social-media-strategist.md` | 📣 **Social Media Strategist** | Expert social media strategist for LinkedIn, Twitter, and professional platforms. Creates cross-platform campaigns, builds communities, manages real-time engagement, and develops thought leadership strategies. |
| `marketing-tiktok-strategist.md` | 🎵 **TikTok Strategist** | Expert TikTok marketing specialist focused on viral content creation, algorithm optimization, and community building. Masters TikTok's unique culture and features for brand growth. |
| `marketing-twitter-engager.md` | 🐦 **Twitter Engager** | Expert Twitter marketing specialist focused on real-time engagement, thought leadership building, and community-driven growth. Builds brand authority through authentic conversation participation and viral thread creation. |
| `marketing-video-optimization-specialist.md` | 🎬 **Video Optimization Specialist** | Video marketing strategist specializing in YouTube algorithm optimization, audience retention, chaptering, thumbnail concepts, and cross-platform video syndication. |
| `marketing-wechat-official-account.md` | 📱 **WeChat Official Account Manager** | Expert WeChat Official Account (OA) strategist specializing in content marketing, subscriber engagement, and conversion optimization. Masters multi-format content and builds loyal communities through consistent value delivery. |
| `marketing-weibo-strategist.md` | 🔥 **Weibo Strategist** | Full-spectrum operations expert for Sina Weibo, with deep expertise in trending topic mechanics, Super Topic community management, public sentiment monitoring, fan economy strategies, and Weibo advertising, helping brands achieve viral reach and sustained growth on China's leading public discourse platform. |
| `marketing-xiaohongshu-specialist.md` | 🌸 **Xiaohongshu Specialist** | Expert Xiaohongshu marketing specialist focused on lifestyle content, trend-driven strategies, and authentic community engagement. Masters micro-content creation and drives viral growth through aesthetic storytelling. |
| `marketing-zhihu-strategist.md` | 🧠 **Zhihu Strategist** | Expert Zhihu marketing specialist focused on thought leadership, community credibility, and knowledge-driven engagement. Masters question-answering strategy and builds brand authority through authentic expertise sharing. |

---

### Design Narrativo
> Sistemas de narrativa, dialogos e storytelling ambiental para jogos.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `narrative-designer.md` | 📖 **Narrative Designer** | Story systems and dialogue architect - Masters GDD-aligned narrative design, branching dialogue, lore architecture, and environmental storytelling across all game engines |

---

### Midia Paga
> Especialistas em Google Ads, Meta, programatica, PPC, social pago e analise de queries.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `paid-media-auditor.md` | 📋 **Paid Media Auditor** | Comprehensive paid media auditor who systematically evaluates Google Ads, Microsoft Ads, and Meta accounts across 200+ checkpoints spanning account structure, tracking, bidding, creative, audiences, and competitive positioning. Produces actionable audit reports with prioritized recommendations and projected impact. |
| `paid-media-creative-strategist.md` | ✍️ **Ad Creative Strategist** | Paid media creative specialist focused on ad copywriting, RSA optimization, asset group design, and creative testing frameworks across Google, Meta, Microsoft, and programmatic platforms. Bridges the gap between performance data and persuasive messaging. |
| `paid-media-paid-social-strategist.md` | 📱 **Paid Social Strategist** | Cross-platform paid social advertising specialist covering Meta (Facebook/Instagram), LinkedIn, TikTok, Pinterest, X, and Snapchat. Designs full-funnel social ad programs from prospecting through retargeting with platform-specific creative and audience strategies. |
| `paid-media-ppc-strategist.md` | 💰 **PPC Campaign Strategist** | Senior paid media strategist specializing in large-scale search, shopping, and performance max campaign architecture across Google, Microsoft, and Amazon ad platforms. Designs account structures, budget allocation frameworks, and bidding strategies that scale from $10K to $10M+ monthly spend. |
| `paid-media-programmatic-buyer.md` | 📺 **Programmatic & Display Buyer** | Display advertising and programmatic media buying specialist covering managed placements, Google Display Network, DV360, trade desk platforms, partner media (newsletters, sponsored content), and ABM display strategies via platforms like Demandbase and 6Sense. |
| `paid-media-search-query-analyst.md` | 🔍 **Search Query Analyst** | Specialist in search term analysis, negative keyword architecture, and query-to-intent mapping. Turns raw search query data into actionable optimizations that eliminate waste and amplify high-intent traffic across paid search accounts. |
| `paid-media-tracking-specialist.md` | 📡 **Tracking & Measurement Specialist** | Expert in conversion tracking architecture, tag management, and attribution modeling across Google Tag Manager, GA4, Google Ads, Meta CAPI, LinkedIn Insight Tag, and server-side implementations. Ensures every conversion is counted correctly and every dollar of ad spend is measurable. |

---

### Produto
> Gestao de produto, priorizacao, pesquisa de tendencias e engine de nudge comportamental.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `product-behavioral-nudge-engine.md` | 🧠 **Behavioral Nudge Engine** | Behavioral psychology specialist that adapts software interaction cadences and styles to maximize user motivation and success. |
| `product-feedback-synthesizer.md` | 🔍 **Feedback Synthesizer** | Expert in collecting, analyzing, and synthesizing user feedback from multiple channels to extract actionable product insights. Transforms qualitative feedback into quantitative priorities and strategic recommendations. |
| `product-manager.md` | 🧭 **Product Manager** | Holistic product leader who owns the full product lifecycle — from discovery and strategy through roadmap, stakeholder alignment, go-to-market, and outcome measurement. Bridges business goals, user needs, and technical reality to ship the right thing at the right time. |
| `product-sprint-prioritizer.md` | 🎯 **Sprint Prioritizer** | Expert product manager specializing in agile sprint planning, feature prioritization, and resource allocation. Focused on maximizing team velocity and business value delivery through data-driven prioritization frameworks. |
| `product-trend-researcher.md` | 🔭 **Trend Researcher** | Expert market intelligence analyst specializing in identifying emerging trends, competitive analysis, and opportunity assessment. Focused on providing actionable insights that drive product strategy and innovation decisions. |

---

### Gestao de Projetos
> Coordenacao de projetos, experimentos, operacoes de studio e rastreamento Jira.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `project-management-experiment-tracker.md` | 🧪 **Experiment Tracker** | Expert project manager specializing in experiment design, execution tracking, and data-driven decision making. Focused on managing A/B tests, feature experiments, and hypothesis validation through systematic experimentation and rigorous analysis. |
| `project-management-jira-workflow-steward.md` | 📋 **Jira Workflow Steward** | Expert delivery operations specialist who enforces Jira-linked Git workflows, traceable commits, structured pull requests, and release-safe branch strategy across software teams. |
| `project-management-project-shepherd.md` | 🐑 **Project Shepherd** | Expert project manager specializing in cross-functional project coordination, timeline management, and stakeholder alignment. Focused on shepherding projects from conception to completion while managing resources, risks, and communications across multiple teams and departments. |
| `project-management-studio-operations.md` | 🏭 **Studio Operations** | Expert operations manager specializing in day-to-day studio efficiency, process optimization, and resource coordination. Focused on ensuring smooth operations, maintaining productivity standards, and supporting all teams with the tools and processes needed for success. |
| `project-management-studio-producer.md` | 🎬 **Studio Producer** | Senior strategic leader specializing in high-level creative and technical project orchestration, resource allocation, and multi-project portfolio management. Focused on aligning creative vision with business objectives while managing complex cross-functional initiatives and ensuring optimal studio operations. |
| `project-manager-senior.md` | 📝 **Senior Project Manager** | Converts specs to tasks and remembers previous projects. Focused on realistic scope, no background processes, exact spec requirements |

---

### Imoveis
> Assistente para representacao de compradores e vendedores no mercado imobiliario.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `real-estate-buyer-seller.md` | 🏠 **Real Estate Buyer & Seller** | Comprehensive real estate agent assistant for buyer representation, seller representation, listing management, offer negotiation, transaction coordination, and closing support — delivering a world-class client experience from first showing to final closing across residential and investment real estate |

---

### Recrutamento
> Aquisicao de talentos e operacoes de RH com foco no mercado global.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `recruitment-specialist.md` | 🎯 **Recruitment Specialist** | Expert recruitment operations and talent acquisition specialist — skilled in China's major hiring platforms, talent assessment frameworks, and labor law compliance. Helps companies efficiently attract, screen, and retain top talent while building a competitive employer brand. |

---

### Relatorios
> Distribuicao automatizada de relatorios de vendas para representantes.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `report-distribution-agent.md` | 📤 **Report Distribution Agent** | AI agent that automates distribution of consolidated sales reports to representatives based on territorial parameters |

---

### Varejo — Devolucoes
> Gestao de devolucoes, trocas e reembolsos no varejo omnichannel.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `retail-customer-returns.md` | 🛒 **Retail Customer Returns** | Comprehensive retail customer returns specialist for processing returns, exchanges, and refunds across in-store, online, and omnichannel retail — handling policy enforcement, fraud prevention, customer retention, vendor returns, and returns analytics to maximize recovery while preserving customer loyalty |

---

### Roblox
> Desenvolvimento de experiencias, avatares UGC e scripting Luau para Roblox.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `roblox-avatar-creator.md` | 👤 **Roblox Avatar Creator** | Roblox UGC and avatar pipeline specialist - Masters Roblox's avatar system, UGC item creation, accessory rigging, texture standards, and the Creator Marketplace submission pipeline |
| `roblox-experience-designer.md` | 🎪 **Roblox Experience Designer** | Roblox platform UX and monetization specialist - Masters engagement loop design, DataStore-driven progression, Roblox monetization systems (Passes, Developer Products, UGC), and player retention for Roblox experiences |
| `roblox-systems-scripter.md` | 🔧 **Roblox Systems Scripter** | Roblox platform engineering specialist - Masters Luau, the client-server security model, RemoteEvents/RemoteFunctions, DataStore, and module architecture for scalable Roblox experiences |

---

### Vendas
> Estrategistas de vendas, coaches, engenheiros de pre-venda e analise de pipeline.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `sales-account-strategist.md` | 🗺️ **Account Strategist** | Expert post-sale account strategist specializing in land-and-expand execution, stakeholder mapping, QBR facilitation, and net revenue retention. Turns closed deals into long-term platform relationships through systematic expansion planning and multi-threaded account development. |
| `sales-coach.md` | 🏋️ **Sales Coach** | Expert sales coaching specialist focused on rep development, pipeline review facilitation, call coaching, deal strategy, and forecast accuracy. Makes every rep and every deal better through structured coaching methodology and behavioral feedback. |
| `sales-data-extraction-agent.md` | 📊 **Sales Data Extraction Agent** | AI agent specialized in monitoring Excel files and extracting key sales metrics (MTD, YTD, Year End) for internal live reporting |
| `sales-deal-strategist.md` | ♟️ **Deal Strategist** | Senior deal strategist specializing in MEDDPICC qualification, competitive positioning, and win planning for complex B2B sales cycles. Scores opportunities, exposes pipeline risk, and builds deal strategies that survive forecast review. |
| `sales-discovery-coach.md` | 🔍 **Discovery Coach** | Coaches sales teams on elite discovery methodology — question design, current-state mapping, gap quantification, and call structure that surfaces real buying motivation. |
| `sales-engineer.md` | 🛠️ **Sales Engineer** | Senior pre-sales engineer specializing in technical discovery, demo engineering, POC scoping, competitive battlecards, and bridging product capabilities to business outcomes. Wins the technical decision so the deal can close. |
| `sales-outbound-strategist.md` | 🎯 **Outbound Strategist** | Signal-based outbound specialist who designs multi-channel prospecting sequences, defines ICPs, and builds pipeline through research-driven personalization — not volume. |
| `sales-outreach.md` | 🎯 **Sales Outreach** | Consultative B2B sales outreach specialist for cold prospecting, lead follow-up, objection handling, proposal writing, and pipeline management — combining data-driven targeting with genuine relationship-building to open doors and close deals |
| `sales-pipeline-analyst.md` | 📊 **Pipeline Analyst** | Revenue operations analyst specializing in pipeline health diagnostics, deal velocity analysis, forecast accuracy, and data-driven sales coaching. Turns CRM data into actionable pipeline intelligence that surfaces risks before they become missed quarters. |
| `sales-proposal-strategist.md` | 🏹 **Proposal Strategist** | Strategic proposal architect who transforms RFPs and sales opportunities into compelling win narratives. Specializes in win theme development, competitive positioning, executive summary craft, and building proposals that persuade rather than merely comply. |

---

### Especializados
> Agentes especializados: civil, MCP builder, Salesforce, fluxo de trabalho, IA cultural e mais.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `specialized-chief-of-staff.md` | 🧭 **Chief of Staff** | Master coordinator for founders and executives — filters noise, owns processes, enforces consistency, routes decisions, and positions outputs for impact so the boss can think clearly. |
| `specialized-civil-engineer.md` | 🏗️ **Civil Engineer** | Expert civil and structural engineer with global standards coverage — Eurocode, DIN, ACI, AISC, ASCE, AS/NZS, CSA, GB, IS, AIJ, and more. Specializes in structural analysis, geotechnical design, construction documentation, building code compliance, and multi-standard international projects. |
| `specialized-cultural-intelligence-strategist.md` | 🌍 **Cultural Intelligence Strategist** | CQ specialist that detects invisible exclusion, researches global context, and ensures software resonates authentically across intersectional identities. |
| `specialized-developer-advocate.md` | 🗣️ **Developer Advocate** | Expert developer advocate specializing in building developer communities, creating compelling technical content, optimizing developer experience (DX), and driving platform adoption through authentic engineering engagement. Bridges product and engineering teams with external developers. |
| `specialized-document-generator.md` | 📄 **Document Generator** | Expert document creation specialist who generates professional PDF, PPTX, DOCX, and XLSX files using code-based approaches with proper formatting, charts, and data visualization. |
| `specialized-french-consulting-market.md` | 🇫🇷 **French Consulting Market Navigator** | Navigate the French ESN/SI freelance ecosystem — margin models, platform mechanics (Malt, collective.work), portage salarial, rate positioning, and payment cycle realities |
| `specialized-korean-business-navigator.md` | 🇰🇷 **Korean Business Navigator** | Korean business culture for foreign professionals — 품의 decision process, nunchi reading, KakaoTalk business etiquette, hierarchy navigation, and relationship-first deal mechanics |
| `specialized-mcp-builder.md` | 🔌 **MCP Builder** | Expert Model Context Protocol developer who designs, builds, and tests MCP servers that extend AI agent capabilities with custom tools, resources, and prompts. |
| `specialized-model-qa.md` | 🔬 **Model QA Specialist** | Independent model QA expert who audits ML and statistical models end-to-end - from documentation review and data reconstruction to replication, calibration testing, interpretability analysis, performance monitoring, and audit-grade reporting. |
| `specialized-salesforce-architect.md` | ☁️ **Salesforce Architect** | Solution architecture for Salesforce platform — multi-cloud design, integration patterns, governor limits, deployment strategy, and data model governance for enterprise-scale orgs |
| `specialized-workflow-architect.md` | \U0001F5FA\uFE0F **Workflow Architect** | Workflow design specialist who maps complete workflow trees for every system, user journey, and agent interaction — covering happy paths, all branch conditions, failure modes, recovery paths, handoff contracts, and observable states to produce build-ready specs that agents can implement against and QA can test against. |

---

### Educacao Internacional
> Planejamento completo de estudos no exterior para estudantes.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `study-abroad-advisor.md` | 🎓 **Study Abroad Advisor** | Full-spectrum study abroad planning expert covering the US, UK, Canada, Australia, Europe, Hong Kong, and Singapore — proficient in undergraduate, master's, and PhD application strategy, school selection, essay coaching, profile enhancement, standardized test planning, visa preparation, and overseas life adaptation, helping Chinese students craft personalized end-to-end study abroad plans. |

---

### Cadeia de Suprimentos
> Gestao estrategica de supply chain e sourcing.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `supply-chain-strategist.md` | 🔗 **Supply Chain Strategist** | Expert supply chain management and procurement strategy specialist — skilled in supplier development, strategic sourcing, quality control, and supply chain digitalization. Grounded in China's manufacturing ecosystem, helps companies build efficient, resilient, and sustainable supply chains. |

---

### Suporte Operacional
> Analytics, resumos executivos, financas, infraestrutura e conformidade legal.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `support-analytics-reporter.md` | 📊 **Analytics Reporter** | Expert data analyst transforming raw data into actionable business insights. Creates dashboards, performs statistical analysis, tracks KPIs, and provides strategic decision support through data visualization and reporting. |
| `support-executive-summary-generator.md` | 📝 **Executive Summary Generator** | Consultant-grade AI specialist trained to think and communicate like a senior strategy consultant. Transforms complex business inputs into concise, actionable executive summaries using McKinsey SCQA, BCG Pyramid Principle, and Bain frameworks for C-suite decision-makers. |
| `support-finance-tracker.md` | 💰 **Finance Tracker** | Expert financial analyst and controller specializing in financial planning, budget management, and business performance analysis. Maintains financial health, optimizes cash flow, and provides strategic financial insights for business growth. |
| `support-infrastructure-maintainer.md` | 🏢 **Infrastructure Maintainer** | Expert infrastructure specialist focused on system reliability, performance optimization, and technical operations management. Maintains robust, scalable infrastructure supporting business operations with security, performance, and cost efficiency. |
| `support-legal-compliance-checker.md` | ⚖️ **Legal Compliance Checker** | Expert legal and compliance specialist ensuring business operations, data handling, and content creation comply with relevant laws, regulations, and industry standards across multiple jurisdictions. |
| `support-support-responder.md` | 💬 **Support Responder** | Expert customer support specialist delivering exceptional customer service, issue resolution, and user experience optimization. Specializes in multi-channel support, proactive customer care, and turning support interactions into positive brand experiences. |

---

### Arte Tecnica
> Pipeline arte-engine: shaders, VFX, LOD e otimizacao de assets.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `technical-artist.md` | 🎨 **Technical Artist** | Art-to-engine pipeline specialist - Masters shaders, VFX systems, LOD pipelines, performance budgeting, and cross-engine asset optimization |

---

### Terminal e Integracao
> Emulacao de terminal e integracao SwiftTerm para apps Swift.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `terminal-integration-specialist.md` | 🖥️ **Terminal Integration Specialist** | Terminal emulation, text rendering optimization, and SwiftTerm integration for modern Swift applications |

---

### Testes e QA
> Testes de acessibilidade, API, performance, E2E e auditoria de qualidade.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `testing-accessibility-auditor.md` | ♿ **Accessibility Auditor** | Expert accessibility specialist who audits interfaces against WCAG standards, tests with assistive technologies, and ensures inclusive design. Defaults to finding barriers — if it's not tested with a screen reader, it's not accessible. |
| `testing-api-tester.md` | 🔌 **API Tester** | Expert API testing specialist focused on comprehensive API validation, performance testing, and quality assurance across all systems and third-party integrations |
| `testing-evidence-collector.md` | 📸 **Evidence Collector** | Screenshot-obsessed, fantasy-allergic QA specialist - Default to finding 3-5 issues, requires visual proof for everything |
| `testing-performance-benchmarker.md` | ⏱️ **Performance Benchmarker** | Expert performance testing and optimization specialist focused on measuring, analyzing, and improving system performance across all applications and infrastructure |
| `testing-reality-checker.md` | 🧐 **Reality Checker** | Stops fantasy approvals, evidence-based certification - Default to "NEEDS WORK", requires overwhelming proof for production readiness |
| `testing-test-results-analyzer.md` | 📋 **Test Results Analyzer** | Expert test analysis specialist focused on comprehensive test result evaluation, quality metrics analysis, and actionable insight generation from testing activities |
| `testing-tool-evaluator.md` | 🔧 **Tool Evaluator** | Expert technology assessment specialist focused on evaluating, testing, and recommending tools, software, and platforms for business use and productivity optimization |
| `testing-workflow-optimizer.md` | ⚡ **Workflow Optimizer** | Expert process improvement specialist focused on analyzing, optimizing, and automating workflows across all business functions for maximum productivity and efficiency |

---

### Engine Unity
> Especialistas Unity: arquitetura, editor tools, multiplayer e Shader Graph.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `unity-architect.md` | 🏛️ **Unity Architect** | Data-driven modularity specialist - Masters ScriptableObjects, decoupled systems, and single-responsibility component design for scalable Unity projects |
| `unity-editor-tool-developer.md` | 🛠️ **Unity Editor Tool Developer** | Unity editor automation specialist - Masters custom EditorWindows, PropertyDrawers, AssetPostprocessors, ScriptedImporters, and pipeline automation that saves teams hours per week |
| `unity-multiplayer-engineer.md` | 🔗 **Unity Multiplayer Engineer** | Networked gameplay specialist - Masters Netcode for GameObjects, Unity Gaming Services (Relay/Lobby), client-server authority, lag compensation, and state synchronization |
| `unity-shader-graph-artist.md` | ✨ **Unity Shader Graph Artist** | Visual effects and material specialist - Masters Unity Shader Graph, HLSL, URP/HDRP rendering pipelines, and custom pass authoring for real-time visual effects |

---

### Engine Unreal
> Especialistas Unreal Engine 5: C++, multiplayer, arte tecnica e mundo aberto.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `unreal-multiplayer-architect.md` | 🌐 **Unreal Multiplayer Architect** | Unreal Engine networking specialist - Masters Actor replication, GameMode/GameState architecture, server-authoritative gameplay, network prediction, and dedicated server setup for UE5 |
| `unreal-systems-engineer.md` | ⚙️ **Unreal Systems Engineer** | Performance and hybrid architecture specialist - Masters C++/Blueprint continuum, Nanite geometry, Lumen GI, and Gameplay Ability System for AAA-grade Unreal Engine projects |
| `unreal-technical-artist.md` | 🎨 **Unreal Technical Artist** | Unreal Engine visual pipeline specialist - Masters the Material Editor, Niagara VFX, Procedural Content Generation, and the art-to-engine pipeline for UE5 projects |
| `unreal-world-builder.md` | 🌍 **Unreal World Builder** | Open-world and environment specialist - Masters UE5 World Partition, Landscape, procedural foliage, HLOD, and large-scale level streaming for seamless open-world experiences |

---

### visionOS e Spatial Computing
> Desenvolvimento nativo visionOS com SwiftUI e design Liquid Glass.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `visionos-spatial-engineer.md` | 🥽 **visionOS Spatial Engineer** | Native visionOS spatial computing, SwiftUI volumetric interfaces, and Liquid Glass design implementation |

---

### XR — Realidade Estendida
> WebXR, interfaces espaciais e cockpit para ambientes AR/VR/XR.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `xr-cockpit-interaction-specialist.md` | 🕹️ **XR Cockpit Interaction Specialist** | Specialist in designing and developing immersive cockpit-based control systems for XR environments |
| `xr-immersive-developer.md` | 🌐 **XR Immersive Developer** | Expert WebXR and immersive technology developer with specialization in browser-based AR/VR/XR applications |
| `xr-interface-architect.md` | 🫧 **XR Interface Architect** | Spatial interaction designer and interface strategist for immersive AR/VR/XR environments |

---

### Zettelkasten — Gestao do Conhecimento
> Gestao de base de conhecimento no estilo Zettelkasten de Niklas Luhmann.

| Arquivo | Agente | Descricao |
|---------|--------|----------|
| `zk-steward.md` | 🗃️ **ZK Steward** | Knowledge-base steward in the spirit of Niklas Luhmann's Zettelkasten. Default perspective: Luhmann; switches to domain experts (Feynman, Munger, Ogilvy, etc.) by task. Enforces atomic notes, connectivity, and validation loops. Use for knowledge-base building, note linking, complex task breakdown, and cross-domain decision support. |

---

## Como Usar

Os agentes sao invocados automaticamente pelo Claude Code quando o contexto e apropriado. Voce tambem pode solicitar explicitamente:

```
Use o agente security-code-reviewer para analisar este codigo
```

Ou ao invocar diretamente via Claude Code:

```
@security-code-reviewer revise este endpoint
```

## Requisitos

- Claude Code CLI
- Modelo: Claude Opus (recomendado para todos os agentes)

## MCPs Recomendados

Para melhor funcionamento dos agentes, recomenda-se configurar:

- **MCP Supabase** - Para operacoes de banco de dados
- **MCP Playwright** - Para testes E2E e validacao de UI
- **MCP Sequential-Thinking** - Para raciocinio complexo
- **MCP Context7** - Para documentacao atualizada de bibliotecas
- **MCP Serena** - Para analise semantica de codigo

## Licenca

MIT

---

Desenvolvido por [Made in Low Code](https://github.com/madeinlowcode)
