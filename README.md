# FluxoLab

Ferramenta web para criar e resolver atividades educacionais de algoritmos com fluxogramas.

## Versão atual

`FluxoLab-Educador_08-11-2026_21-19`, proveniente da entrega **Vidas e Conferir Etapas** do ChatGPT e aprovada pelo usuário para publicação.

Abra `index.html` em um navegador moderno para usar o Educador. Não há instalação ou compilação. Monte a atividade e use **Gerar arquivo do aluno** para escolher o modo Simples ou Desafio e produzir um HTML com os dados da atividade.

- `index.html`: Educador da versão atual.
- `student-template.html`: modelo do Aluno, com marcador de dados; não deve ser aberto como atividade pronta.
- `FluxoLab-Educador_08-11-2026_21-19/`: cópia versionada dos dois HTML, com nomes no padrão acordado.
- `CONTEXTO_FLUXOLAB.md`: origem, fluxo de trabalho, verificações e pendências para continuidade do desenvolvimento.

## Recursos

Editor de blocos e conexões, importação/exportação JSON, rascunho local, desfazer/refazer, modos Simples e Desafio, biblioteca com ordenação alfanumérica e índices fixos, cinco vidas e conferência parcial de etapas.

## Estado de validação

Sintaxe JavaScript verificada e modelo do Aluno sincronizado com a cópia embutida no Educador. Testes visuais e funcionais no navegador ainda pendentes. As conferências comparam origem e destino das conexões, sem comparar os rótulos Verdadeiro/Falso.

## Versionamento

Cada atualização usa pasta `FluxoLab-Educador_dd-MM-aaaa_hh-mm` com os HTML Educador e Aluno no mesmo timestamp, no fuso America/Sao_Paulo. Publicações no GitHub dependem de confirmação do usuário. O histórico Git preserva as versões anteriores dos arquivos da raiz.
