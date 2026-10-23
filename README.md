# Normas ambientais de SP

Acervo de normas ambientais do Estado de São Paulo em texto pesquisável (Markdown), com o PDF original ao lado e link para a fonte oficial. Complementa o repositório [ctresb/leis](https://github.com/ctresb/leis), que não cobre atos da CETESB nem da SEMIL.

Mantido por Eduardo Rodrigo Viana Mallet — VM Ambiental - Consultoria Ambiental e Engenharia.

> [!IMPORTANT]
> Conteúdo de caráter informativo, obtido por conversão automática (e OCR, nos documentos escaneados). **Não substitui a publicação oficial.** Confira sempre o PDF e o link `fonte` de cada arquivo antes de citar.

## Conteúdo

| Pasta | O que é | Situação |
|---|---|---|
| [`dds-cetesb/`](dds-cetesb/INDICE.md) | Decisões de Diretoria da CETESB, 2012–2026 | 234 DDs (15 por OCR), inventário de 22/10/2026 |
| [`resolucoes/`](resolucoes/INDICE.md) | Resoluções SEMIL, SIMA e SMA | 1.181 vigentes com texto integral; índice das 2.627 (inclui revogadas, com a norma revogadora), coleta de 23/10/2026 |

## Estrutura

```
dds-cetesb/
  INDICE.md            tabela navegável (DD, data, ementa, links)
  indice.csv           mesma tabela para planilha ou script
  texto/AAAA/*.md      texto integral, com cabeçalho YAML (número, data, ementa, fonte, método de conversão)
  pdf/AAAA/*.pdf       PDF original baixado do site da CETESB
resolucoes/
  INDICE.md            vigentes por tipo (SEMIL, SIMA, SMA) com links; totais de revogadas
  indice.csv           todas as 2.627 normas: status, situação, revogada_por, data, links
  semil|sima|sma/
    texto/AAAA/*.md    texto integral das vigentes, com cabeçalho YAML
    pdf/AAAA/*.pdf     PDF original (e anexos, quando há)
```

Nas resoluções, o nome do arquivo é o mesmo endereço da norma no site da SEMIL (ex.: `resolucao-sima-080-20`). A situação (vigente/revogada e por qual norma) é a informada pelo site; a data vem do próprio documento.

Nomes de arquivo: `DD-NNN-AAAA-SIGLAS` (ex.: `DD-038-2017-C`). Quando o inventário traz a mesma DD mais de uma vez (original, atualizada, consolidada), as demais recebem `-v2`, `-v3`; o campo `titulo_no_site` diz qual é qual.

Data e siglas seguem o próprio documento. Onde o inventário do site diverge (data de publicação no lugar da data da DD, ou sigla de diretoria errada — 8 casos), a forma do site fica registrada no cabeçalho (`diretorias_no_site`, `titulo_no_site`).

## Limitações

- O inventário publicado no site da CETESB **não contém todas as DDs** — a numeração anual passa de 300, mas o site lista só uma seleção. Ausência aqui não significa que a DD não existe.
- Textos por OCR (marcados com ⚠️ no índice e com aviso no próprio arquivo) podem ter erros de reconhecimento, sobretudo em tabelas e anexos.
- Fonte do inventário: https://www.cetesb.sp.gov.br/cetesb/institucional/diretoria/decisoes_de_diretoria
- Resoluções: a situação vigente/revogada é a publicada pelo site da SEMIL, que pode estar desatualizada; normas posteriores que alterem ou revoguem uma resolução devem ser conferidas no texto. Algumas normas de 2019–2020 aparecem no site como SMA sendo SIMA no documento (e vice-versa), por causa da troca de nome da secretaria. 44 vigentes ficaram sem data por erro de digitação no próprio documento ou por não trazerem data no cabeçalho.
- Fonte das resoluções: https://semil.sp.gov.br/legislacao/ (listagem e API do site).
