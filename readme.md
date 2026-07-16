# VerboPro 🇪🇸

Aplicação web para prática de conjugação de verbos em espanhol, voltada para falantes de português brasileiro. Funciona diretamente no navegador, sem instalação ou dependências externas.

## Como usar

1. Abra o arquivo `verbospro_espanhol.html` em qualquer navegador moderno.
2. Selecione o **tempo verbal** desejado na barra de botões no topo.
3. Leia a pergunta exibida no card: ela indica o **verbo**, o **tempo** e a **pessoa** a conjugar.
4. Digite a conjugação no campo de texto e clique em **Verificar ✅** (ou pressione **Enter**).
5. Leia o feedback:
   - ✅ **Acerto** — exibe a conjugação correta e a tabela completa do verbo.
   - ❌ **Erro** — mostra sua resposta, a forma correta, a regra gramatical aplicada e um exemplo de uso.
6. Clique em **⏩ Próximo** (ou pressione **→**) para avançar para o próximo verbo.

## Tempos verbais disponíveis

| Botão | Tempo | Verbos | Descrição |
|---|---|:---:|---|
| Imperativo | Modo Imperativo | 65 | Ordens e pedidos (tú, usted, nosotros, vosotros, ustedes) |
| Presente | Presente Indicativo | 61 | Ações habituais ou em curso (yo, tú, él, nosotros, vosotros, ellos) |
| Pretérito | Pretérito Indefinido | 62 | Ações concluídas no passado |
| Futuro | Futuro Simple | 60 | Ações futuras |
| Reflexivos | Verbos Reflexivos | 41 | Verbos com pronome reflexivo (me, te, se…) |
| Subjuntivo | Presente do Subjuntivo | 62 | Dúvida, desejo, hipótese |
| Condicional | Condicional Simple | 62 | Ações condicionais ("faria", "comeria"…) |
| 🔀 Misturado | Todos os tempos | 413 | Sorteio aleatório entre todos os tempos acima |

## Funcionalidades

- **Meta diária** — padrão de 10 acertos por dia; acompanhe pelo painel de estatísticas.
- **Streak 🔥** — contador de dias consecutivos de prática, salvo automaticamente.
- **Áudio 🔊** — botão para ouvir a conjugação em espanhol via síntese de voz do navegador.
- **Tema claro/escuro 🌙** — alternado pelo botão no canto superior direito.
- **Dicas de estudo ❓** — modal com orientações e estratégias de aprendizado.
- **Resetar meta 🔄** — zera os acertos do dia para recomeçar a contagem.
- **Persistência** — progresso, streak e preferências são salvos no `localStorage` do navegador.

## Atalhos de teclado

| Tecla | Ação |
|---|---|
| `Enter` | Verificar resposta |
| `→` (seta direita) | Próxima pergunta |

## Estrutura do projeto

```
verbospro/
└── verbospro_espanhol.html   # Aplicação completa (HTML + CSS + JS em arquivo único)
```

Não há dependências de frameworks, bibliotecas externas ou servidor. Basta abrir o arquivo no navegador.

## Verbos incluídos

A aplicação cobre verbos regulares e irregulares das principais categorias:

- **Irregulares totais**: ir, ser, decir, hacer, poner, salir, tener, venir…
- **Mudança e→ie**: cerrar, pensar, preferir, sentir, encender, perder…
- **Mudança o→ue**: recordar, dormir, volver, encontrar, jugar…
- **Mudança e→i**: pedir, servir, repetir, elegir, seguir…
- **Verbos em -uir**: construir, destruir, incluir, concluir, huir…
- **Mudança c→qu**: explicar, tocar, aparcar…
- **Reflexivos**: levantarse, acostarse, vestirse, ducharse…
- **E muitos outros** distribuídos pelos 7 tempos verbais.

## Requisitos

- Navegador moderno com suporte a ES6+ (Chrome, Firefox, Edge, Safari)
- Para o áudio: suporte a `SpeechSynthesis` API e voz em espanhol instalada no sistema operacional
