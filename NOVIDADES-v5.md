# Arcana Atlas — V5: lousa por carta/caminho e digitação

## Cinco novos tipos

| Categoria | Tipo | Controle de ativação | Resposta |
|---|---|---|---|
| Lousa | Arcano Maior → desenhar letra | **Carta E letra** ativas | Desenho livre no canvas |
| Lousa | Caminho 11–32 → desenhar letra | Letra ativa | Desenho livre no canvas |
| Digitação | Imagem de Arcano Maior → número do Arcano | Carta ativa | 0–21 (arábico), 0, I–XXI (romano) |
| Digitação | Imagem de Arcano Maior → número do caminho | Carta ativa | 11–32 |
| Digitação | Letra em hebraico → nome | Letra ativa | Nome, aceitando variantes comuns |

### Atenção

Os números dos **Arcanos Maiores** e dos **caminhos** não são a mesma coisa:
- **A Imperatriz**: Arcano **III / 3**, caminho hermético **14** (Daleth).
- **O Louco**: Arcano **0**, caminho **11** (Aleph).
- **A Força**: Arcano **VIII / 8**, caminho **19** (Teth).
- **A Justiça**: Arcano **XI / 11**, caminho **22** (Lamed).

A imagem do Rider–Waite–Smith é mostrada sem esconder seus elementos impressos, incluindo título e numeração. Se ainda não estiverem armazenadas em `assets/cards`, as ilustrações precisam de internet e serão carregadas pelo endereço remoto quando disponível. Execute `baixar-cartas.cmd` para obter as imagens locais.

### Compatibilidade

Preserva a mesma chave `arcana-atlas-v1` no armazenamento do navegador, o sistema de estatísticas, backup JSON, seleção de letras/cartas e categorias/tipos personalizados. Quem havia selecionado **todos** os tipos da V4 passa a ter os novos tipos habilitados. Seleções parciais continuam parciais. A digitação não envia suas respostas a serviços externos.

A correção da lousa continua **heurística e aproximada**; a digitação é corrigida por texto normalizado e comparações explícitas.
