# FluxoLab — base atual de desenvolvimento

Contexto atualizado em 08/11/2026 às 21:19 (America/Sao_Paulo).

## Fluxo de trabalho acordado

1. Cada atualização deve ser entregue em uma pasta `FluxoLab-Educador_dd-MM-aaaa_hh-mm`, contendo `FluxoLab-Educador_dd-MM-aaaa_hh-mm.html` e `FluxoLab-Aluno_dd-MM-aaaa_hh-mm.html`. Usar a data e hora reais da atualização no fuso America/Sao_Paulo, com o mesmo timestamp na pasta e nos dois arquivos. Preservar versões anteriores; não sobrescrever silenciosamente uma pasta existente.
2. Em cada resposta de entrega após uma atualização local, perguntar ao usuário se deseja fazer o commit e atualizar o repositório GitHub `lucasmmps/FluxoLab`. Somente realizar essas alterações no GitHub após confirmação explícita para a atualização em questão. A aprovação de uma atualização não autoriza automaticamente publicações futuras.
3. Atualizar este contexto sempre que necessário ou solicitado, registrando a versão vigente, alterações, verificações, pendências e estado de publicação, para permitir migração entre ferramentas de IA.
4. Manter o modelo do aluno separado e sua cópia embutida no Educador sincronizados.

## Versão local vigente

Pasta: `FluxoLab-Educador_08-11-2026_21-19/`.

- Educador: `FluxoLab-Educador_08-11-2026_21-19.html`.
- Aluno: `FluxoLab-Aluno_08-11-2026_21-19.html`.

Esta primeira entrega no padrão acordado é uma cópia byte a byte dos HTML do ZIP fornecido pelo usuário, sem mudanças funcionais. Os hashes continuam iguais aos registrados abaixo. A pasta original foi preservada. Publicação no GitHub autorizada pelo usuário: esta entrega inclui a pasta versionada e este contexto na branch `main` de `lucasmmps/FluxoLab`. Os arquivos `index.html` e `student-template.html` da raiz acompanham a versão vigente, mantendo o ponto de entrada do projeto atualizado.

## Fonte de verdade

O usuário forneceu o arquivo `FluxoLab_Vidas_Conferir_Etapas.zip`, produzido na última resposta da conversa ChatGPT “Ferramenta para fluxogramas puzzle” (6ab32e76-f11c-83e9-bff0-1c4a1b5c9e28). Esta entrega substitui a versão de 21/10/2026 do GitHub como base para continuar o desenvolvimento.

Origem: `C:/Users/lucas/TI/Associação Arcanjo Rafael/FluxoLab/FluxoLab_Vidas_Conferir_Etapas.zip`.

Os HTML foram extraídos sem modificações para `FluxoLab_Vidas_Conferir_Etapas/`:

- `FluxoLab_Educador_Vidas_Conferir_Etapas.html`: editor e gerador de atividades; arquivo a abrir para usar o projeto.
- `FluxoLab_Aluno_Vidas_Conferir_Etapas.html`: modelo do aluno, com marcador `__FLUXOLAB_DATA__`; precisa receber dados via geração pelo Educador, não é uma atividade autônoma preenchida.

## Recursos confirmados no código

- Editor de fluxogramas com início, processo, entrada, saída, decisão e fim; conexões, edição, desfazer/refazer, importação/exportação JSON e rascunho local.
- Geração de HTML para aluno em modo Simples (peças no quadro) ou Desafio (peças na biblioteca).
- Biblioteca ordenada por categoria: Início, Processo, Entrada, Saída, Decisão, Fim; ordenação alfanumérica pt-BR dentro de cada categoria.
- Índices fixos e exclusivos, calculados a partir da ordenação inicial, em círculos externos aos blocos da biblioteca. Não aparecem nos blocos do quadro; peças devolvidas mantêm o índice.
- Cinco vidas, corações e botão Conferir Etapas; erro destaca um bloco e consome uma vida; ao chegar a zero o botão é desabilitado.
- Conferir Resposta continua separado da conferência parcial.

## Comportamento da conferência parcial

O código percorre as conexões a partir dos blocos de Início, procura conexões ausentes no gabarito e verifica componentes conectados que não foram alcançados pelo percurso. Peças soltas sem conexões não são consideradas erros nessa etapa. Portanto, a implementação é mais específica do que a descrição resumida da resposta anterior do ChatGPT.

As duas conferências comparam origem e destino; os rótulos Verdadeiro/Falso não participam da comparação. Isso é uma limitação existente, ainda não corrigida.

## Verificação desta importação

- Sintaxe dos scripts dos dois HTML validada com Node.js (`vm.Script`, sem executar o aplicativo).
- Modelo do aluno embutido em Base64 no Educador é textualmente idêntico ao HTML do Aluno fornecido.
- Nenhuma mudança funcional nesta entrega; publicação da versão importada autorizada pelo usuário após a conferência local.
- Testes visuais e funcionais no navegador ainda pendentes, especialmente decisões, ramificações e reinício das vidas.

SHA-256 dos arquivos originais extraídos:

- Aluno: `E7DD86F3FB886FA47822C4DBB0EA569E346DA1C9E53E633B6B332C947DC34BB0`
- Educador: `8F1056C45A0FECA8F7E66839BB1FA39FC939D222A9F86B78218E785EDFD24B55`

Ao alterar a interface do aluno, manter o HTML separado e sua cópia embutida no Educador sincronizados. Preservar esta referência de origem; mudanças futuras devem ser identificadas como novas versões.
