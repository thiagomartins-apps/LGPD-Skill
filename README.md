
# Antigravity LGPD Compliance Skill 🛡️🤖

Uma Skill inteligente e interativa para o ecossistema de agentes **Antigravity**, projetada para auditar código-fonte, arquitetura de software e bancos de dados com foco total na **Lei Geral de Proteção de Dados (LGPD - Lei nº 13.709/2018)**.

Esta Skill utiliza como base de conhecimento o **Guia de Proteção de Dados Pessoais do Ministério da Ciência, Tecnologia e Inovação (MCTI)**.

---

## 🚀 Funcionalidades

	🔍 **Varredura Automatizada (Scanner):** Identifica a manipulação de Dados Pessoais Comuns e Sensíveis (como CPF, e-mails, dados biométricos) direto nos arquivos do projeto.
	🛡️ **Análise de Vulnerabilidades:** Detecta falhas contra o *Princípio da Segurança* (como logs expondo dados em texto limpo ou falta de criptografia).
	🤝 **Fluxo 100% Assistido:** A IA elabora um plano de correção por etapas e **solicita a sua aprovação explícita** antes de efetuar qualquer alteração no código.
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
Com a Skill instalada, você pode interagir diretamente com o seu agente através do chat ou terminal.

1. **Iniciar a Varredura do Projeto**
Para começar a auditoria em uma pasta específica do seu projeto, digite:

@nome-do-agente varrer projeto na pasta ./src

2. **Fluxo Assistido (Aprovação por Etapas)**
O agente listará as falhas encontradas uma por uma e aguardará o seu comando.

Para aceitar a alteração sugerida pela IA, digite: [Aprovar] ou Sim.

Para ignorar o ponto apontado, digite: [Recusar] ou Não.

3. **Visualizar o Relatório Final**
Após a conclusão das etapas, a Skill gerará automaticamente um arquivo chamado relatorio_lgpd.html na raiz do projeto analisado. Basta abri-lo em qualquer navegador para visualizar o painel de conformidade e a governança dos dados.

## 🗺️ Roadmap de Evolução
Estamos trabalhando para tornar esta Skill ainda mais completa. Sinta-se à vontade para abrir uma Issue ou enviar um Pull Request para ajudar a desenvolver as seguintes melhorias mapeadas:

	-	🐳 Segurança em DevOps & CI/CD: Implementar varredura em arquivos de configuração de infraestrutura (como Dockerfile, workflows do GitHub Actions e scripts do Terraform) para identificar variáveis de ambiente e chaves privadas expostas antes do deploy.

	-	🌍 Suporte a Múltiplas Legislações (Internacionalização): Modularizar o motor da Skill para permitir a validação de regras de outros territórios (como a GDPR europeia) através de parâmetros específicos (ex: --regra=gdpr).

## 📝 Licença e Créditos
Desenvolvido por: Thiago Martins

Base de Conhecimento: Resumo técnico estruturado a partir do Guia Oficial de Proteção de Dados Pessoais — MCTI (1ª Edição - 2025).

Este projeto é livre para reprodução e modificação para fins não comerciais, desde que citada a fonte (Copyleft MCTI).