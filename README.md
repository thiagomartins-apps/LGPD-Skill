# Antigravity LGPD & GDPR Compliance Skill 🛡️🤖

Uma Skill inteligente e interativa para o ecossistema de agentes **Antigravity**, projetada para auditar código-fonte, arquitetura de software, bancos de dados e infraestrutura de CI/CD com foco em conformidade regulatória internacional (**LGPD** e **GDPR**).

Esta Skill utiliza como bases de conhecimento o **Guia de Proteção de Dados Pessoais do Ministério da Ciência, Tecnologia e Inovação (MCTI)** e o **Regulamento Geral sobre a Proteção de Dados da União Europeia (Regulamento UE 2016/679)**.

---

## 🚀 Funcionalidades

	🔍 **Varredura Automatizada (Scanner):** Identifica a manipulação de Dados Pessoais Comuns e Sensíveis (como CPF, e-mails, dados biométricos) direto nos arquivos do projeto.
	🐳 **Auditoria de DevOps & CI/CD:** Detecta chaves privadas, tokens e senhas expostas (*hardcoded*) em arquivos de infraestrutura (como `Dockerfile`, `docker-compose.yml` e workflows do GitHub Actions).
	🛡️ **Análise de Vulnerabilidades:** Detecta falhas contra os princípios de segurança e confidencialidade (como logs expondo dados em texto limpo ou falta de criptografia).
	🤝 **Fluxo 100% Assistido:** A IA elabora um plano de correção por etapas e **solicita a sua aprovação explícita** antes de efetuar qualquer alteração nos arquivos locais.
	🌍 **Suporte Multilegislação:** Permite chavear o motor de análise para validar tanto as regras brasileiras (LGPD) quanto as diretrizes europeias (GDPR).
	📊 **Relatório em HTML Didático:** Ao fim das correções, gera um relatório visual completo estruturado com base no Ciclo de Vida do Tratamento de Dados (Coleta, Retenção, Processamento, Compartilhamento e Eliminação).

---

## 📦 Instalação

Como o Antigravity utiliza arquivos Markdown nativos para registrar novas habilidades, a instalação é extremamente simples:

	1. Baixe o arquivo `lgpd_skill.md` deste repositório.
	2. Mova o arquivo para o diretório de configurações de Skills do seu agente Antigravity:
		`bash
		`meu-agente/skills/
	3. Reinicie ou recarregue o seu agente. Pronto! A Skill já estará ativa e integrada à memória do auditor.

## 🛠️ Como Usar
Com a Skill instalada, você pode interagir diretamente com o seu agente através do chat ou terminal de comandos.

	1. **Iniciar a Varredura Padrão (LGPD)**
Para começar a auditoria em uma pasta específica do seu projeto utilizando a legislação brasileira como base, digite:

		@nome-do-agente varrer_projeto_LGPD_GDPR na pasta ./src

	2. **Iniciar a Varredura Internacional (GDPR)**
Para chavear a persona e as citações técnico-legais para o regulamento europeu, utilize a flag --regra=gdpr:

		@nome-do-agente varrer_projeto_LGPD_GDPR na pasta ./src --regra=gdpr

	3. **Fluxo Assistido (Aprovação por Etapas)**
O agente listará as falhas encontradas uma por uma e aguardará o seu comando no chat.

	Para aceitar a alteração sugerida pela IA, digite: [Aprovar] ou Sim.

	Para ignorar o ponto apontado, digite: [Recusar] ou Não.

	4. **Visualizar o Relatório Final**
Após a conclusão das etapas, a Skill invocará a API do sistema para gerar automaticamente um arquivo chamado relatorio_lgpd.html ou relatorio_gdpr.html na raiz do seu projeto. Basta abri-lo em qualquer navegador para visualizar o painel de conformidade.

## 📝 Licença e Créditos
**Desenvolvido por:** Thiago Martins

**Bases de Conhecimento:** Resumo técnico estruturado a partir do Guia Oficial de Proteção de Dados Pessoais — MCTI (1ª Edição)  e das diretrizes do Regulamento Europeu UE 2016/679.  

Este projeto é livre para reprodução e modificação para fins não comerciais, desde que citada a fonte (Copyleft MCTI).