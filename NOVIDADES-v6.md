# Arcana Atlas V6 — Sequência do alfabeto e novos desafios de digitação

A V6 mantém os cursos, a Árvore da Vida, a lousa, a digitação, a ordenação, o filtro por **tipo de pergunta** e as configurações locais das versões anteriores.

## 1. Alfabeto em sequência: quatro modalidades

No **Modo Quiz → Conteúdo ou modalidade**, escolha **↔ Alfabeto em sequência · normal e inversa**. Abaixo, em **Tipo de pergunta**, marque uma ou várias das seguintes opções:

| Modalidade | Direção | Entrada |
| --- | --- | --- |
| Ordem normal · digitação | Aleph → Tav | Digite o **nome** ou o **caractere hebraico** de cada letra |
| Ordem inversa · digitação | Tav → Aleph | Digite o **nome** ou o **caractere hebraico** de cada letra |
| Ordem normal · lousa | Aleph → Tav | Desenhe cada letra com mouse, toque ou caneta |
| Ordem inversa · lousa | Tav → Aleph | Desenhe cada letra com mouse, toque ou caneta |

**As questões são sequenciais, não embaralhadas, nessa categoria.** Se todas as 22 letras estiverem ativas, cada modalidade tem 22 etapas. Se apenas Aleph, Gimel e Tav estiverem ativas, a ordem normal será Aleph → Gimel → Tav; a inversa será Tav → Gimel → Aleph. O programa mostra a posição da próxima letra **ativa** sem revelar seu nome/símbolo antes de sua resposta.

Se você marcar mais de uma modalidade, o sistema executa um percurso completo de cada uma, em blocos, na ordem indicada no seletor. Por exemplo: com 6 letras ativas e três modalidades selecionadas, serão 18 etapas.

Na categoria **Alfabeto em sequência**, o controle de 5/10/20/40 perguntas fica oculto porque a prática usa todas as letras ativas. Na categoria **Misturar todas**, os exercícios do alfabeto também podem entrar, porém como questões individuais sorteadas; nesse caso, a sessão não é um percurso sequencial.

As avaliações da lousa são **heurísticas**, baseadas na comparação aproximada com o desenho tipográfico da letra: não utilizam IA, nem verificam obrigatoriamente a ordem dos traços. Pode haver falsos acertos e falsos erros.

## 2. Dois tipos de digitação sobre Arcanos Maiores

Na categoria **⌨ Digitação · escreva a resposta**, ou no modo misturado, marque:

- **Número do Arcano → digite o nome da carta.** O programa exibe apenas um número de 0 a 21. Exemplo: `0` → `O Louco` ou `Louco`. Não mostra a carta.
- **Nome do Arcano Maior → digite seu número.** Exemplo: `A Justiça` → `11` ou `XI`. A imagem também não aparece.

O programa aceita grafias dos títulos com ou sem artigo inicial e algumas variantes usuais (por exemplo, **A Papisa** para **A Sacerdotisa**). A numeração é a **Rider–Waite–Smith**: **A Força = VIII** e **A Justiça = XI**. Não confundir número do arcano (0–21) com número do caminho da Árvore da Vida (11–32).

Essas modalidades respeitam **apenas os Arcanos Maiores ativados em Configurações**. Se você desativar um Arcano Maior, ele não será sorteado nessas perguntas.

## 3. Navegação somente por Enter nas perguntas digitadas

1. Digite a resposta no campo.
2. Pressione **Enter** para corrigir.
3. Leia o feedback.
4. Pressione **Enter** novamente para ir à próxima questão (ou concluir, na última).

O campo da questão seguinte recebe foco automaticamente, permitindo praticar sem alternar para o mouse. O comportamento é aplicado aos desafios de digitação antigos e novos, inclusive os percursos alfabéticos digitados. A lousa continua com os botões próprios de avaliar e avançar.

## 4. Estatísticas e compatibilidade

Com todas as letras e cartas habilitadas, a V6 tem **964 modelos de desafio** (832 anteriores + 88 etapas alfabéticas nos quatro percursos + 44 perguntas de número/nome do Arcano) e **49 tipos de pergunta**. O total disponível diminui conforme você desabilita letras, cartas ou tipos. O **Misturar todas** usa apenas as sequências curtas do jogo de ordenação, então pode mostrar menos modelos disponíveis que o banco total.

Os dados permanecem em `localStorage` sob a mesma chave `arcana-atlas-v1` das versões anteriores. Seleções **parciais** de tipos permanecem parciais; se a seleção anterior era literalmente **todos** os tipos de uma categoria, a V6 inclui automaticamente os tipos novos. O backup JSON continua funcionando.

## 5. Atualizando da V5

1. Abra a V5 e use **Configurações → Exportar progresso e configurações**.
2. Descompacte o ZIP da V6 e substitua os arquivos da V5 **na mesma pasta**, mantendo a pasta `assets/cards` se já tiver baixado as imagens.
3. Abra `index.html`. Se o navegador não mostrar as preferências antigas, importe o JSON exportado.
4. Não é necessário instalar pacotes, nem configurar servidor.

**Importante:** o ZIP contém o código e o baixador das imagens, mas **não inclui os 78 arquivos JPG** das cartas. A apresentação das cartas pode usar os URLs de origem enquanto você tiver internet, ou os JPGs locais após usar `baixar-cartas.cmd`.

Arquivos centrais: `index.html`, `styles.css`, `data.js`, `app.js`, `drawing.js`.
