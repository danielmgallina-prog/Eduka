# Eduka · Gamificação: especificação para o protótipo

Oct 30, 2026 · @Metropole

A gamificação do Eduka é coletiva, por domínio e sem punição: a turma é um clã, o inimigo é a lacuna, e cada exercício certo de qualquer aluno é um golpe no chefão da turma. Este documento define as mecânicas, as regras de negócio, os números e as telas, e separa o que entra no protótipo da final (30/10) do que fica para o MVP.

## Princípios: o que a evidência diz e as regras fixas do Eduka

A evidência aponta para o mesmo lado das regras que a equipe já tinha: cooperação e domínio funcionam, competição e ranking atrapalham. Uma meta-análise de 2026 sobre gamificação em matemática encontrou efeito positivo moderado na motivação (g = 0,38) e os poucos efeitos negativos vieram de competição, recompensa externa e desenho mal adaptado; a recomendação é progressão gradual, indicadores de progresso individual, tarefas cooperativas e selos usados como feedback, não como controle. O que prende crianças de 11 a 14 em Brawl Stars e Clash Royale é rodada curta com vitória rápida, conquista compartilhada no time e personagens para colecionar. O que o Duolingo mostra é que a sequência de dias funciona melhor com proteção contra a quebra e que meta diária alta demais produz falha constante, não engajamento.

| Princípio | Como aparece no Eduka | Base |
| --- | --- | --- |
| Domínio, não competição | Nenhuma lista de alunos ordenada por desempenho; a maior comemoração é "lacuna fechada" | Ratinho et al., 2026; Hanus e Fox, 2015 |
| Rodadas curtas, vitória rápida | Rodada de 8 exercícios, cerca de 3 minutos, com resumo no fim | Brawl Stars (klicksafe) |
| Conquista compartilhada | A turma é um clã; cada acerto é um golpe no chefão da turma | Teoria da autodeterminação (pertencimento); Classcraft |
| Feedback de progresso, não controle | Selos registram "frações: dominada", nunca condicionam acesso | Ratinho et al., 2026 |
| Perda evitada, sem punição | Sequência de dias letivos com escudo automático; pontos nunca caem | Duolingo (streak freeze) |
| Prática que ensina | Cada rodada é prática de recuperação; cartas voltam em intervalos; minijogos misturam habilidades | Rohrer (intercalação, 7º ano, d = 0,83) |

**Regras fixas (não negociáveis em nenhuma tela):**

1. Nunca mostrar lista de alunos ordenada por pontos, acertos, golpes ou qualquer medida de desempenho. O aluno vê só o próprio progresso; o clã vê só totais.
2. Pontos só sobem. Errar vale zero, nunca negativo. Quebrar a sequência não tira nada.
3. Nada bloqueia a prática: sem vidas, sem energia, sem espera. O aluno sempre pode fazer mais uma rodada.
4. Sem cronômetro em exercício de aprendizagem. Tempo só em minijogo, que é opcional.
5. Nada se compra. Sem loja, sem moeda real, sem anúncio. Cosméticos só se ganham.
6. O professor nunca vê pontos, nível ou sequência; vê domínio por habilidade em %. Ele escolhe a missão do clã entre sugestões ligadas às lacunas da turma.
7. Kadu: no máximo um por tela, grande só na abertura e no resultado do nivelamento; no clã aparece o emblema do clã, não o Kadu.

## Os três ciclos de engajamento

&#91;embedded content: os três ciclos · rodada, dia e temporada\]

O ciclo curto (rodada) é onde o aluno aprende; o médio (dia) cria o hábito; o longo (temporada) dá sentido coletivo. A temporada coincide com o bimestre da escola, então o calendário do jogo é o calendário real: a prova é o final de temporada, e o resultado dela corrige o perfil do aluno para a próxima.

## Mecânicas

Onze mecânicas, cada uma com um motivo pedagógico e uma referência de jogo que o aluno reconhece. Nenhuma depende de IA generativa.

| Mecânica | O que é | Por que funciona | Onde o aluno já viu |
| --- | --- | --- | --- |
| Rodada | 8 exercícios da trilha, cerca de 3 min, com cartão de resumo no fim (acertos, pontos, habilidade que subiu) | Rodada curta com vitória rápida; prática de recuperação a cada questão | Partidas de 3 min do Brawl Stars |
| Sequência (combo) | 3 acertos seguidos na rodada acendem uma faixa "em chamas"; só visual, sem pontos extras | Feedback imediato de competência sem inflar a economia | Combos de jogos de ritmo |
| Chefão da turma | A missão do clã vira um chefão com vida; cada acerto de qualquer aluno tira 1 de vida; 3 fases | Objetivo compartilhado; quem tem mais lacuna contribui praticando o que precisa | Chefes de raid; Guerra de Clãs |
| Baú do clã | Ao cair cada fase, o clã abre um baú com um cosmético para o emblema ou para o Kadu da turma | Recompensa coletiva, previsível, sem dinheiro | Baús do Clash Royale, sem aleatoriedade paga |
| Missões do dia | 3 tarefas pequenas por dia letivo (ex.: 1 rodada, 5 acertos de frações, 3 cartas) | Meta diária alcançável; evita a meta alta que produz falha constante | Quests diárias de Brawl Stars e Duolingo |
| Sequência de dias | Conta dias letivos com pelo menos 1 rodada; 2 escudos por semana seguram a sequência; fim de semana não conta | Aversão à perda com rede de proteção; nunca pune | Ofensiva do Duolingo com congelamento |
| Cartas de revisão | Habilidade praticada vira carta que volta em 1, 3, 7 e 14 dias; acertar na volta sobe o domínio | Repetição espaçada: a lacuna só fecha com acerto dias depois | Colecionáveis; cartas do Clash |
| Minijogos de 60 s | Jogos rápidos que misturam habilidades já vistas (balança de frações, fatia, caça-erro, monta-frase) | Intercalação: decidir qual estratégia usar, como na prova; variedade de interação | Minijogos de festa; modos rotativos |
| Níveis do aluno | Pontos acumulados sobem o nível; o nome do nível é só do aluno | Progresso visível e privado | Trophy road |
| Kadu evolui | Guarda-roupa do Kadu desbloqueado por sequência e por lacunas fechadas | Propriedade e identidade, sem comparar com colegas | Skins do Fortnite e do Roblox, só ganhas |
| Álbum da temporada | Selos por habilidade dominada, cartas revisadas e missões do clã cumpridas; abre no fim do bimestre | Selo como feedback de progresso, não como controle | Álbum de figurinhas; passe de temporada sem compra |
| Torre do clã | Cada missão cumprida constrói um andar; a torre fica o ano todo na tela da turma | Memória coletiva do que a turma conquistou | Construção de base em jogos de clã |

## Economia de pontos, níveis e sequência

A economia é determinística e simples de implementar: tudo é soma de inteiros, sem sorteio. Acertar com dica vale o mesmo que acertar de primeira, para que pedir ajuda nunca custe.

| Evento | Pontos do aluno | Golpes no chefão |
| --- | --- | --- |
| Exercício certo (de primeira ou após dica) | +10 | +1 |
| Exercício errado (viu a resolução) | 0 | 0 |
| Rodada concluída (8 exercícios, qualquer placar) | +20 | 0 |
| Carta de revisão certa | +10 | +1 |
| Minijogo: cada acerto | +5 | 0 |
| Missões do dia completas (3 de 3) | +30 | 0 |
| Lacuna fechada (habilidade dominada) | +100 e selo no álbum | 0 |
| Missão do clã cumprida | +50 para cada membro | baú final |

**Níveis do aluno** (nome visível só para ele): Semente 0 · Broto 200 · Explorador 500 · Construtor 1.000 · Guardião 1.700 · Mestre 2.600 · Lenda 3.800. Um aluno que faz uma rodada por dia letivo com 6 acertos chega a Explorador em cerca de 6 dias e a Construtor em 3 semanas.

**Sequência de dias**: conta dias letivos (segunda a sexta) com pelo menos uma rodada concluída. Dois escudos por semana são usados automaticamente no primeiro dia sem rodada; o aluno vê "O Kadu segurou sua sequência". Sem escudo, a sequência volta a zero sem perder pontos e com a mensagem "Bora recomeçar". Marcos de sequência (5, 10, 20, 40 dias) liberam peças do guarda-roupa do Kadu.

**Regra de domínio (do motor adaptativo, não da gamificação)**: uma habilidade é "dominada" quando o domínio estimado passa de 80% e o aluno acerta a carta de revisão de 7 dias. Se a prova importada contradisser, o domínio cai e a habilidade volta à trilha. A gamificação nunca altera o domínio; só reage a ele.

## Chefão da turma: regras completas

O chefão é a missão do clã com cara de inimigo: a lacuna da turma ganha nome, vida e três fases. Quem tem mais dificuldade é quem mais ajuda, porque cada exercício da própria trilha é um golpe.

| Regra | Definição |
| --- | --- |
| Quem cria | O professor escolhe entre missões sugeridas pelo motor a partir do maior grupo de reforço da turma (ex.: 6 alunos em frações). Ele pode ajustar a meta e a data. |
| Nome | Gerado por tabela fixa habilidade → criatura: Dragão das Frações, Golem da Multiplicação, Hidra da Regra de Três, Fantasma da Vírgula, Esfinge da Interpretação. Sem IA. |
| Vida | Igual à meta da missão (ex.: 500). Prazo = data da prova. |
| O que dá golpe | Exercício certo ou carta de revisão certa na habilidade da missão **ou em um pré-requisito dela** (a Ana praticando multiplicação também acerta o Dragão das Frações). Minijogo não dá golpe. |
| Limite diário | 60 golpes por aluno por dia. Depois disso os pontos continuam, o golpe não; mensagem: "Você já deu o máximo de golpes hoje. Deixa a turma ajudar." Evita que três alunos carreguem o clã. |
| Fases | Três, a cada terço da vida. Ao cair uma fase: animação na próxima abertura do app de cada aluno, o chefão muda de forma (rachaduras) e o clã abre um baú. |
| Vitória | Vida zero: "Chefão derrotado!", +50 pontos para cada membro, baú final com item lendário garantido, um andar na torre do clã. |
| Prazo vencido | Sem punição. "O chefão fugiu com 32% de vida. Ele volta na próxima temporada 10% mais fraco." Os golpes dados ficam no álbum. |
| O que a turma vê | Chefão, barra de vida, fase, dias até a prova, golpes da turma hoje. Nunca uma lista de quem deu quantos golpes. |
| O que o aluno vê de si | Só no próprio cartão: "Você deu 23 golpes nesta temporada". |
| O que o professor vê | Progresso da missão em % e participação (quantos alunos praticaram na semana), como já existe no painel. Nenhum ranking de golpes. |

**Números fixos para a demonstração** (coerentes com as telas já feitas): 7º A · Dragão das Frações · vida 500 · 340 golpes dados (68%) · fase 3 de 3 · 2 baús abertos · prova sexta, 6/11 · Ana deu 23 golpes · golpes da turma hoje: 41.

## Skins e baús (nada se vende)

O aluno personaliza o próprio Kadu; a turma personaliza o emblema do clã. Tudo se ganha com prática, nada tem preço. O ECA Digital (Lei 15.211/2025) veda caixa de recompensa paga para crianças e adolescentes; a Riot bloqueou o League of Legends para menores no Brasil por depender de baús pagos. O baú do Eduka não tem nenhum caminho de pagamento, e é isso que o torna permitido. Na banca e nas telas o nome é sempre "baú", nunca "lootbox".

**Guarda-roupa do Kadu (skin do aluno)**

| Categoria | Exemplos | Como se ganha |
| --- | --- | --- |
| Cabeça | boné, laço, fones, coroa de folhas | marcos de sequência (5, 10, 20, 40 dias) |
| Rosto | óculos, pintura de guerra, sardas | nível novo (1 item fixo por nível) |
| Cor do Kadu | branco (padrão), lilás, menta, pêssego | lacuna fechada (1 baú pessoal) |
| Fundo da tela inicial | floresta, espaço, praia, cidade | álbum da temporada completo |
| Efeito de acerto | confete, estrelas, faíscas, bolhas | baú pessoal |

O aluno começa com 2 itens por categoria. A skin é vista só por ele (tela inicial e resultado): assim não existe "quem tem a skin legal" na turma, a pressão que o Fortnite cria com o "default".

**Emblema do clã (skin da turma)**: forma do escudo, duas cores, símbolo e lema. O lema vem de uma lista de palavras (ex.: "Juntos", "Sem medo de errar", "Frações não nos assustam"), nunca texto livre, para não precisar de moderação. Itens do emblema vêm dos baús do clã; a escolha é por votação no app (maioria simples, 48 h) ou aplicada pelo professor. O emblema aparece na tela da turma e no topo da torre: é a vitrine coletiva.

**Como o baú abre** (pessoal ou do clã):

1. Toque: o baú balança e abre revelando 3 itens sorteados do conjunto que o aluno (ou o clã) ainda não tem.
2. Escolhe 1. Os outros 2 voltam ao conjunto. Nunca há repetido.
3. Raridade: comum 60%, raro 30%, lendário 10%, com as porcentagens escritas na tela do baú. A cada 5 baús, pelo menos 1 raro garantido; o baú final da temporada tem 1 lendário garantido.
4. Sem troca entre alunos, sem moeda, sem loja, sem item vendido à parte, sem acelerar com dinheiro.

A surpresa dos 3 itens mantém a emoção de abrir; a escolha de 1 dá autonomia e tira a lógica de cassino. Quando se ganha um baú: cada fase do chefão (clã), vitória sobre o chefão (clã, lendário garantido), lacuna fechada (pessoal), 5 dias de missões completas na mesma semana (pessoal).

## Cartas de revisão e minijogos

As cartas são a repetição espaçada com cara de coleção; os minijogos são a intercalação com cara de brincadeira. Os dois existem por razão pedagógica, não só por diversão.

**Cartas de revisão (o Baralho)**

| Regra | Definição |
| --- | --- |
| Nasce | Quando o aluno termina uma rodada com 4 ou mais acertos em uma habilidade, ela vira carta. |
| Volta | Em 1, 3, 7 e 14 dias. Acertou: passa para o próximo intervalo. Errou: volta para 1 dia e a habilidade reaparece na trilha. |
| Cada carta | 2 exercícios curtos da habilidade. Máximo 5 cartas por dia, cerca de 2 minutos. |
| Estágio visual | Bronze (nova), prata (acertou na volta de 7 dias), ouro (dominada: domínio acima de 80% e acerto aos 7 dias). |
| Frente da carta | Nome da habilidade em linguagem de aluno ("Frações de um número"), código BNCC pequeno (EF05MA03), ícone, "volta em 3 dias". |
| Tela | "Baralho": cartas de hoje em cima, coleção embaixo, com contagem "12 cartas, 3 de ouro". |

A carta de ouro é a prova visual de que a lacuna fechou. É a resposta para a pergunta da banca "como sabem que o aluno aprendeu?": ele acertou de novo, dias depois.

**Minijogos de 60 segundos**

| Minijogo | Matéria | Como joga | O que treina |
| --- | --- | --- | --- |
| Balança | Matemática | Arrasta frações para os dois pratos até equilibrar | Frações equivalentes |
| Fatia | Matemática | Toca as fatias da pizza para mostrar 3/4, 2/5… | Fração de um todo e de um número |
| Ponte | Matemática | Escolhe a operação certa para cada tábua da ponte (+, −, ×, ÷, regra de três) | Decidir qual estratégia usar, como na prova |
| Caça-erro | As duas | Uma resolução com um passo errado; toca no passo errado | Reconhecer o próprio tipo de erro |
| Monta-frase | Português | Arrasta palavras para formar a frase com concordância e pontuação certas | Concordância, pontuação, ordem |

Regras: opcional, com cronômetro de 60 s e placar só do próprio aluno (recorde pessoal). +5 pontos por acerto, sem golpe no chefão. Cada partida mistura 2 ou 3 habilidades que o aluno já praticou (intercalação: no estudo de Rohrer com 7º ano, prática intercalada deu 61% contra 38% na prova final). Libera quando o aluno tem 2 habilidades praticadas. No MVP o resultado do minijogo não altera o domínio; o motor só usa rodadas, cartas e provas.

## Kadu: reações e falas por situação

O Kadu fala pouco, nunca compara, nunca envergonha e nunca usa "errou feio" ou "quase". Cada situação tem 2 ou 3 variações sorteadas para não cansar; a tabela traz uma. Texto fixo, sem IA.

| Situação | Expressão do Kadu | Fala |
| --- | --- | --- |
| Início do nivelamento | curioso | "Vou conhecer você. Errar aqui não tira nada, só me ajuda a montar sua trilha." |
| Resultado do nivelamento | feliz | "Sua trilha começa em Frações. É por aí que tudo destrava." |
| Acerto | feliz | "Isso! +10 e um golpe no Dragão." |
| Erro (1ª vez, com dica) | pensativo | "Olha a dica e tenta de novo. Vale os mesmos pontos." |
| Erro (2ª vez, resolução) | calmo | "Vamos ver juntos, passo a passo." |
| Combo de 3 acertos | em chamas | "Três seguidas!" |
| Rodada concluída (≥ 5 acertos) | comemorando | "Rodada fechada: 7 de 8. Frações subiu." |
| Rodada concluída (≤ 4 acertos) | encorajando | "4 erros viraram 4 dicas. Amanhã essa habilidade volta mais fácil." |
| Missões do dia completas | comemorando | "Dia completo! +30." |
| Escudo usado | protegendo | "Ontem você não veio e eu segurei sua sequência. Tenho mais um escudo nesta semana." |
| Sequência zerada | tranquilo | "A sequência recomeça hoje. Seus pontos continuam todos aí." |
| Carta de revisão certa | feliz | "Acertou de novo, 7 dias depois. Isso é aprender de verdade." |
| Lacuna fechada | festa (único momento grande fora da abertura) | "Frações: dominada. Essa peça encaixou." |
| Fase do chefão caiu | guerreiro | "A turma derrubou uma fase do Dragão! Tem baú para abrir." |
| Chefão derrotado | festa | "Dragão das Frações derrotado. Foi a turma inteira." |
| Prazo vencido | sereno | "O Dragão fugiu com 32% de vida. Ele volta mais fraco." |
| Limite de golpes do dia | piscando | "Você já deu o máximo de golpes hoje. Deixa a turma ajudar." |
| Baú aberto | surpreso | "Três itens apareceram. Escolhe um." |
| Sem rodada hoje (estado vazio) | acenando | "Uma rodada de 3 minutos já conta para o clã." |

Regra de presença: no máximo um Kadu por tela; grande só na abertura, no resultado do nivelamento e na lacuna fechada; nunca na navegação, em listas ou perto dos nós da trilha. Na tela da turma aparece o emblema do clã, não o Kadu.

## Telas: o que muda nas existentes e as novas

Seis telas novas e quatro ajustes. Cada linha traz o conteúdo pronto (textos e números) para o canvas e para o protótipo, no tom lúdico do aluno (cantos 20 a 28 px, Fredoka nos títulos, laranja só em recompensa).

**Ajustes em telas que já existem**

| Tela | O que muda |
| --- | --- |
| Trilha (início) | Faixa no topo: "Sequência: 6 dias · 2 escudos" (ícone de escudo). Cartão acima da trilha: "Missões do dia 1/3: Fazer 1 rodada ✓ · Acertar 5 de frações · Revisar 3 cartas". Botão primário "Rodada de hoje" (laranja). Sem Kadu perto dos nós. |
| Acerto | Abaixo de "+10 pontos": linha "+1 golpe no Dragão das Frações" com ícone pequeno do chefão e a barra de vida descendo 1 ponto. |
| Erro com dica | Fala do Kadu: "Olha a dica e tenta de novo. Vale os mesmos pontos." |
| Turma (clã) | Vira a tela do chefão (abaixo). A barra de missão atual é a barra de vida. |

**Telas novas**

| Tela | Conteúdo |
| --- | --- |
| Resumo da rodada | Título "Rodada fechada". "7 de 8". "+90 pontos" (70 + 20 da rodada). "Frações ↑" com barra subindo, sem porcentagem. "+7 golpes no Dragão". "Missões do dia 2/3". Kadu pequeno comemorando. Botões "Mais uma rodada" (primário) e "Voltar à trilha". |
| Chefão da turma | Topo: emblema do 7º A. Centro: Dragão das Frações feito de peças que se encaixam (a marca), com rachaduras na fase 3. Barra de vida "160 / 500" e "Fase 3 de 3". Linha "Prova sexta, 6/11 · 7 dias". "Golpes da turma hoje: 41". Cartão privado "Você deu 23 golpes nesta temporada". "2 baús abertos" com os 2 itens do emblema. Torre do clã com 3 andares, pequena. Botão "Dar golpes agora" (abre a rodada). Sem lista de alunos. |
| Baú | Baú fechado no centro; toque: balança e abre; 3 cartas viram: "Fones (comum)", "Coroa de folhas (raro)", "Fundo espaço (comum)". "Escolhe 1". Rodapé: "Comum 60% · Raro 30% · Lendário 10% · Nada aqui se compra". |
| Baralho | "3 cartas para hoje": Frações de um número (volta em 3 dias), Multiplicação (7 dias, prata), Interpretação de texto (1 dia). Abaixo: "Sua coleção: 12 cartas · 3 de ouro" em grade. Carta de ouro com borda dourada e "dominada". |
| Guarda-roupa do Kadu | Kadu em tamanho médio no topo (exceção à regra, confirmar com o Daniel). Abas: Cabeça · Rosto · Cor · Fundo · Efeito. Grade de itens: 2 ganhos por aba, os demais com cadeado e "como ganhar" ("Sequência de 10 dias"). |
| Lacuna fechada | Kadu grande em festa. "Frações: dominada". Carta virando para ouro. "+100 pontos". "Você ganhou um baú". Botão "Abrir baú". |
| Minijogo Balança | Cronômetro 60 s no topo, placar "Recorde: 9". Balança com dois pratos; fichas 1/2, 2/4, 3/6, 1/3, 2/6 embaixo; arrasta para equilibrar. Acerto: pratos nivelam e +5. Fim: "8 certas · +40 pontos". |

**Professor (ajuste mínimo)**: no Painel da turma, o cartão "Missão da turma" passa a mostrar "Dragão das Frações · 68% · participação 21 de 28" e ganha o botão "Escolher próxima missão", que lista 3 sugestões do motor ("Multiplicação: 3 alunos precisam", "Interpretação: 5 alunos"). O professor nunca vê golpes por aluno, pontos ou nível.

## Prioridade: final de hoje, MVP e depois

Para a final só entra o que cabe em poucas horas no protótipo e aparece na demonstração. O resto fica especificado para o MVP.

**Final de hoje, em ordem (cada item cabe em 30 a 60 min no protótipo):**

- [ ] Tela do chefão no lugar da tela da turma, com os números fixos (160/500, fase 3 de 3, 2 baús, 23 golpes da Ana).
- [ ] Acerto mostra "+1 golpe no Dragão" e a barra desce.
- [ ] Resumo da rodada após o 8º exercício (7 de 8, +90, Frações ↑, +7 golpes).
- [ ] Trilha com "Missões do dia 1/3" e "Sequência: 6 dias · 2 escudos".
- [ ] Baú abrindo com 3 itens e escolha de 1 (pode ser estático, uma animação simples).
- [ ] Exportar a tela do chefão em PNG e trocar a imagem do slide "Turma" no deck.

**Se sobrar tempo hoje:** Baralho com "3 cartas para hoje" · Minijogo Balança com uma interação funcionando.

**MVP (12 semanas):** tudo acima funcional e ligado ao motor · níveis com nomes · guarda-roupa do Kadu · emblema do clã com votação · torre · álbum da temporada · os 5 minijogos · limite diário de golpes · escudos automáticos · cartão "Escolher próxima missão" do professor.

**Depois:** evento da escola (todos os clãs contra um chefão da escola) · temporadas com tema · Kadu animado · cosméticos sazonais.

**Na apresentação:** o slide "O que prende a Ana" resume as mecânicas; a tela do chefão é a prova visual. Se a tela não ficar pronta, o slide cobre sozinho.

## Fontes

- [Ratinho et al., 2026. Gamificação em matemática: revisão sistemática e meta-análise, Educational Psychology Review](https://link.springer.com/article/10.1007/s10648-025-10108-1): g = 0,38 na motivação; efeitos negativos ligados a competição e recompensa externa; recomenda domínio, progressão gradual e cooperação.
- [Rohrer, estudo de eficácia de prática intercalada em matemática, 7º ano, IES](https://ies.ed.gov/use-work/awards/efficacy-study-interleaved-mathematics-practice): 787 alunos; 61% contra 38% na prova final; d = 0,83.
- [Klicksafe: o que fascina as crianças em Brawl Stars](https://www.klicksafe.de/en/news/was-fasziniert-kinder-an-brawl-stars): rodadas curtas, vitórias rápidas, conquista compartilhada em time, personagens.
- [Trophy: estudo de caso da gamificação do Duolingo](https://trophy.so/blog/duolingo-gamification-case-study): sequências com congelamento duram mais; meta diária alta demais gera falha constante.
- [Screenwise: o que seu filho está jogando em 2026, por idade](https://screenwiseapp.com/guides/popular-video-games-by-age): skins como status e a pressão do "default" no Fortnite; Roblox como ponto de encontro.
- [Olhar Digital: Riot bloqueia League of Legends para menores no Brasil](https://olhardigital.com.br/2026/03/13/games-e-consoles/riot-games-bloqueia-league-of-legends-para-menores-no-brasil-entenda-a-nova-lei/): ECA Digital (Lei 15.211/2025) e caixas de recompensa pagas.
- [Conjur: impactos do ECA Digital no segmento de jogos eletrônicos](https://www.conjur.com.br/2025-out-22/impactos-do-eca-digital-no-segmento-de-jogos-eletronicos/): vedação de loot boxes, verificação de idade e supervisão parental.
- Hanus e Fox, 2015, Computers & Education: ranking e selos reduziram a motivação intrínseca ao longo de um semestre. Referência clássica, não consultada nesta sessão.
