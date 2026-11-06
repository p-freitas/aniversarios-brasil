# Quão comum é o seu aniversário no Brasil?

Um calendário interativo com as **366 datas** ordenadas pela frequência entre **76.691.580 nascimentos com data válida** registrados no SINASC entre **1997 e 2022**.

## Como abrir

Abra [`index.html`](index.html) no GitHub, clique no botão de download e abra o arquivo baixado no navegador. O calendário funciona offline. Clique em uma data para ver a contagem e alterne entre o total acumulado e a média por ocorrência da data.

## O que os dados mostram

- **10 de março** foi a data mais frequente, com **234.249 nascimentos**.
- **29 de fevereiro** ficou em 366º lugar pelo total acumulado. Dividindo os nascimentos dessa data pelas seis vezes em que ela ocorreu no período, fica em **310º**.
- **25 de dezembro** teve a menor média por ocorrência: cerca de **5.591 nascimentos**.

## Dados e metodologia

- [`aniversarios-brasil.csv`](aniversarios-brasil.csv): total, média e posição nos dois rankings para cada combinação de dia e mês.
- [`nascimentos-por-data-1997-2022.csv`](nascimentos-por-data-1997-2022.csv): contagens nacionais por data completa. Os CSVs usam ponto e vírgula como separador.

O cálculo agrupa os registros pela data de nascimento (`DTNASC`). Dos 76.691.677 registros lidos, 97 foram excluídos por data inválida. A média usa 26 ocorrências por data, ou 6 para 29 de fevereiro. O recorte descreve nascimentos registrados no período; a distribuição dos aniversários da população brasileira viva pode ser diferente.

A fonte é o [SINASC, do Ministério da Saúde](https://dadosabertos.saude.gov.br/dataset/sistema-de-informacao-sobre-nascidos-vivos-sinasc). As contagens foram calculadas a partir da [cópia documentada em Parquet do projeto healthbr-data](https://huggingface.co/datasets/SidneyBissoli/sinasc), com 702 arquivos das 27 unidades da federação. O HTML inclui mais detalhes, a conferência anual e referências às pesquisas brasileiras consultadas.
