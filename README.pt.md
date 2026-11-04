# Versat Labs · Padrões da organização

[English](README.md) | [Português](README.pt.md) | [Español](README.es.md)

O inglês é a fonte canônica deste README. As traduções em português e espanhol são mantidas em conjunto com ela, seguindo a convenção de idiomas do Versat AI Harness para documentação voltada à comunidade.

## Objetivo

O `versat-labs/.github` é mantido pela Versat Labs para centralizar o perfil público da organização, as diretrizes padrão de contribuição e os templates de issues. Ele segue a convenção do GitHub para o repositório especial `.github`, permitindo que os repositórios da organização compartilhem recursos consistentes para contribuições.

Este repositório contém metadados da organização e documentação. Não possui aplicação executável, processo de build ou suíte de testes automatizados.

## Como o GitHub usa este repositório

- O GitHub exibe `profile/README.md` no perfil público da organização. Consulte a [documentação sobre o perfil da organização](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile).
- O `CONTRIBUTING.md` fornece orientações padrão quando um repositório não possui seu próprio guia de contribuição.
- A pasta `.github/ISSUE_TEMPLATE/` fornece os formulários padrão de issues. Templates válidos ou uma configuração de templates próprios de um repositório substituem toda a pasta padrão.
- O GitHub referencia esses padrões sem copiá-los para os repositórios que os utilizam. Consulte a [documentação sobre arquivos padrão da comunidade](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

O `AGENTS.md` e o `.gitignore` se aplicam a este repositório; o GitHub não os distribui como padrões da organização.

## Guia dos arquivos

| Arquivo | Finalidade |
| --- | --- |
| [README.md](README.md) | Visão geral canônica em inglês deste repositório, de seus arquivos e do fluxo de manutenção. |
| [README.pt.md](README.pt.md) | Tradução desta visão geral para o português. |
| [README.es.md](README.es.md) | Tradução desta visão geral para o espanhol. |
| [profile/README.md](profile/README.md) | Perfil público da organização: missão, visão, áreas de atuação, formas de contribuir e recursos úteis da Versat Labs. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Guia padrão de contribuição: formas de participar, configuração local, desenvolvimento orientado por especificações (SDD), etapas de aprovação humana, validação, pull requests e convenções de idioma. |
| [AGENTS.md](AGENTS.md) | Instruções para agentes que trabalham neste repositório, incluindo escopo, convenções de edição e requisitos de validação. |
| [.gitignore](.gitignore) | Exclui do controle de versão arquivos de ambiente local, configurações de editores, logs e artefatos gerados; permite `.env.example`. Esses padrões não indicam a existência de ferramentas de build neste repositório. |
| [.github/ISSUE_TEMPLATE/bug_report.yaml](.github/ISSUE_TEMPLATE/bug_report.yaml) | Formulário de relato de bugs. Exige descrição, passos para reprodução e comportamento esperado; também oferece campos para capturas de tela, detalhes dos dispositivos e contexto adicional. Usa o prefixo de título `fix: ` e o tipo de issue `Bug`. |
| [.github/ISSUE_TEMPLATE/chore.yaml](.github/ISSUE_TEMPLATE/chore.yaml) | Formulário de manutenção. Exige descrição, escopo e critérios de conclusão. Usa o prefixo de título `chore: ` e o tipo de issue `Task`. |
| [.github/ISSUE_TEMPLATE/feature_request.yaml](.github/ISSUE_TEMPLATE/feature_request.yaml) | Formulário de solicitação de funcionalidades. Exige o problema, o trabalho a ser realizado e as personas de usuário e comprador, com contexto adicional opcional. Usa o prefixo de título `feat: ` e o tipo de issue `Feature`. |

Os três formulários declaram `versat-labs/1` no metadado `projects`.

## Como usar os recursos de contribuição

Abra o repositório para o qual deseja contribuir, leia suas orientações de contribuição e selecione **Issues → New issue**. Quando os padrões da organização se aplicarem, escolha o formulário de bug, funcionalidade ou manutenção, preencha os campos obrigatórios e envie. A issue resultante reúne as informações necessárias para iniciar o planejamento. As orientações específicas do repositório têm precedência.

## Manutenção deste repositório

Leia [CONTRIBUTING.md](CONTRIBUTING.md) e [AGENTS.md](AGENTS.md) antes de editar. Mantenha as três versões do README alinhadas sempre que seu conteúdo mudar.

Mudanças substanciais em processos ou políticas seguem o ciclo de SDD documentado:

`Issue → Proposta e requisitos → Design → Tarefas → Implementação → Validação → Pull request`

Proposta e requisitos, Design e Tarefas exigem aprovação humana em cada etapa antes da implementação. Edições rotineiras de documentação e manutenção de formulários recebem revisão proporcional. Alterações no perfil são públicas, e alterações nos padrões podem afetar vários repositórios.

### Validação

Comece pelos requisitos de validação do [AGENTS.md](AGENTS.md):

1. Revise o diff e execute `git diff --check`.
2. Para Markdown, verifique títulos, formatação, links e alinhamento das traduções. Visualize o conteúdo público quando o layout for relevante.
3. Para formulários de issues alterados, analise o YAML e verifique as chaves obrigatórias, a unicidade dos IDs dos campos, as marcações de obrigatoriedade, os prefixos dos títulos, os tipos de issue e os metadados de projeto. Confira o formulário no GitHub quando o comportamento não puder ser verificado localmente.
4. Informe no pull request as alterações, as verificações concluídas e qualquer validação que não tenha sido possível realizar.
