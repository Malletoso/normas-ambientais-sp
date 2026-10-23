# Normas ambientais de SP

Acervo de normas ambientais do Estado de São Paulo em texto pesquisável (Markdown), com o PDF original ao lado e link para a fonte oficial. Complementa o repositório [ctresb/leis](https://github.com/ctresb/leis), que não cobre atos da CETESB nem da SEMIL.

Mantido por Eduardo Rodrigo Viana Mallet — VM Ambiental - Consultoria Ambiental e Engenharia.

> [!IMPORTANT]
> Conteúdo de caráter informativo, obtido por conversão automática (e OCR, nos documentos escaneados). **Não substitui a publicação oficial.** Confira sempre o PDF e o link `fonte` de cada arquivo antes de citar.

## Conteúdo

| Pasta | O que é | Situação |
|---|---|---|
| [`dds-cetesb/`](dds-cetesb/INDICE.md) | Decisões de Diretoria da CETESB, 2012–2026 | 234 DDs (15 por OCR), inventário de 22/10/2026 |
| `semil/` | Resoluções SMA/SIMA/SEMIL | a fazer |

## Estrutura

```
dds-cetesb/
  INDICE.md            tabela navegável (DD, data, ementa, links)
  indice.csv           mesma tabela para planilha ou script
  texto/AAAA/*.md      texto integral, com cabeçalho YAML (número, data, ementa, fonte, método de conversão)
  pdf/AAAA/*.pdf       PDF original baixado do site da CETESB
```

Nomes de arquivo: `DD-NNN-AAAA-SIGLAS` (ex.: `DD-038-2017-C`). Quando o inventário traz a mesma DD mais de uma vez (original, atualizada, consolidada), as demais recebem `-v2`, `-v3`; o campo `titulo_no_site` diz qual é qual.

Data e siglas seguem o próprio documento. Onde o inventário do site diverge (data de publicação no lugar da data da DD, ou sigla de diretoria errada — 8 casos), a forma do site fica registrada no cabeçalho (`diretorias_no_site`, `titulo_no_site`).

## Limitações

- O inventário publicado no site da CETESB **não contém todas as DDs** — a numeração anual passa de 300, mas o site lista só uma seleção. Ausência aqui não significa que a DD não existe.
- Textos por OCR (marcados com ⚠️ no índice e com aviso no próprio arquivo) podem ter erros de reconhecimento, sobretudo em tabelas e anexos.
- Fonte do inventário: https://www.cetesb.sp.gov.br/cetesb/institucional/diretoria/decisoes_de_diretoria
