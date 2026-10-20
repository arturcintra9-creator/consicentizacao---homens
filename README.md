# Botão Seguro — Site de conscientização (público masculino)

Site de página única sobre violência contra a mulher, voltado para homens adolescentes e jovens adultos. É a parte de conscientização do projeto **Botão Seguro** (Senac, Ensino Médio, 1º ano).

## Como abrir

1. Baixe a pasta do projeto.
2. Dê dois cliques em `index.html`. Ele abre no navegador.

Não precisa de instalação, servidor nem internet. Sem internet, o site troca as fontes Bitter/Inter pelas fontes do sistema, e o resto continua funcionando igual.

**Dica para a Mostra:** abra o site uma vez com internet antes do evento, para o navegador guardar as fontes no cache.

## Como editar

Está tudo em `index.html`. Use Ctrl+F para achar o trecho.

| O que mudar | Onde está |
|---|---|
| Cores, fontes, tamanhos | CSS, seção `1. DESIGN SYSTEM — TOKENS` (`:root`) |
| Textos das seções | HTML, nos comentários `<!-- === 2. NÃO É O ESTRANHO NA RUA === -->` etc. |
| Barras do gráfico "Quem cometeu" | Em cada `<li class="barra" style="--v:59.4">`, troque o `--v` (largura) e o texto do `%` |
| Itens do autoteste | Texto dentro de `<span class="item-texto">` |
| Textos do resultado do autoteste | JavaScript, objeto `RESULTADOS` |
| Gráfico de linha (série histórica) | JavaScript, array `SERIE` |
| Escada (502 / 182 / 79) | HTML da seção `5. A ESCALADA` |

O CSS está separado por seções numeradas e comentadas.

## Privacidade

O site não salva nem envia nada: sem localStorage, sem cookies, sem analytics, sem formulário. O autoteste roda só no navegador e some quando a aba fecha. **Se alguém do grupo editar, não adicione nenhum desses recursos.**

## Conferir antes da Mostra

- [ ] **Distribuição dos autores (59,4% / 21,3% / 10,2% / 4,9% / 4,2%)**: confirmar de qual publicação do FBSP saiu (Anuário? Retrato?) e atualizar a fonte na seção 2 e na lista de fontes. Tem um comentário `[VERIFICAR]` no código.
- [ ] **Links das fontes**: os links do FBSP apontam para a página geral de publicações. Troque pelo link direto de cada PDF. Confira também os links do Movimento Mulher 360 e do Instituto Avon (o da Agência Patrícia Galvão aponta para a página inicial). Também tem um comentário `[VERIFICAR]` no código.
- [ ] **Escada (502 / 182 / 79 por feminicídio)**: são divisões feitas por nós (ex.: 788.531 ameaças ÷ 1.568 feminicídios ≈ 502). Confira se o grupo concorda em usar assim.
- [ ] **"41% conhecem ao menos um homem violento"** (Instituto Avon, 2013): confira se o público da pesquisa eram homens, mulheres ou os dois, e ajuste o texto do último mito se precisar.
- [ ] **"Art. 147-B" do Código Penal**: é o artigo da violência psicológica criado pela Lei 14.188/2021. Vale confirmar no texto da lei.
- [ ] **Barra fixa 180/190**: no celular, os botões ligam direto. No notebook do estande não ligam, o que é normal.
- [ ] Testar no celular de alguém do grupo e no tablet/notebook do estande.
- [ ] Ler tudo em voz alta pelo menos uma vez. Se alguma frase soar como sermão, corte.
