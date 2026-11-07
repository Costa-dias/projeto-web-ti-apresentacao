# Assistente de TI — apresentação profissional

**Versão documentada: 3.2.0 · revisão da documentação em 07/11/2026**

Aplicação privada desenvolvida para organizar atendimentos de TI, consultar soluções anteriores e manter uma biblioteca técnica. Esta apresentação não oferece acesso à aplicação nem divulga código privado ou registros reais.

## Como funciona

- **Ordens de serviço:** cadastro rápido, continuação e edição, conclusão validada e histórico de alterações. Novos registros vão para OS Geral, inclusive com datas retroativas; os antigos permanecem na origem.
- **Dashboard:** totais, conclusão, evolução mensal, categorias estimadas e unidades/setores. Variações de maiúsculas são agrupadas na exibição, preservando a planilha original. A área Registros para revisar permite conferir datas inválidas e unidades não informadas.
- **Recorrências:** agrupamentos por local e tipo de equipamento, com causas registradas e limites explícitos quando faltam informações.
- **Base de Conhecimento:** comandos Windows, procedimentos, casos atípicos e artigos pessoais. Filtros por sistema, favoritos e vínculo com a OS de origem. Artigos pessoais e favoritos sincronizam em uma aba separada do Google Sheets.
- **Gemini opcional:** contexto passa por revisão de privacidade antes de qualquer envio; a biblioteca não é enviada automaticamente.
- **Acesso privado:** Google OAuth, sessão por inatividade, gerenciamento de dispositivos e controle explícito de navegador confiável. A autenticação adicional é decidida pelo Google.

## Minha participação

Identifiquei necessidades da minha rotina de suporte, defini campos e fluxos e validei o uso. O desenvolvimento utiliza apoio de IA, com revisão e ajustes a partir dos testes. A apresentação pública não divulga dados internos nem atribui resultados operacionais não medidos.

## Tecnologias e decisões

React, TypeScript e CSS no frontend; Node.js e Express no backend. Google OAuth e Google Sheets para autenticação e dados; Gemini sob demanda. Hospedagem no Render e versionamento no GitHub.

A planilha continua como armazenamento principal. Os indicadores são derivados dos registros existentes, sem reescrever automaticamente textos ou completar campos desconhecidos. Categorias e identificação de sistemas são estimativas, não métricas de diagnóstico homologadas.

## Exemplo fictício

Uma OS de impressora pode ser registrada rapidamente e complementada após os testes. O dashboard apresenta seu estado; um procedimento incomum pode originar um rascunho de artigo, revisado antes de integrar a biblioteca. Este exemplo não representa um chamado real.

## Privacidade e limites

Código-fonte, credenciais, configurações privadas e dados operacionais permanecem no ambiente privado. Não são fornecidos pacientes, usuários, chamados reais ou acesso ao sistema. O portfólio apresenta uma captura real do formulário vazio, sem dados pessoais ou relatos de atendimentos. A demonstração interativa usa dados fictícios.

A versão documentada descreve a revisão de código; a versão em produção deve ser conferida no rodapé da aplicação. Testes locais e simulações não comprovam disponibilidade contínua das integrações externas.

[Notas da evolução](RELEASES.md).
