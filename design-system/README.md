Eduka é um app de reforço escolar gamificado em matemática e português para o ensino fundamental, contratado pela escola. A marca gira em torno do Kadu, o coelho cujas orelhas formam o K de "eduka". A peça laranja que flutua ao lado dele é a lacuna de aprendizagem: quando o aluno aprende, ela volta para o lugar.

## Uma marca, dois registros

O mesmo produto tem duas caras, e elas precisam parecer da mesma família.

| | App do aluno (6 a 14 anos) | Painel do professor |
| --- | --- | --- |
| Papel | Jogar, praticar, ganhar pontos | Ler, entender e gerar relatórios |
| Cor | `violeta` e `laranja` em áreas grandes | Neutros dominam; `violeta` só em ação e item ativo |
| Títulos | Fredoka (`aluno-titulo`, `aluno-display`) | Lexend (`prof-titulo`, `prof-subtitulo`) |
| Texto | Lexend `aluno-corpo` (18px) | Lexend `corpo` (16px) e `prof-tabela` (14px) |
| Cantos | `radius-lg` e `radius-xl` | `radius-sm` e `radius-md` |
| Profundidade | `shadow-aluno` | Sem sombra; borda `line` e fundo `surface-raised` |
| Ícones | Phosphor, peso Fill, 28px | Phosphor, peso Regular, 20 a 24px |
| Margem lateral | `space-5` (20px) | `space-4` (16px) |
| Toque mínimo | 48px (`space-12`) | 44px |

O que amarra os dois: a mesma paleta, a mesma família Lexend no texto, o mesmo símbolo (o Kadu) e os mesmos cantos arredondados (só muda o tamanho).

## Voz

- Fale com o aluno como um colega mais velho: frases curtas, segunda pessoa, verbo no começo. "Vamos treinar frações", "Quase! Confira o denominador".
- O erro nunca é culpa do aluno. Mostre o que olhar, não o que ele fez de errado: "Confira o denominador", e não "Você errou o denominador".
- Com o professor, use linguagem pedagógica e direta: "habilidade", "lacuna", "reforço". Evite "score", "cluster" e "risco".
- Não compare alunos. Nenhuma tela mostra ranking individual, posição ou "melhor da turma". O que se compara é o aluno com ele mesmo e a turma com a meta da turma.
- Pontos de exclamação só em conquista do aluno, no máximo um por tela. Emoji não entra na interface.

## Cores

- A cor principal é `violeta`. Ela marca o botão principal, o item ativo da navegação e os links. Texto sobre ela usa `on-violeta`, nunca branco fixo: no tema escuro o violeta clareia e o texto passa a ser escuro.
- `laranja` é a peça do logo e de tudo que é recompensa: pontos, nível novo, missão da turma, conquista. Laranja não vira texto; quando precisar escrever em laranja, use `laranja-texto`.
- Os estados sempre vêm com ícone e palavra, nunca só cor. Acerto: `acerto` com check e "Certo". Erro: `erro` com X e "Quase". Alerta: `alerta` com triângulo e o motivo. O verde de acerto puxa para o azul-turquesa de propósito, para se separar melhor do vermelho para quem tem daltonismo.
- Texto sobre fundo de estado: `acerto-texto` em `acerto-soft`, `erro` em `erro-soft`, `alerta-texto` em `alerta-soft`. Todos esses pares passam de 4,5:1 nos dois temas.
- Neutros têm um leve tom violeta (`surface`, `ink`, `ink-muted`) para não parecerem cinza solto.
- No painel do professor, a regra é 80% neutro. A cor aparece onde há ação ou estado.
- O mapa de calor de habilidades (P-05) vai de `violeta-soft` (pouco domínio) a `violeta` (muito domínio), com o número escrito dentro de cada célula. Nunca de vermelho a verde: o mapa mostra domínio, não nota.

## Tipografia

- Fredoka (Google Fonts, peso 600) é a voz do jogo: títulos, botões e números de conquista no app do aluno, e o logotipo. Nunca em parágrafo e nunca no painel do professor.
- Lexend (Google Fonts, pesos 400 e 600) é o texto dos dois públicos. Foi desenhada para facilitar a leitura, o que conversa com o tema de recomposição da aprendizagem e é um bom argumento para a banca.
- Carregue as duas assim: `https://fonts.googleapis.com/css2?family=Fredoka:wght@600&family=Lexend:wght@400;600&display=swap`. No Figma, as duas já vêm na lista de fontes.
- Enunciado de exercício usa `aluno-corpo` (18px). Abaixo de 16px, só `legenda` e `prof-tabela`.

## Logo

- O logo principal é "eduka" em minúsculas, Fredoka 600, com a cabeça do Kadu no lugar da letra k. As orelhas fazem o papel da letra: a esquerda reta é a haste e a direita inclinada é o braço. O texto já está convertido em curva no SVG (não depende da fonte instalada).
- No logo, o Kadu é chapado em `violeta` com olhos brancos, sem degradê, para continuar legível em tamanho pequeno. No negativo, ele fica em violeta claro `#A58BFF` com olhos escuros e as letras ficam brancas.
- Versões:
  - `eduka-logo.svg`: logo principal em fundo claro.
  - `eduka-logo-negativo.svg`: logo principal em fundo escuro.
  - `eduka-logo-com-icone.svg` e `eduka-logo-com-icone-negativo.svg`: ícone do app ao lado de "eduka" escrito por inteiro. Use em slide de abertura, loja e materiais em que o ícone precisa aparecer junto do nome.
  - `eduka-simbolo.svg`: só a cabeça do Kadu chapada, com a peça laranja. Avatar, tela de abertura, espaços quadrados.
  - `eduka-favicon.svg`: Kadu branco chapado em quadrado violeta, para a aba do painel do professor.
- Área de respiro: metade da altura da cabeça do Kadu, em volta de todo o logo.
- Tamanho mínimo: logo com 96px de largura; símbolo com 24px.
- Não fazer: trocar a cabeça do Kadu por um k comum no logo principal, mudar a cor do Kadu para outra que não seja violeta, girar ou espelhar as orelhas, aplicar degradê ou sombra no logo, escrever "Eduka" com maiúscula no logotipo. Em texto corrido, o nome é Eduka, com E maiúsculo.

## Ícone do app

`eduka-icone-app.svg`: fundo `violeta`, cabeça do Kadu branca com o degradê do pelo e a peça laranja no canto. Exporte em 1024 × 1024 sem cantos arredondados para a loja; o celular aplica a máscara. O SVG tem os cantos só para a prévia.

## Mascote: Kadu

O Kadu é uma cabecinha de coelho branca que flutua, sem corpo, sem boca e sem contorno. Kadu é apelido de Carlos Eduardo, então o nome carrega o "Edu" e o "K" da marca. As orelhas e o topete desenham o K de "eduka": a orelha esquerda reta é a haste, a direita inclinada é o braço de cima e o topete na testa é o braço de baixo. A peça laranja da marca flutua ao lado dele.

- `kadu.svg`: neutro. Boas-vindas, começo de trilha, telas vazias.
- `kadu-comemorando.svg`: sobe um pouco, fecha os olhos de alegria e a peça vira brilho. Acerto em sequência, nível novo, missão concluída.
- `kadu-dica.svg`: depois de um erro. Tomba a orelha e olha para a peça laranja.
- `kadu-avatar.svg`: em círculo `violeta`, para notificações e cantos de tela.

Regras:
- A expressão está só nos olhos e nas orelhas. Não acrescente boca, nariz, bochecha ou corpo.
- O pelo é branco com degradê suave para lilás `#D3C6FB` no canto de baixo à direita. Esse degradê é o que separa o Kadu do fundo claro; não use branco chapado.
- Fundo ideal: `violeta` ou escuro. Em fundo claro, deixe a sombra flutuante embaixo dele ou apoie num círculo `violeta-soft`.
- Não mexer no K: orelha esquerda sempre reta, direita sempre inclinada para fora, topete sempre descendo para a direita.
- O Kadu só aparece no app do aluno, no máximo um por tela, com no máximo uma frase ao lado. Nunca triste nem bravo.
- Tamanho mínimo: 48px de altura (avatar: 32px).

## Ícones

- Use Phosphor Icons (gratuito, licença MIT): Fill no aluno, Regular no professor. Os dois pesos têm o mesmo desenho, então a família continua igual.
- Cor do ícone: `ink` ou `ink-muted` em repouso, `violeta` quando ativo, cor do estado quando for um estado.
- Barra inferior do professor: Hoje (casa), Turmas (grupo de pessoas), Provas (calendário), Relatórios (gráfico de barras).

## Cantos, sombras e espaçamento

- Grade de 4px. Use só os passos `space-1` a `space-12`.
- Aluno: cartões e botões com `radius-lg`, folhas e telas de conquista com `radius-xl`, padding interno `space-4`, `shadow-aluno` nos cartões que se tocam.
- Professor: cartões e botões com `radius-md`, chips com `radius-sm`, padding interno `space-3`, sem sombra; cartão é `surface-raised` com borda 1px `line`.
- `shadow-flutua` vale para os dois e só para o que flutua: a folha de registrar reforço (P-08) e a faixa de feedback de resposta.
- Campos e botões secundários usam borda `line-strong`, que passa de 3:1 nos dois temas.
- Foco de teclado: anel 2px `focus-ring` com 2px de folga na cor do fundo.

## Gamificação sem expor ninguém

- Pontos e nível aparecem só para o próprio aluno.
- Clãs e missões mostram o progresso da turma em porcentagem, com a barra em `laranja`. Nunca uma lista de quem contribuiu mais.
- Conquista é celebrada com o mascote e uma frase; o número de pontos fica pequeno, em `laranja-texto`.
