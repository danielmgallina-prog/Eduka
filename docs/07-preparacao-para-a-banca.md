# Eduka – Preparação para a banca

Oct 29, 2026 · @Metropole

Material de apoio para a fase classificatória (hoje, 21h; 7 minutos de fala e 7 de perguntas). O roteiro da fala é do Gabriel; este documento cobre a demonstração e as perguntas. Ajustem com as palavras de vocês.

## Demonstração (2:10 a 3:30 do pitch)

Segue a ordem do pitch do Gabriel (slide 5, de 2:10 a 3:30): primeiro o lado da professora Marina, depois o app da Ana. Gabriel clica, Daniel fala na parte do professor e Gabriel fala na parte do aluno. Para a fala bater, a aluna do app precisa aparecer como Ana (hoje está Lia). Tudo no modo Play do canvas, em tela cheia, com o Play já aberto na primeira tela antes de começar.

| Tempo | Tela (modo Play) | Clique (Gabriel) | O que a banca precisa ver (Daniel fala) |
| --- | --- | --- | --- |
| 2:10 | Professor · Importar resultados, passo 3 | Nenhum | A prova que a escola já aplicou; cada questão ligada a uma habilidade, com "sugestão: confirme" (a IA sugere, o professor confirma) |
| 2:25 | Professor · 7º A · Grupos | Abrir "Precisam de reforço" | Em vez de 30 notas, grupos; o de frações tem 6 alunos e código do 5º ano (EF05MA03) |
| 2:40 | Ficha da Ana Beatriz | Tocar no nome da Ana | Regra de três → frações (origem) → multiplicação; pausa de 2 segundos depois de "A origem está em frações." |
| 2:55 | Registrar reforço | Escolher o tipo e salvar | O sistema sugere, o professor decide; aviso para não anotar dado de saúde |
| 3:05 | App do aluno · Trilha (Gabriel fala) | Nenhum | A trilha abre em Frações, antes da regra de três que cai na prova |
| 3:10 | Exercício → erro com dica → tentar de novo → acerto | Errar, tentar de novo, acertar | O aluno não recebe a resposta pronta; recebe uma dica |
| 3:25 | Turma · Clã Cometas | Nenhum | Missão coletiva; a turma vê a própria evolução, sem ranking |
| 3:30 | Volta para os slides |  |  |

**Antes de apresentar:**

- Passar esse caminho inteiro 3 vezes no canvas, de preferência no computador que vai para a sala.
- Gravar a tela fazendo o caminho uma vez, como plano B, e deixar o vídeo aberto numa aba.
- Se o Kadu não aparecer, recarregar a página antes de começar (no render externo ele não carregou).
- Mateus fica de reserva no computador: se o Play travar, ele abre o vídeo do plano B.

## Perguntas da banca (7 minutos)

Cada pergunta tem um responsável principal, mas todos devem saber responder todas (art. 9º). Sugestão de treino: cada um responde em voz alta duas perguntas que **não** são dele. Respostas com no máximo 30 segundos.

| Critério | Pergunta | Resposta curta | Quem responde |
| --- | --- | --- | --- |
| Inovação | Qual a diferença para o Duolingo ou o Khan Academy? | Eles têm conteúdo genérico e o aluno escolhe por onde ir. O Eduka parte da prova real da escola, acha a origem da lacuna e devolve a ação para o professor da turma. | Lucas |
| Inovação | O que é "origem da lacuna"? | O aluno erra regra de três, mas o problema está em frações, que é do 5º ano. O sistema desce pelo mapa de pré-requisitos da BNCC até achar onde ele travou e começa a trilha dali. | Lucas |
| Inovação | Por que não tem ranking, se é gamificado? | O documento dos desafios diz que "nenhuma solução pode expor, rotular ou punir um aluno", e ranking desmotiva justamente quem está atrás. A gamificação é coletiva: a turma inteira soma para a missão do clã. | Daniel |
| Viabilidade | Quem paga e quanto? | A escola ou a secretaria, nunca o aluno. Licença anual por aluno: hipótese de R$ 90 a 110 nas particulares e R$ 55 a 75 nas redes públicas, com mínimo de cerca de R$ 10 mil por escola. Para comparar: a Letrus propôs R$ 103 por aluno por ano à Secretaria de Goiás. E um município com até uns 900 alunos do 6º ao 9º nos contrata por dispensa de licitação (limite de R$ 65.492,11 em 2026). | Gabriel |
| Viabilidade | A escola precisa integrar com algum sistema? | Não. Alunos, turmas e notas entram por planilha. Prova em papel funciona: o professor marca certo ou errado por questão. | Gabriel |
| Viabilidade | Quanto tempo o professor gasta? | Estimamos 10 a 20 minutos por semana, e 30 a 60 na semana de prova, por causa da importação. | Mateus |
| Viabilidade | E se o aluno não tiver celular ou internet? | Funciona no laboratório da escola pela versão web. O professor pode preparar a planilha sem internet e enviar depois. O modo offline completo fica para depois do MVP. | Mateus |
| Viabilidade | Como seria construído? | App do aluno em React Native, painel em Next.js, API em Node.js, motor em Python e banco PostgreSQL com cada escola isolada. MVP em cerca de 12 semanas com 4 a 6 pessoas. | Mateus |
| Qualidade | Onde entra a IA? | Só do lado do professor: sugere a habilidade de cada questão da prova e organiza o currículo, sempre como "sugestão: confirme". O nivelamento e a trilha seguem regras fixas. A IA trabalha para o professor, nunca decide sobre a criança, como pede o desafio: "a decisão é sempre de uma pessoa". | Lucas |
| Qualidade | Por que não usaram o Gemini, que é grátis? | Os termos da API do Gemini proíbem uso em apps acessados por menores de 18 anos. No protótipo, a opção é o Groq; em produção, um modelo aberto rodando em servidor nosso no Brasil, sem mandar dado de aluno para fora. | Lucas |
| Qualidade | Como o sistema sabe que o aluno domina uma habilidade? | Cada resposta conta com um peso: prova vale mais que exercício do app, e acerto depois da dica não conta. Domina a partir de 80%, com pelo menos 3 respostas em momentos diferentes. | Lucas |
| Qualidade | Funciona em português também? | Sim: leitura (localizar, inferir, tema e finalidade) e análise linguística (ortografia, pontuação, concordância), com as mesmas regras. Cada alternativa errada revela um erro típico, como em matemática. | Daniel |
| Design | Por que o painel do professor é tão diferente do app do aluno? | São públicos diferentes: o aluno precisa de algo que pareça jogo; o professor precisa de clareza e pressa. Mesma marca, dois tons. O mascote aparece só para o aluno. | Daniel |
| Design | Por que o professor não vê a nota? | Nota mistura tudo. O professor vê o domínio por habilidade, que diz o que retomar na aula. A lista é em ordem alfabética para ninguém virar "o pior da turma". | Daniel |
| LGPD | Como protegem os dados das crianças? | Cadastro mínimo, sem e-mail, sem foto, sem dado de saúde. Cada escola isolada, cada professor vê só as próprias turmas, a escola não vê desempenho, e todo acesso fica registrado. Seguimos o art. 14 da LGPD e o ECA Digital. | Gabriel |
| LGPD | Precisa de autorização dos pais? | Depende da base legal, que muda entre escola pública e particular, e vamos validar com jurídico. O sistema já tem o registro de consentimento e o canal para os responsáveis. | Gabriel |
| Validação | Vocês conversaram com professores? | Sim, 14 professores de redes pública e particular, a maioria com mais de 10 anos de sala. 79% dizem que metade ou mais da turma chega com dificuldade de anos anteriores, 86% têm no máximo 1 hora por semana para acompanhar aluno a aluno e 71% acharam que a ideia faz sentido. A maior preocupação foi o custo, por isso o preço é por aluno e cabe na dispensa de licitação em municípios pequenos. É uma amostra pequena; o próximo passo é validar com escolas parceiras. | Daniel |
| Validação | Como vão provar que funciona? | Com um piloto de um bimestre: comparamos o domínio das habilidades em provas equivalentes antes e depois. Os dados da demonstração são fictícios, não são resultado. | Gabriel |

### Perguntas mais duras (acrescentadas às 20h)

| Pergunta | Resposta curta | Quem responde |
| --- | --- | --- |
| Vocês dizem que não é trabalho extra, mas marcar certo ou errado por questão dá trabalho. | O sistema já funciona só com o nivelamento e o app. Importar a prova é o ganho a mais, com planilha modelo e a IA sugerindo a habilidade. A evolução é ler o gabarito por foto. | Daniel |
| E se o aluno não usar o app? | Sessões de 5 minutos, missão da turma com prazo ligado à prova, o professor vê quem parou, e quem não tem celular usa no laboratório. Vamos medir alunos ativos por semana desde o piloto. | Gabriel |
| Como vocês sabem que funciona? | Ainda não sabemos, e não prometemos. O próximo passo é um piloto de um bimestre: nivelamento como linha de base e comparação com a prova seguinte. A pesquisa mostra que o problema existe. | Gabriel |
| De onde vem o conteúdo em escala? | Banco por habilidade da BNCC. A IA gera variações e professores das escolas parceiras revisam antes de publicar. | Lucas |
| E o professor de português? | Usa o mesmo painel, filtrado pela disciplina dele. Na demonstração mostramos matemática. | Mateus |
| Os pais acompanham? (ECA Digital) | É evolução prevista: aviso e resumo para os responsáveis, combinados com a escola. Nada de dado sensível. | Mateus |
| O que a secretaria vê na rede pública? | No MVP, a escola e o professor. O relatório da rede, só com dados agregados, vem depois. | Lucas |
| O custo não é alto para a escola? | Foi a maior preocupação na pesquisa. Por isso: preço por aluno, mínimo por escola, parcelado, piloto antes do contrato e dispensa de licitação em municípios pequenos. | Lucas |
| Vocês usaram IA para fazer o projeto? | Sim, como apoio, como o regulamento permite (art. 9º). As decisões são nossas: público, regras, sem ranking, preço e o que ficou fora. Qualquer um de nós explica cada uma. | Daniel |
| O que é diferente de verdade? | Ninguém aqui inventa prova nem aula nova. O Eduka pega a prova que a escola já aplica e transforma em ação no dia seguinte, indo até a origem da lacuna em anos anteriores. | Daniel |

## Checagem final antes de enviar o link

- [ ] Pasta do Drive com quatro partes: apresentação em PDF, link do modo Play, imagens das telas e documentação (pacotes 1 e 2 com o CSV de português novo)
- [ ] Pasta com acesso "qualquer pessoa com o link pode ver"
- [ ] Deck e canvas com acesso aberto pelo link
- [ ] Link testado numa aba anônima, sem login: tudo abre
- [ ] Nenhum nome ou dado real de aluno em slides, telas e planilhas (art. 9º)
- [ ] Slide de decisões da equipe presente (art. 16)
- [ ] Ensaio feito em 7 minutos cravados (art. 18)
- [ ] Vídeo do plano B aberto numa aba
- [ ] Link enviado pelo site oficial às 20h20 (limite 20h40)
