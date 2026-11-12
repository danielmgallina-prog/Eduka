# Eduka – Relatório do projeto para validação

Oct 29, 2026 · @Metropole

Equipe Abençoados f.c (Lucas, Mateus, Gabriel e Daniel) · Hackathon UniCesumar e Elotech 2026 · Desafio 2 "Aprender no tempo certo". Leiam e marquem nos comentários o que não bate com o que vocês entenderam.

## Resumo em 1 minuto

**Eduka: reforço escolar gamificado.** É um app que a escola contrata para alunos do **6º ao 9º ano**, em **matemática e português**. O aluno faz um nivelamento, a escola importa as notas das provas por questão e o sistema descobre **onde a dificuldade começou** (ex.: a aluna erra regra de três porque trava em frações). A partir daí, monta uma trilha que começa por essa lacuna. O professor recebe, no celular ou no computador, quem precisa de reforço, em qual habilidade e uma sugestão para a próxima aula.

O que nos diferencia do Duolingo e do Khan Academy:

- Parte das **provas reais da escola**, não de um conteúdo genérico.
- Vai até a **origem da lacuna**, inclusive em habilidades de anos anteriores.
- Devolve a ação para o **professor da turma**.
- Gamificação **só coletiva**: a turma joga junta e ninguém é exposto.

## Problema, público e ciclo

**Problema.** Em 2023, só 16,5% dos alunos do 9º ano tinham aprendizagem adequada em matemática, e 35,9% em português (Todos Pela Educação, com dados do Saeb). A escola aplica prova, mas o resultado raramente vira ação: o professor tem muitas turmas e pouco tempo para descobrir quem precisa de reforço e em quê.

**Público.**

- Alunos do 6º ao 9º ano (11 a 14 anos), em matemática e português.
- O mapa de habilidades desce até os anos iniciais, porque é lá que a lacuna costuma começar.
- Quem contrata é a escola ou a secretaria; o aluno nunca paga.

**O ciclo ("um perfil libera o outro").** Ao final, o ciclo recomeça a cada prova.

1. **Escola** importa turmas, alunos e professores e libera o nivelamento.
2. **Aluno** faz o nivelamento; o sistema encontra o ponto de partida e monta a trilha.
3. **Professor** cadastra a prova e publica a trilha de revisão.
4. **Aluno** faz a trilha de revisão.
5. **Professor** importa os resultados da prova por questão; o sistema atualiza as lacunas.
6. **Aluno e professor:** a trilha do aluno se ajusta, e o professor vê os grupos que precisam de reforço.
7. **Professor** registra o reforço feito em sala; a próxima prova mede o resultado.

## Perfis, telas e decisões de produto

No canvas "Eduka Interface", 37 das 59 telas mapeadas estão prontas, com o fluxo navegável no modo Play.

| Perfil | O que faz | Telas prontas |
| --- | --- | --- |
| Aluno (app lúdico, celular e computador) | Entra com código da escola ou QR Code + PIN; faz nivelamento; segue a trilha em matemática ou português; vê provas e a missão do clã | 21 de 24 |
| Professor (painel sóbrio, celular e computador) | Vê o que precisa da atenção dele hoje; acompanha grupos de reforço e a ficha de cada aluno; cadastra provas e trilhas de revisão; importa resultados; registra reforços; gera relatório | 12 de 21 |
| Escola (administrador, computador) | Implanta o sistema (assistente de 9 etapas, com Currículo); cadastra alunos e gera os acessos; cuida da privacidade | 4 de 14 |

**Decisões de produto que todos precisam saber defender:**

- **Sem ranking individual.** A gamificação é só coletiva (missão do clã da turma). O aluno vê apenas os próprios pontos e nível.
- **O professor vê domínio da habilidade em %, nunca nota, ranking ou XP.** Listas de alunos sempre em ordem alfabética.
- **No erro, o aluno tenta de novo com uma dica** antes de ver a resposta.
- **A escola não vê desempenho pedagógico**, só cadastro, uso agregado e implantação. Cada professor vê só as próprias turmas.
- **Aluno entra sem e-mail**, com código ou QR + PIN de 4 dígitos.
- **O mascote Kadu aparece só no app do aluno** e só em momentos de emoção ou orientação (abertura, nivelamento, acerto, erro, missão concluída).
- **Linguagem pedagógica:** habilidade, lacuna, reforço. Nada de "score", "risco" ou "cluster".
- **Registro de reforço avisa** para não anotar diagnóstico nem dado de saúde.

**Identidade visual:** violeta como cor principal, laranja só para recompensa; fontes Fredoka e Lexend; dois tons dentro da mesma marca (aluno lúdico, professor sóbrio).

## Motor, IA e tecnologia

**Motor (regras fixas, sem IA decidindo sobre o aluno):**

- **Nivelamento:** até 15 perguntas por disciplina, sem nota. Se erra, desce para o pré-requisito; se acerta, sobe. Termina ao achar o ponto de partida.
- **Domínio por habilidade (0 a 100%):** cada resposta conta com peso (app 1; nivelamento 1,5; prova importada 3; acerto depois da dica não conta). Domina a partir de 80%; lacuna abaixo de 60%, com no mínimo 3 evidências.
- **Origem da lacuna:** desce pelo mapa até o pré-requisito mais básico com lacuna confirmada.
- **Trilha:** começa pela origem; 5 exercícios por etapa; avança com 4 de 5; revisões depois de 1, 3 e 7 dias; prova próxima aumenta a prioridade.
- **Fila de atenção:** lacuna em pré-requisito, 7 dias sem atividade, queda entre avaliações ou lacuna cobrada em prova próxima. O professor pode dispensar com motivo.
- **Pontos:** 10 no primeiro acerto, 5 depois da dica; nível a cada 100 pontos. A missão do clã conta exercícios, não pontos.
- **Português:** leitura (localizar → inferir → tema e finalidade) e análise linguística (ortografia, pontuação, concordância), com as mesmas regras.

**IA: "a IA trabalha para o professor, nunca decide sobre a criança".**

- Ela só prepara conteúdo: extrai o currículo do arquivo da escola, sugere a habilidade BNCC de cada questão da prova e gera exercícios e dicas. Tudo aparece como "sugestão: confirme", e um professor aprova.
- Nenhum nome, nota ou resposta de aluno é enviado para a IA.
- Sem a IA, tudo funciona pelo catálogo BNCC preenchido à mão.
- **O Gemini ficou fora:** os termos da API dele proíbem uso em apps acessados por menores de 18 anos. No protótipo, a opção é o Groq (gratuito, sujeito a conferência dos termos); em produção, um modelo aberto rodando em servidor próprio no Brasil.

**Formas de a escola trazer o currículo:** catálogo BNCC pré-carregado (padrão), upload do arquivo da proposta curricular (PDF, Word ou planilha), planilha modelo do Eduka ou currículo da rede importado uma vez pela secretaria.

**Tecnologia proposta:**

| Parte | Tecnologia |
| --- | --- |
| App do aluno | React Native (Expo), com versão web |
| Painel do professor e da escola | React com Next.js |
| API | Node.js com NestJS |
| Motor | Python com FastAPI |
| Banco de dados | PostgreSQL, com isolamento por escola |
| Filas | Redis |
| Hospedagem | Containers Docker em nuvem com região em São Paulo |

## Negócio, viabilidade e LGPD

**Quem paga e quanto** (valores são estimativas da equipe, não preços de mercado):

| Cliente | Modelo | Preço de referência | Exemplo |
| --- | --- | --- | --- |
| Secretaria municipal | Licença anual por aluno | R$ 55 a 75 por aluno por ano (menor com volume) | Rede de 5.000 alunos a R$ 62: cerca de R$ 310 mil por ano; até \~900 alunos cabe na dispensa de licitação (R$ 65.492,11 em 2026) |
| Escola particular | Licença anual por aluno, em 10 ou 12 parcelas | R$ 90 a 110 por aluno por ano; mínimo de \~R$ 10 mil por escola | 500 alunos do 6º ao 9º: cerca de R$ 50 mil por ano |
| Piloto | 45 a 60 dias com 1 ou 2 turmas (particular); contrato de solução inovadora (pública) | Sem custo na particular; pago na pública | Até 2 turmas |

**Viabilidade:**

- **Implantação:** uma escola pequena fica pronta em 1 dia útil, se as planilhas estiverem prontas; uma rede, em 3 a 6 semanas (estimativas).
- **Sem integração obrigatória:** tudo entra por planilha. Prova em papel funciona: o professor preenche certo/errado por questão.
- **Tempo do professor:** 10 a 20 minutos por semana sem prova; 30 a 60 minutos na semana de prova (estimativa).
- **Infraestrutura:** cerca de R$ 2 mil por mês para uma rede de 5.000 alunos (estimativa). O preço fecha vendendo para a rede inteira, não escola por escola.
- **MVP:** cerca de 12 semanas com 4 a 6 pessoas, terminando num piloto fechado com professores.

**LGPD e proteção do aluno:**

- **Cadastro mínimo:** nome, identificador escolar, turma e ano de nascimento (não a data completa). Nunca saúde, laudo, renda, situação familiar, foto ou localização.
- **LGPD, art. 14:** dados de crianças e adolescentes tratados no melhor interesse deles. A base legal exata (escola pública ou particular) depende de validação jurídica.
- **ECA Digital (Lei 15.211/2025, regulamentado pelo Decreto 12.880/2026):** segurança desde o desenho, sem publicidade, sem compras, sem chat entre alunos, sem ranking. **Não citar números de artigos do ECA Digital na fala**, porque não foram conferidos.
- **Técnico:** isolamento por escola, criptografia, verificação em duas etapas para professores e administradores, registro de todo acesso a dado identificado.
- **No hackathon:** só dados fictícios, como exige o regulamento (art. 9º).

## Status das entregas por pessoa

| Pessoa | Papel | Entregue | Pendente |
| --- | --- | --- | --- |
| Daniel | Design e interface | Identidade visual, kit de componentes, 37 telas (aluno, professor e escola, celular e desktop), modo Play, mapa "Fluxo e funções", modelo de slides e imagens | Corrigir pontos confusos do painel do professor; passar o Play inteiro no canvas; abrir o acesso do deck |
| Lucas | Estrutura do produto | Regras do motor, mapa BNCC, canvas de negócio, estrutura do banco e base fictícia (pacotes 1 e 2) | Refazer as alternativas erradas de português; confirmar o número de R$ 65 mil |
| Mateus | Protótipo | Protótipo navegável pronto no canvas | Testar o caminho de demonstração de 2 minutos; gravar vídeo de plano B |
| Gabriel | Pitch e viabilidade | Especificação das telas do professor e da escola; viabilidade e LGPD (pacote 2) | Slides 7 a 9 e roteiro; treinar as perguntas da banca; montar e enviar a pasta do Drive |

Observação: várias entregas foram feitas com apoio de IA (Claude e ChatGPT). Pelo regulamento (art. 9º), isso é permitido, desde que cada um entenda e saiba explicar o que foi feito.

**Links:**

- Painel de entregas: https://claude.ai/artifact/1EojA7nVh4YWxfNbCnCopX
- Guia de marca: https://claude.ai/artifact/M2HjaWcV7d6zEzsFCnMMWo
- Interface (canvas, com modo Play): https://claude.ai/artifact/NHKcZBHrfonXKUCe7fbYff
- Slides: https://claude.ai/artifact/7UU1JLagW4EcbYzSVZRqFv
- Formulário para professores (3 respostas até o meio-dia): https://docs.google.com/forms/d/e/1FAIpQLSezj37UAf\_Ckx2MgcEt7XLmlg4awdxBgKQqSc2\_4bhKZmLPjw/viewform

## O que falta para hoje (regulamento)

O regulamento não exige software funcionando: a entrega obrigatória é a apresentação mais o protótipo navegável, numa pasta do Google Drive (art. 16).

- [ ] Slides completos, com a solução **e as decisões tomadas pela equipe** (art. 16) · Gabriel · até 19h
- [ ] Slide com o resultado da pesquisa com professores · encerrar a contagem às 18h
- [ ] Pasta do Drive: deck em PDF, link do modo Play, PNGs das telas, pacotes 1 e 2 · acesso "qualquer pessoa com o link" · Gabriel
- [ ] Deck e canvas com acesso aberto pelo link · Daniel
- [ ] Testar o link do Drive numa aba anônima
- [ ] Conferir que só há dados fictícios em slides, telas e planilhas (art. 9º)
- [ ] Equipe completa na sala às 19h (arts. 12 e 16); menos de 4 integrantes desclassifica (art. 5º)
- [ ] Ensaio com cronômetro, 7 minutos cravados (art. 18) · 20h às 20h30
- [ ] Cada um responde 2 perguntas da banca sobre a parte de outro colega (art. 9º)
- [ ] Link enviado pelo site oficial · meta 20h20, limite 20h40 (art. 16)
- [ ] Amanhã, 30/10: todos no Auditório Joaquim Lauer às 19h; ausência na chamada desclassifica (art. 22)

## Pontos para a equipe validar

Responda nos comentários se concorda ou não com cada ponto:

1. **Público:** só 6º ao 9º ano, matemática e português. Todos de acordo?
2. **Preço:** faixa do pitch, R$ 90 a 110 por aluno por ano (particular) e R$ 55 a 75 (pública), com mínimo de \~R$ 10 mil por escola. Proposta de valor exato: R$ 96 (particular) e R$ 70, 62 e 55 por volume (pública). Lucas fecha?
3. **Número único na fala:** na fala, só "escola de 500 alunos do 6º ao 9º paga cerca de R$ 50 mil por ano". Rede de 5.000 alunos (cerca de R$ 310 mil por ano) e dispensa de licitação ficam para as perguntas.
4. **IA:** fica só do lado do professor, como sugestão, e sem dado de aluno. O Gemini fica fora por causa da trava de idade nos termos dele.
5. **Solução entregue hoje:** protótipo navegável e documentação, sem código funcionando. Uma parte funcional pode entrar como melhoria antes da final (art. 23).
6. **Login na demonstração:** acesso fictício (ex.: código "ALVORADA" e PIN 1234), dito em voz alta.
7. **Códigos BNCC:** foram sugeridos pelo ChatGPT e precisam ser conferidos na BNCC oficial antes de aparecerem em slide (matemática: EF04MA06, EF04MA07, EF05MA03, EF05MA04, EF06MA07, EF06MA09, EF06MA10, EF07MA13; português: EF15LP03, EF35LP12, EF67LP28, EF69LP29, EF67LP32, EF67LP33, EF06LP06).
8. **Data da prova de português (19/11):** foi inventada para a aba Provas do aluno e coincide com a prova de decimais do 6º C. Está ok?
9. **Quem fala o quê na apresentação:** a definir pelo Gabriel no roteiro.
