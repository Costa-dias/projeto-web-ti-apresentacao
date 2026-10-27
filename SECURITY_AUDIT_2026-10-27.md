# Auditoria de segurança — 27/10/2026

## Atualização: integração e implantação autorizadas em 27/10/2026

Após a auditoria inicial, o proprietário autorizou integrar as correções e realizar o deploy, mantendo o Supabase sem testes enquanto estiver hibernando. Esta seção registra o estado posterior e substitui as pendências de merge/deploy mencionadas no registro inicial abaixo. Os limites de auditoria e de testes não executados continuam válidos.

Commit auditado integrado à `main`: `95efe446e13e237a6da6e266b5623b53ba693e2c`.

Não há aplicação executável deste repositório público para publicar. Documentação e controles de CI foram integrados à `main`; nenhuma aplicação privada vinculada foi alterada.

Nenhuma tabela, política RLS, configuração Supabase, credencial ou dado de usuário foi alterado. O registro abaixo descreve a etapa inicial, anterior à autorização de deploy. Esta atualização é somente documental e usa `[skip render]` para não provocar outro deploy.

---


Repositório: `Costa-dias/projeto-web-ti-apresentacao`. Responsável: Codex. Base auditada: `61325c9bb3803a1aa57b258d9e19a3c6328948ec`.
Branch de trabalho: `security/audit-2026-10-27`. Este relatório acompanha o commit de correção/documentação desta branch; consulte seu SHA no histórico do arquivo.

## Escopo e critérios

Somente conteúdo deste repositório público e histórico alcançável pelas referências obtidas no clone. Nenhum repositório privado foi modificado. Avisos e versões foram consultados em 27/10/2026. Versão antiga, isoladamente, não confirma explorabilidade. Ausência de alerta não garante ausência de vulnerabilidade.

- **CORRIGIDO**: problema confirmado corrigido nesta branch; não implica implantação.
- **SEM IMPACTO**: aviso específico não alcança a versão ou funcionalidade verificada.
- **PENDENTE**: medida necessária ainda não aplicada no ambiente indicado.
- **NÃO VERIFICADO**: faltam código, credenciais, ambiente ou evidência suficiente.

## Histórico e segredos

Gitleaks 8.30.1, regras padrão, `git --log-opts=--all --redact`, sem exceções do repositório na varredura independente: código de saída 0, 0 achados. Escopo: 2 commits alcançáveis (o contador do scanner pode excluir merges/commits sem conteúdo examinável). Não foram detectadas credenciais pelas regras executadas. Objetos apagados, referências não obtidas e segredos sem padrão reconhecível não são cobertos.

## Conteúdo disponível e limitações

Este repositório público contém apresentação/documentação e, quando presentes, metadados de registro. Não contém o código executável, manifestos de dependências, lockfiles, Dockerfile ou workflows da aplicação descrita. As tecnologias citadas no README são declarações, não versões instaladas confirmadas.

**NÃO VERIFICADO**: dependências, CVEs da aplicação, configurações de autenticação/banco, build, inicialização, endpoints e PWA da aplicação real. Não foram acessados repositórios privados para preencher essa lacuna. Não é correto afirmar “SEM IMPACTO” para a aplicação apenas porque não há dependências neste repositório de apresentação.

Testes de aplicação não executados: código e scripts indisponíveis neste repositório. Nenhuma correção de código/dependências foi inventada. O relatório é a única alteração.

## Resultado e integridade operacional

As mudanças desta branch são locais/de revisão. **Nenhum merge, deploy, alteração de credencial, escrita no banco/RLS/autenticação, exclusão ou modificação de produção foi realizado.** Verificações do Render, quando realizadas para FraudLens, foram somente leitura. Produção pode divergir do repositório; não foi declarada integralmente validada.

O diff foi revisado e `git diff --check` passou. Commits são separados por repositório. Para reproduzir a identificação: `git log -1 --format=%H -- SECURITY_AUDIT_2026-10-27.md`.
