# Avaliação de Acessibilidade

## Escopo da avaliação

Foram selecionadas as seguintes telas para inspeção:

- **Página inicial:** identificação dos elementos de navegação e acesso às transmissões recomendadas.
- **Pesquisa e descoberta:** navegação pelos campos de pesquisa e resultados.
- **Página de transmissão:** identificação das informações do canal, do vídeo e dos controles do player.
- **Chat ao vivo:** identificação dos campos de mensagem e dos elementos interativos.
- **Anúncios:** observação do comportamento do leitor de tela durante a reprodução.
- **Navegação por teclado:** verificação do acesso aos elementos interativos sem utilizar o mouse.

A avaliação teve como objetivo identificar possíveis barreiras de acessibilidade, considerando especialmente pessoas com deficiência visual e usuários que dependem da navegação por teclado ou de tecnologias assistivas.

## Processo utilizado

A inspeção foi organizada em três etapas: **detecção, coleção e discriminação**, com base nas verificações realizadas na interface da Twitch e na análise das ocorrências identificadas.

### Detecção

Foram realizadas verificações utilizando somente o teclado e, posteriormente, um leitor de tela. Durante os testes de teclado, não foram identificadas dificuldades significativas nas funcionalidades verificadas.

Na utilização do leitor de tela, foi observada uma dificuldade durante a reprodução de anúncios: diferentes vozes eram reproduzidas simultaneamente, prejudicando a compreensão das informações.

Também foram avaliados aspectos relacionados à identificação dos controles do player, ao contraste visual e à presença de alternativas textuais em imagens informativas, com o objetivo de identificar possíveis barreiras adicionais de acessibilidade.

### Coleção

As ocorrências foram organizadas em uma tabela para reunir problemas semelhantes, identificar as funcionalidades envolvidas e registrar a frequência dos problemas identificados.

| Código | Problema identificado ou aspecto avaliado | Tela/funcionalidade | Frequência |
|---|---|---|---|
| A01 | Sobreposição de vozes durante anúncios, dificultando a compreensão pelo leitor de tela | Transmissão e anúncios | 3 em 5 testes |
| A02 | Navegação utilizando somente o teclado | Página inicial e controles testados | Nenhuma dificuldade relatada |
| A03 | Identificação dos controles pelo leitor de tela | Player de transmissão | 1 em 5 controles avaliados |
| A04 | Contraste entre textos e plano de fundo | Interface da Twitch | 2 em 5 elementos avaliados |
| A05 | Alternativas textuais para imagens informativas | Página inicial e canais | 2 em 5 imagens avaliadas |

### Discriminação

Os registros foram analisados para distinguir os problemas identificados dos aspectos que não apresentaram dificuldades e daqueles que necessitam de investigação complementar.

| Código | Ocorrência | Classificação | Justificativa |
|---|---|---|---|
| A01 | Múltiplas vozes durante a reprodução de anúncios | Achado observado; causa a investigar | A sobreposição de vozes prejudicou a compreensão das informações em 3 dos 5 testes considerados. É necessário investigar a causa do problema e sua relação com os critérios da WCAG. |
| A02 | Navegação por teclado nas funcionalidades testadas | Sem dificuldade identificada no escopo observado | Não foram relatadas dificuldades significativas durante a navegação pelas funcionalidades avaliadas. |
| A03 | Identificação dos controles pelo leitor de tela | Problema identificado; conformidade a confirmar | Um dos cinco controles avaliados apresentou possível inadequação na identificação pelo leitor de tela. É necessário verificar seu nome, sua função e seu estado. |
| A04 | Contraste dos elementos visuais | Problema identificado; conformidade a confirmar | Dois dos cinco elementos avaliados apresentaram possíveis inadequações de contraste, que devem ser verificadas por meio de medições. |
| A05 | Alternativas textuais das imagens | Problema identificado; conformidade a confirmar | Duas das cinco imagens avaliadas apresentaram possíveis inadequações nas alternativas textuais, sendo necessário verificar se são informativas e se suas descrições são adequadas. |

## Resultados da inspeção

### Síntese dos problemas encontrados

A principal ocorrência identificada durante a avaliação envolveu a utilização do leitor de tela em conjunto com os anúncios reproduzidos na Twitch. A presença de múltiplas vozes simultâneas dificultou a compreensão das informações.

Também foram identificados possíveis problemas na identificação de controles, no contraste visual e nas alternativas textuais de imagens. A navegação por teclado, por sua vez, não apresentou dificuldades significativas nas funcionalidades avaliadas.

A tabela a seguir consolida os problemas identificados, seus critérios WCAG relacionados e as respectivas frequências.

| Problema | Critério WCAG | Tela/Página | Frequência |
|---|---|---|---|
| Dificuldade de compreensão devido à reprodução simultânea de vozes | Investigar a aplicabilidade dos critérios 1.4.2 e 1.4.7 | Transmissão com anúncios | 3 em 5 testes |
| Navegação por teclado | 2.1.1 — Teclado | Páginas e controles testados | Nenhuma dificuldade relatada |
| Identificação dos controles pelo leitor de tela | 4.1.2 — Nome, função e valor | Player e elementos interativos | 1 em 5 controles avaliados |
| Contraste entre textos e plano de fundo | 1.4.3 — Contraste mínimo | Interface | 2 em 5 elementos avaliados |
| Alternativas textuais para imagens informativas | 1.1.1 — Conteúdo não textual | Página inicial e canais | 2 em 5 imagens avaliadas |

### Critérios WCAG violados

Os critérios abaixo estão relacionados aos aspectos avaliados na interface e orientam a análise de conformidade com a WCAG 2.2.

| Princípio | Diretriz | Critério relacionado | Nível |
|---|---|---|---|
| Perceptível | 1.1 — Alternativas em texto | 1.1.1 — Conteúdo não textual | A |
| Perceptível | 1.4 — Distinguível | 1.4.2 — Controle de áudio | A |
| Perceptível | 1.4 — Distinguível | 1.4.3 — Contraste mínimo | AA |
| Perceptível | 1.4 — Distinguível | 1.4.7 — Áudio de fundo baixo ou ausente | AAA |
| Operável | 2.1 — Acessível por teclado | 2.1.1 — Teclado | A |
| Robusto | 4.1 — Compatível | 4.1.2 — Nome, função e valor | A |

O critério 1.4.2 trata do controle de áudio reproduzido automaticamente em determinadas condições. Já o critério 1.4.7 refere-se à possibilidade de compreender a fala em primeiro plano sem que sons de fundo prejudiquem sua compreensão em conteúdo de áudio pré-gravado, sob condições específicas.

O critério 2.1.1 está relacionado ao acesso às funcionalidades por teclado; o 4.1.2 trata das informações programaticamente determináveis sobre nome, função e valor dos componentes; o 1.4.3 estabelece requisitos mínimos de contraste para texto; e o 1.1.1 aborda alternativas textuais para conteúdo não textual.

### Análise dos resultados

Os resultados indicam que a navegação por teclado apresentou comportamento satisfatório nas funcionalidades verificadas, sem dificuldades significativas relatadas e a reprodução de anúncios durante a utilização do leitor de tela representou a principal barreira identificada, pois a presença simultânea de vozes prejudicou a compreensão do conteúdo. 

## Considerações sobre os resultados

A avaliação identificou uma dificuldade relacionada à compreensão de informações sonoras durante a utilização do leitor de tela e apontou outros aspectos relevantes para a acessibilidade, incluindo a identificação dos controles, o contraste visual e as alternativas textuais das imagens.

Os resultados demonstram a importância de avaliar a acessibilidade por diferentes métodos, pois a possibilidade de navegar pela interface não garante, por si só, que todas as informações sejam apresentadas de maneira compreensível e que todos os componentes possam ser utilizados adequadamente.

Conclui-se que a inspeção identificou pontos de atenção que podem afetar a experiência de pessoas com deficiência visual e de usuários que dependem de tecnologias assistivas. Para concluir a avaliação de conformidade, é necessário confirmar os resultados dos testes, registrar as evidências correspondentes e verificar a aplicação dos critérios WCAG relacionados a cada problema.

A partir dessa análise, recomenda-se priorizar a investigação da sobreposição de vozes, verificar a identificação dos controles do player, medir o contraste dos elementos visuais e inspecionar as alternativas textuais das imagens informativas. Essas ações permitirão estabelecer com maior precisão a gravidade das barreiras encontradas e definir possíveis melhorias de acessibilidade.
