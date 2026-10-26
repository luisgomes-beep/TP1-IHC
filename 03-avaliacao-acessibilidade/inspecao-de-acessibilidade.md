# Avaliação de Acessibilidade

## Escopo da avaliação

Foram selecionadas as seguintes telas para inspeção:

- **Página inicial:** identificação dos elementos de navegação e acesso às transmissões recomendadas.
- **Pesquisa e descoberta:** navegação pelos campos de pesquisa e resultados.
- **Página de transmissão:** identificação das informações do canal, do vídeo e dos controles do player.
- **Chat ao vivo:** identificação dos campos de mensagem e elementos interativos.
- **Anúncios:** observação do comportamento do leitor de tela durante a reprodução.
- **Navegação por teclado:** verificação do acesso aos elementos interativos sem utilizar o mouse.

A avaliação teve como objetivo identificar possíveis barreiras de acessibilidade, considerando especialmente pessoas com deficiência visual e usuários que dependem da navegação por teclado ou de tecnologias assistivas.

## Processo utilizado

A inspeção foi organizada em três etapas: **detecção, coleção e discriminação**, com base nas verificações manuais realizadas na interface da Twitch e nas ocorrências relatadas pela equipe.

### Detecção

Foram realizadas verificações utilizando somente o teclado e, posteriormente, um leitor de tela. Durante os testes de teclado, não foram relatadas dificuldades significativas nas funcionalidades verificadas.

Na utilização do leitor de tela, foi observada uma dificuldade durante a reprodução de anúncios: diferentes vozes eram reproduzidas simultaneamente, prejudicando a compreensão das informações.

Também foram considerados outros aspectos relevantes para a acessibilidade, como a identificação dos controles do player, o contraste visual e a presença de alternativas textuais em imagens informativas. Esses aspectos, entretanto, ainda necessitam de verificações específicas.

### Coleção

As ocorrências foram organizadas em uma tabela para reunir problemas semelhantes, identificar as funcionalidades envolvidas e distinguir resultados observados de verificações pendentes.

| ID | Problema identificado ou aspecto avaliado | Tela/funcionalidade | Frequência |
|---|---|---|---|
| A01 | Sobreposição de vozes durante anúncios, dificultando a compreensão pelo leitor de tela | Transmissão e anúncios | Não confirmada |
| A02 | Navegação utilizando somente o teclado | Página inicial e controles testados | Nenhuma dificuldade relatada |
| A03 | Identificação dos controles pelo leitor de tela | Player de transmissão | Pendente de verificação |
| A04 | Contraste entre textos e plano de fundo | Interface da Twitch | Pendente de verificação |
| A05 | Alternativas textuais para imagens informativas | Página inicial e canais | Pendente de verificação |

### Discriminação

Os registros foram analisados para distinguir as ocorrências observadas dos aspectos que ainda precisam ser verificados.

| ID | Ocorrência | Classificação | Justificativa |
|---|---|---|---|
| A01 | Múltiplas vozes durante a reprodução de anúncios | Achado observado; causa a investigar | A dificuldade foi relatada, mas sua causa e sua relação com uma não conformidade específica da WCAG ainda precisam ser determinadas. |
| A02 | Navegação por teclado nas funcionalidades testadas | Sem dificuldade relatada no escopo observado | Não foi relatada dificuldade significativa durante os testes realizados. |
| A03 | Identificação dos controles pelo leitor de tela | Pendente de verificação | É necessário conferir os nomes, as funções e os estados anunciados pelos controles. |
| A04 | Contraste dos elementos visuais | Pendente de verificação | É necessário medir o contraste das combinações de cores utilizadas nas telas. |
| A05 | Alternativas textuais das imagens | Pendente de verificação | É necessário inspecionar as imagens informativas e verificar suas descrições. |

A ocorrência A01 deve permanecer como um achado em investigação até que a equipe determine a origem do problema. Os demais aspectos não devem ser classificados como defeitos sem evidências específicas.

## Resultados da inspeção

### Síntese dos problemas encontrados

A principal ocorrência relatada durante a avaliação envolveu a utilização do leitor de tela em conjunto com os anúncios reproduzidos na Twitch. A presença de múltiplas vozes simultâneas dificultou a compreensão das informações.

A tabela a seguir consolida a ocorrência observada e os demais aspectos avaliados ou pendentes de verificação. Os critérios indicados representam possibilidades de investigação, não violações confirmadas.

| Problema | Critério WCAG | Tela/Página | Frequência |
|---|---|---|---|
| Dificuldade de compreensão devido à reprodução simultânea de vozes | Investigar a aplicabilidade dos critérios 1.4.2 e 1.4.7 | Transmissão com anúncios | Não confirmada |
| Navegação por teclado | 2.1.1 — Teclado | Páginas e controles testados | Nenhuma dificuldade relatada |
| Identificação dos controles pelo leitor de tela | 4.1.2 — Nome, função e valor | Player e elementos interativos | Pendente |
| Contraste entre textos e plano de fundo | 1.4.3 — Contraste mínimo | Interface | Pendente |
| Alternativas textuais para imagens informativas | 1.1.1 — Conteúdo não textual | Página inicial e canais | Pendente |

A frequência da ocorrência relacionada aos anúncios não foi confirmada por uma contagem documentada. Por isso, não foi utilizada a frequência ilustrativa anteriormente indicada. A associação aos critérios 1.4.2 e 1.4.7 depende da verificação das condições específicas de cada critério.

### Critérios WCAG violados

Até o momento, os resultados fornecidos não permitem confirmar uma violação específica da WCAG 2.2. A tabela abaixo apresenta os critérios relevantes para a investigação, preservando a distinção entre critérios a verificar e violações efetivamente comprovadas.

| Princípio | Diretriz | Critério a verificar | Nível |
|---|---|---|---|
| Perceptível | 1.1 — Alternativas em texto | 1.1.1 — Conteúdo não textual | A |
| Perceptível | 1.4 — Distinguível | 1.4.2 — Controle de áudio | A |
| Perceptível | 1.4 — Distinguível | 1.4.3 — Contraste mínimo | AA |
| Perceptível | 1.4 — Distinguível | 1.4.7 — Áudio de fundo baixo ou ausente | AAA |
| Operável | 2.1 — Acessível por teclado | 2.1.1 — Teclado | A |
| Robusto | 4.1 — Compatível | 4.1.2 — Nome, função e valor | A |

**Observação:** a presença de um critério na tabela não comprova sua violação. O critério 1.4.2 requer análise das condições de reprodução automática de áudio previstas pela WCAG. O critério 1.4.7 trata de fala em primeiro plano com sons de fundo em conteúdo de áudio pré-gravado, sob condições específicas. A ocorrência relatada, isoladamente, não comprova a violação de nenhum dos dois.

### Análise dos resultados

Os resultados preliminares indicam que a navegação por teclado apresentou comportamento satisfatório nas funcionalidades verificadas, sem dificuldades significativas relatadas. Esse resultado se limita ao escopo observado e não garante a acessibilidade de todas as páginas e funcionalidades da plataforma.

A reprodução de anúncios durante a utilização do leitor de tela representou uma dificuldade relevante, pois as vozes simultâneas prejudicaram a compreensão do conteúdo. É necessário investigar se o problema decorre da combinação entre o áudio do anúncio e a saída de voz do leitor de tela, da reprodução automática de áudio ou de outro comportamento da interface.

A identificação dos controles do player, o contraste visual e as alternativas textuais também precisam de investigação complementar. Como esses aspectos não possuem resultados confirmados, não devem ser apresentados como falhas comprovadas.

## Considerações sobre os resultados

A avaliação permitiu identificar uma dificuldade de compreensão durante a utilização do leitor de tela em conjunto com anúncios e registrar aspectos que precisam de investigação complementar. A navegação por teclado não apresentou dificuldades significativas nas funcionalidades testadas.

Os resultados demonstram a importância de avaliar a acessibilidade por diferentes métodos, pois a possibilidade de navegar pela interface não garante, por si só, que todas as informações sejam apresentadas de maneira compreensível.

Conclui-se que a inspeção identificou um ponto de atenção relevante, mas ainda não fornece evidências suficientes para afirmar que houve violação de critérios específicos da WCAG 2.2. A versão final deverá refletir as evidências efetivamente obtidas, incluindo a confirmação das frequências e a identificação dos critérios violados, caso sejam constatadas não conformidades durante os testes complementares.
