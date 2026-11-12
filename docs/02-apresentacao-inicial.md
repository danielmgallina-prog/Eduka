**Eduka: reforço escolar gamificado.**

Oct 28, 2026 · @Metropole

Hackathon 2026 · UniCesumar e Elotech · Desafio 2 – Aprender no tempo certo

## Contexto do desafio

**Dor:** muitos alunos passam de ano sem aprender o básico de leitura e matemática, e essa dificuldade vai junto para o ensino médio e para a faculdade. A escola aplica provas, mas a nota sozinha não mostra em que ponto o aluno deixou de entender. Com várias turmas, o professor não consegue analisar cada prova para saber quem precisa de reforço e em qual conteúdo.

**Dados e fatos:**

- Só 66% das crianças estavam alfabetizadas ao final do 2º ano do EF em 2025: cerca de 1 em cada 3 não estava (Inep/MEC, mar/2026).
- Média de 268 pontos, numa escala de 0 a 500, em matemática no 3º ano do EM da rede pública (Saeb 2025, Inep).
- Na média, os alunos terminam o EM sem dominar regra de três e gráfico de pizza (Folha de S.Paulo, ago/2026).

**Objetivo:** ajudar a escola e o professor a saber quais alunos precisam de reforço e em quais conteúdos, e organizar esse reforço com o que a escola já tem: provas, notas e professores.

**Pergunta-guia:** como transformar os resultados de notas e avaliações em ações de reforço que cheguem ao aluno certo, no momento certo?

**Nossa resposta:** cada questão da prova é ligada a uma habilidade da BNCC. Os erros do aluno definem por onde a trilha dele começa, o professor recebe um resumo da turma e a avaliação seguinte mostra se o reforço deu resultado.

## II – Breve explicação da solução proposta

O Eduka é um aplicativo de reforço escolar em Matemática e Língua Portuguesa para alunos do 6º ao 9º ano. A escola contrata o serviço, e cada aluno recebe uma trilha de exercícios montada a partir das próprias dificuldades. O professor e a secretaria de educação acompanham os resultados por relatórios.

- **Diagnóstico:** o aluno faz um teste de nivelamento no app, e o sistema cruza o resultado com as notas e provas lançadas no sistema de gestão escolar. Se o aluno erra regra de três, o app testa frações; se erra frações, testa multiplicação, até chegar à origem da dificuldade.
- **Trilha:** começa pelo conteúdo que ficou para trás, segue a ordem de pré-requisitos da BNCC e muda de ritmo conforme o aluno acerta ou erra. Antes das provas, entra uma revisão do conteúdo que vai ser cobrado.
- **Gamificação:** pontos, níveis, sequência de dias e ligas com alunos de nível parecido. A turma funciona como um clã com missões em conjunto, e quem domina um conteúdo pode ser monitor dos colegas. O app premia o avanço, e não a quantidade de exercícios feitos.
- **Professor e secretaria:** um painel mostra quem precisa de reforço e em quê, quem está evoluindo e quem parou de usar o app, com sugestões para a aula. A decisão continua sendo do professor.

Na demonstração usamos apenas dados fictícios. O projeto segue a LGPD: nenhum aluno é exposto ou ranqueado publicamente, e a secretaria recebe dados agregados.

## III – Como a equipe chegou à ideia

Começamos pela pergunta-guia e por uma constatação do grupo: a escola já tem as notas, mas elas não chegam ao aluno como ajuda concreta.

1. A primeira ideia foi um chatbot no WhatsApp que dava bônus para quem estudasse.
2. Na discussão, vimos que o WhatsApp limitava os exercícios e o acompanhamento do professor. Passamos para um aplicativo próprio, com a mecânica de jogo do Duolingo, conhecida por manter o hábito de estudo diário.
3. A diferença para o Duolingo é que o Eduka parte das provas da escola e segue a BNCC, em vez de uma sequência igual para todos.
4. Escolhemos o 6º ao 9º ano por ser a última etapa antes do ensino médio, e Matemática e Português por serem as áreas apontadas nos dados do desafio.
5. Para não expor quem tem mais dificuldade, as turmas são comparadas pela evolução e pela participação, nunca pela nota.
