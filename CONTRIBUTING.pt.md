# Contribuir com a Versat Labs

[English](CONTRIBUTING.md) | [Português](CONTRIBUTING.pt.md) | [Español](CONTRIBUTING.es.md)

Quem desenvolve, projeta arquitetura, faz design ou contribui de outras formas pode ajudar a planejar ou implementar uma issue existente, propor uma nova ou melhorar a qualidade. Escolha o repositório, leia seu README, AGENTS.md e orientações disponíveis. O CONTRIBUTING.md próprio do repositório tem precedência sobre estes padrões da organização.

## Começar uma contribuição

Abra **Issues → New issue** no repositório alvo e use o formulário disponível de bug, funcionalidade ou manutenção. Descreva problema, contexto e resultado esperado; inclua reprodução para bugs. É possível contribuir com uma issue bem definida sem implementá-la. Antes de trabalhar nos arquivos, siga preparação, especificações e validação do repositório. No PR, vincule a issue, explique a mudança e informe verificações reais e validações indisponíveis.

## Instalar o plugin Versat AI Harness

O plugin `versat-ai-harness` fornece Skills reutilizáveis e orientações para planejar, implementar e validar contribuições com o Codex. Siga o caminho de instalação correspondente à sua conta. Os nomes dos menus abaixo estão em inglês.

### Membros do workspace da Versat

1. No Codex, selecione o workspace da Versat e abra **Settings > Plugins > Browse Directory > Versat**.
2. Abra **Versat-ai-harness** e selecione **Install**.

A administração do workspace gerencia a distribuição. Se o plugin não aparecer ou a instalação estiver indisponível, procure o administrador do workspace.

### Colaboradores externos

Se sua conta no Codex não faz parte do workspace da Versat:

1. Abra **Settings > Plugins > Add > Add Marketplace**.
2. Em **Source**, informe a URL do repositório do Harness: [https://github.com/versat-labs/versat-ai-harness](https://github.com/versat-labs/versat-ai-harness).
3. Confirme a adição do marketplace. No marketplace **Versat Plugins** adicionado, encontre `versat-ai-harness` e selecione **Install**. Adicionar o marketplace e instalar o plugin são etapas separadas.

**Atualize manualmente a cada nova versão.** Leia as instruções da versão e confira a compatibilidade com seu projeto, atualize o marketplace adicionado e atualize o plugin instalado usando os controles disponíveis na sua versão do Codex. Confirme a versão instalada em um novo chat antes de continuar; atualizar apenas o catálogo não confirma a atualização do plugin. Se a versão selecionada estiver indisponível ou a atualização falhar, procure os mantenedores do Harness antes de continuar com essa versão.

O repositório do Harness é público. O acesso ao repositório em que você deseja contribuir é separado da instalação do plugin.

## Começar a usar o plugin

1. Clone ou abra o repositório alvo como projeto no Codex. Leia seu README, AGENTS.md e orientações de contribuição.
2. Inicie um novo chat após instalar ou atualizar o plugin e peça ao Codex para verificar a preparação:

   ```text
   Confirme a pasta atual do projeto, a versão instalada do versat-ai-harness e onde encontrou a Skill versat-sdd e seus recursos canônicos correspondentes. Informe qualquer pré-requisito ausente antes de alterar arquivos.
   ```

3. Com a preparação confirmada, use uma issue real para solicitar o planejamento inicial. Substitua os campos abaixo:

   ```text
   Use $versat-sdd para planejar a mudança <change-name> da issue <issue-url>: <descreva o problema e o resultado esperado>. Crie somente Proposal e Requirements; não implemente. Pare para revisão do Gate 1.
   ```

Espere os arquivos `specs/changes/<change-name>/proposal.md` e `requirements.md`, escritos em inglês. Revise-os antes de aprovar a próxima etapa. Design e Tasks seguem seus respectivos gates de aprovação; a implementação requer um pedido explícito após a revisão de Tasks. Se a Skill ou seus recursos estiverem ausentes, resolva a instalação com o administrador do workspace ou os mantenedores do Harness antes de continuar.

## Guias do Harness

Estes links apontam para a documentação mantida do Harness em `main`; siga a documentação correspondente à versão instalada ao trabalhar em um projeto versionado. Você também pode propor uma issue pela entrada pública de contribuição sem instalar o plugin.

- [Primeiro uso](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/quickstart.pt.md)
- [Preparar o ambiente](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/workspace-setup.pt.md)
- [SDD e aprovações](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/sdd-with-codex.pt.md)
- [Entrega pelo GitHub](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/github-delivery.pt.md)
- [Validação](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/validation-and-evaluations.pt.md)
- [Política canônica de idiomas (inglês)](https://github.com/versat-labs/versat-ai-harness/blob/main/standards/core/language.md)

## Direitos e procedência

Antes de propor código, texto ou recursos, identifique a origem, as permissões aplicáveis e os avisos exigidos. Se não conseguir comprovar a permissão para contribuir com uma ilustração, retire-a e consulte o responsável pelo repositório; uma issue ou revisão técnica não supre direitos ausentes. Siga os termos efetivos do repositório de destino. A permissão para usar uma ferramenta interna de desenvolvimento é distinta da licença do projeto de destino, e instalar essa ferramenta não é requisito para a contribuição pública descrita acima. Esta orientação não introduz CLA, DCO ou cessão de direitos.

## Relatos de segurança

Para bugs comuns, use Bug report. Para suspeitas de vulnerabilidade em repositórios públicos, use o Private Vulnerability Reporting do GitHub quando habilitado. Nos privados, envie email aos CODEOWNERS relevantes pelos canais internos existentes da Versat. Não divulgue detalhes de vulnerabilidade em issues comuns. Consulte [reporte de segurança](SECURITY.pt.md) para encaminhamento e recuperação quando o canal estiver indisponível.
