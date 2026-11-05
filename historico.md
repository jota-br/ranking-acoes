# Histórico de versões (pontos de retorno)

Cada mudança relevante vira uma versão numerada. Para desfazer, volte ao arquivo da versão anterior.

## v006 — política de valuation, critério nos balões/detalhes e nível automático
- Nova política de múltiplos por setor (politica-valuation.md e politica.json). Múltiplos e faixas são propostas de Jota para teste.
- A página mostra o critério de cada valor justo (balão ⓘ na coluna FV base e conta completa ao clicar na linha), o marcador ⚑ para desvios aprovados e o selo IA nos ativos com insumos não auditados.
- O nível (N1 a N3) passou a ser calculado pela página a partir do upside e do risco, com a regra no balão.
- Entram CURY3, TEND3 e ITUB4, avaliados pela política (insumos do ChatGPT, não auditados). Os 20 originais mantêm o valor original; VIVA3 e DIRR3 mostram o comparativo pela política.
- Arquivos: index.html, analises.json, politica.json, politica-valuation.md. Para voltar: index-v005.html e o histórico do analises.json no GitHub.

## v005 — cotações dos 151 e página lendo analises.json
- A rotina das 19h passa a ler os tickers do universo.json e atualiza os 151 (brapi, 1 por vez, com tentativa dupla).
- A página passa a montar o ranking a partir do analises.json (os 20 iniciais) e a mostrar o preço atual de todos os ativos do universo. Se o analises.json faltar, usa os 20 embutidos no código.
- Arquivos: index.html (v005), analises.json (v005), update-prices.yml (v005). Para voltar: index-v004.html (página) e o histórico do arquivo update-prices.yml no GitHub (rotina com 20 ativos).
- Setores na página agora seguem o universo.json (por exemplo, VIVA3 passa a aparecer como "Varejo").

## v004 — seção "Universo monitorado" na página
- Nova tabela com os 151 ativos (ticker, setor, preço de referência de 30/10, preço atual e variação para os 20 da carteira), com busca, filtro de setor e opção "só os 20".
- Arquivos: index.html (v004) e universo.json (v003). Para voltar: index-v003.html (página sem a seção).

## v003 — setores aprovados para os 151 ativos
- Cada ativo ganhou um setor (35 setores, de Siderurgia e metalurgia a ETF). Setores aprovados por Jota; agrupamentos podem ser revistos depois.
- Arquivo: universo.json (igual a universo-v003.json). Para voltar ao estado anterior (sem setores): universo-v002.json.
- A página ainda não lê esse arquivo.

## v002 — universo com 151 ativos
- Retirados: ODPV3 e NEOE3 (sem preço na planilha de 30/10).
- Mantidos: ativos abaixo de R$ 1 (BHIA3, CVCB3, LJQQ3, ONCO3, RAIZ4).
- Fora do universo (não são ações): META11, MATB11 e LTBX11 (fundos), além de BDRs, ETFs, futuros, índices e FII.
- Arquivo: universo.json (igual a universo-v002.json). Para voltar: universo-v001.json.

## v001 — universo inicial com 153 ativos
- 152 ações + SMAL11, extraídas da planilha de 30/10/2026.
- Arquivo: universo-v001.json.

## Antes do universo (já publicados no GitHub)
- index.html e prices.json: página com 20 ativos e preços atualizados pela brapi (rotina às 19h, dias úteis).
