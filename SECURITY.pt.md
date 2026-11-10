# Reporte de segurança

[English](SECURITY.md) | [Português](SECURITY.pt.md) | [Español](SECURITY.es.md)

Siga as instruções de segurança próprias do repositório de destino, quando existirem. Bugs funcionais comuns devem usar o formulário de issue **Bug report**. Suspeitas de vulnerabilidade não devem ser divulgadas em issues, discussões ou pull requests públicos.

Os CODEOWNERS relevantes são responsáveis por acompanhar, triar e coordenar a resolução dos relatos de segurança dos componentes sob sua responsabilidade, tanto pelo PVR dos repositórios públicos quanto pelo email interno dos privados. Os mantenedores configuram as permissões e notificações necessárias; a atribuição em CODEOWNERS não configura sozinha o recebimento no GitHub.

## Repositórios públicos

Use **Security and quality → Report a vulnerability** no repositório público afetado quando o Private Vulnerability Reporting estiver habilitado. Envie versão afetada, resumo, reprodução segura e impacto nesse formulário privado. Os relatos podem ser escritos em inglês, português ou espanhol. Não inclua segredos, dados de clientes ou anexos sensíveis desnecessários.

A organização fornece um padrão `.github/VULNERABILITY_REPORT.yml`; o formulário próprio do repositório tem prioridade. Um template não habilita o recurso nem comprova que responsáveis o acompanham. Se a opção privada estiver ausente ou indisponível, solicite instruções de reporte privado a um mantenedor sem revelar a vulnerabilidade. Não substitua essa rota por uma issue comum com detalhes de segurança.

## Repositórios privados

Envie email aos **CODEOWNERS** relevantes pelos canais internos já existentes da Versat. Identifique os responsáveis pelos caminhos afetados no arquivo CODEOWNERS do repositório e obtenha os emails no diretório interno ou por um contato interno estabelecido. Não deduza emails a partir dos nomes de usuário do GitHub nem publique contatos internos.

Se faltar CODEOWNERS, houver dúvida sobre responsabilidade ou você não tiver acesso aos contatos internos, solicite instruções privadas ao mantenedor do repositório ou ao seu contato existente na Versat, sem revelar detalhes sensíveis. Uma issue em repositório privado não substitui essa rota: seu público pode ser maior que o dos destinatários previstos.

## Recebimento e escopo

Esta política não concede acesso a repositórios privados nem permissão para realizar testes. Não promete prazo de resposta ou monitoramento contínuo. Os mantenedores devem estabelecer destinatários permitidos, notificações e recebimento real antes de afirmar que a rota foi verificada. Mantenha os detalhes privados durante a coordenação da correção.
