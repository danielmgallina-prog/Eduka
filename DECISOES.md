# Decisões do Eduka

O que a equipe decidiu e por quê. Detalhes em `docs/`.

## Escopo
- **6º ao 9º ano, matemática e português.** É a última janela antes de a lacuna se consolidar no ensino médio, e são as áreas apontadas pelos dados do desafio (Saeb, alfabetização).
- **Parte das provas que a escola já aplica**, não de conteúdo genérico. É o que diferencia do Duolingo e do Khan Academy.
- **Começa pela lacuna de origem**, não pelo conteúdo da série.
- **De chatbot no WhatsApp para app próprio.** O WhatsApp limitava os exercícios e o acompanhamento do professor.

## Ninguém é exposto
- **Sem ranking individual.** O desafio pede que nenhuma solução exponha ou rotule o aluno; ranking deixa sempre alguém em último, justamente quem tem lacuna.
- **Gamificação só coletiva:** a turma é um clã e o inimigo é a lacuna (o "chefão da turma"). Cada acerto de qualquer aluno é um golpe.
- **Professor vê domínio por habilidade em %, nunca nota, XP ou ranking.** Listas sempre em ordem alfabética.
- **Escola não vê desempenho pedagógico**, só cadastro, uso agregado e implantação.
- **Pontos só sobem.** Errar vale zero, nunca negativo. Quebrar a sequência não tira nada.
- **Limite de 60 golpes por aluno por dia**, para três alunos não carregarem o clã.

## Gamificação
- **Rodadas de 8 exercícios (~3 min)**, chefão por fases, baú, missões do dia, sequência com escudo, cartas de revisão (1, 3, 7 e 14 dias), minijogos de 60 s.
- **Baú sem nenhum caminho de pagamento:** nada se compra, sem moeda, sem troca; abre 3 itens e o aluno escolhe 1, com as probabilidades na tela. O ECA Digital proíbe caixa de recompensa paga. O nome é sempre "baú", nunca "lootbox".
- **No erro, dica e nova tentativa** antes da resposta, valendo os mesmos pontos.
- **A lacuna só fecha quando o aluno acerta de novo dias depois** e a prova da escola confirma.

## Mascote e marca
- **Kadu**, cabeça de coelho branca flutuante, sem boca; as orelhas formam o K de "eduka". A peça laranja ao lado é a lacuna.
- **Expressão só nos olhos e orelhas.** No máximo um Kadu por tela, só no app do aluno, nunca triste nem bravo.
- **Violeta** como cor principal, **laranja** só para recompensa. Fredoka nos títulos do aluno, Lexend no texto (feita para facilitar a leitura).
- **Dois registros da mesma marca:** aluno lúdico, professor sóbrio (80% neutro, sem sombra).

## IA
- **A IA trabalha para o professor e nunca decide sobre a criança.** Ela sugere a habilidade BNCC de cada questão e gera dicas; tudo aparece como "sugestão: confirme".
- **Nenhum nome, nota ou resposta de aluno vai para a IA.**
- **O motor da trilha é por regras e modelo estatístico simples**, explicável, sem IA generativa decidindo.
- **Gemini ficou fora:** os termos da API proíbem apps usados por menores de 18. Protótipo com Groq; produção com modelo aberto em servidor no Brasil.

## Negócio
- **Quem paga é a escola ou a rede; aluno e família nunca.**
- Classificatória: hipótese de R$ 90–110/aluno/ano (particular) e R$ 55–75 (pública), mínimo ~R$ 10 mil por escola.
- **Final:** modelo revisado para **gratuito na escola pública**; privada assina (hipótese de R$ 4 a 6 por aluno/mês) e paga por acompanhamento dedicado; serviços de gestão para secretarias e parceiros de impacto sustentam o gratuito. Valores são hipóteses a validar em piloto.

## Tecnologia proposta
- App do aluno em React Native (Expo) com versão web; painel em Next.js; API em NestJS; motor em Python/FastAPI; PostgreSQL com isolamento por escola; Redis; Docker em nuvem em São Paulo.
- **Sem integração obrigatória:** tudo entra por planilha; prova em papel funciona.
- **MVP em ~12 semanas** com 4 a 6 pessoas, terminando num piloto de um bimestre.

## Privacidade (LGPD e ECA Digital)
- Cadastro mínimo: nome, identificador escolar, turma, ano de nascimento. Nunca saúde, renda, foto ou localização.
- Cada escola isolada, cada professor vê só as próprias turmas, todo acesso registrado.
- No hackathon, só dados fictícios (art. 9º).
