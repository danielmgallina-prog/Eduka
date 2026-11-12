# Desafio 2 – Aprender no tempo certo

Hackathon Unicesumar · Oct 28, 2026 · @Metropole

## A dor

A informação sobre o aprendizado existe, mas não chega como ação ao aluno certo, no momento certo.

Todos os anos, milhares de alunos passam de série sem dominar o básico de leitura e matemática. A lacuna não some: ela se acumula. Quem não entendeu frações no 6º ano trava em regra de três no 7º, em porcentagem no 8º e chega ao ensino médio, e depois à faculdade, carregando dificuldades que deveriam ter sido resolvidas anos antes.

As escolas já avaliam: aplicam provas, lançam notas e acompanham boletins. O problema é que esses resultados raramente viram ação em sala. A nota mostra que o aluno foi mal, mas não mostra onde ele travou nem o que fazer a seguir.

Do outro lado está o professor, com muitas turmas, muitos alunos e pouco tempo. Na prática, ele não consegue analisar prova por prova para descobrir quem precisa de reforço, em qual conteúdo e por onde começar. O resultado é um reforço genérico, tardio ou que simplesmente não acontece.

**Quem sente a dor:**

- **Aluno:** avança sem base, acumula dificuldade e perde a confiança.
- **Professor:** sabe que parte da turma está defasada, mas não tem tempo nem ferramenta para saber quem e em quê.
- **Escola e secretaria de educação:** investem em avaliações cujos resultados não se transformam em melhora mensurável.

## Dados e fatos

Os números oficiais mostram que a defasagem começa cedo e chega intacta ao fim da educação básica.

| Indicador | Dado | Fonte |
| --- | --- | --- |
| Alfabetização ao final do 2º ano do EF (2025) | Apenas 66% das crianças alfabetizadas, ou seja, cerca de 1 em cada 3 avançou sem ler e escrever adequadamente | Inep/MEC, Indicador Criança Alfabetizada (mar/2026) |
| Matemática no 3º ano do EM, rede pública (Saeb 2025) | Média de 268 pontos, numa escala de 0 a 500 | Inep |
| Conteúdos básicos ao fim do EM | Na média, os alunos terminam o ensino médio sem dominar regra de três e gráfico de pizza, conteúdos do ensino fundamental | Folha de S.Paulo (ago/2026) |

**O que esses dados mostram:**

- A defasagem começa nos anos iniciais, atravessa os anos finais do fundamental sem ser corrigida e aparece no fim do ensino médio.
- Os **anos finais (6º ao 9º ano)** são a última janela antes de a lacuna se consolidar, por isso são o foco da nossa solução.
- O problema não é falta de avaliação: é falta de um caminho entre o resultado da prova e a ação de reforço.

## Objetivo

Criar uma solução que ajude **escolas e professores** a identificar quais alunos precisam de reforço, em quais conteúdos, e a organizar esse apoio **com os recursos que já têm**.

1. **Identificar** quais alunos precisam de reforço.
2. **Descobrir** em quais conteúdos e habilidades da BNCC cada um tem lacunas.
3. **Organizar** o apoio de forma prática, usando as provas, as notas e os professores que a escola já tem.
4. **Medir** a evolução de cada aluno, turma e escola, com relatórios prontos para a secretaria de educação.

**Nossa resposta:** um app de aprendizagem gamificado, contratado pela escola, para alunos do 6º ao 9º ano em Matemática e Língua Portuguesa. Ele cria uma trilha personalizada para cada aluno a partir das lacunas reais dele e entrega ao professor e à secretaria relatórios de quem precisa de reforço e em quê.

## Perguntas e respostas

**Pergunta-guia do desafio:** como transformar os resultados de notas e avaliações em ações de reforço que cheguem ao aluno certo, no momento certo?

**Resposta:** ligando a prova que a escola já aplica a uma trilha de estudo individual. Cada questão é associada a uma habilidade da BNCC; o erro do aluno vira um ponto de partida na trilha dele; o professor recebe o diagnóstico pronto; e uma nova avaliação mede se o reforço funcionou. O ciclo é: nivelamento → relatório → integração com as notas → trilha personalizada → nova avaliação.

### 1. Quem precisa de reforço?

No primeiro acesso, o aluno faz um **nivelamento no app**. Em seguida, o sistema cruza esse resultado com as **notas e provas corrigidas** do sistema de gestão escolar (diário de classe digital). O professor recebe um painel com os alunos já agrupados por lacuna, sem precisar analisar prova por prova.

### 2. Em quê, exatamente?

O sistema usa três camadas de dados:

- **Notas por matéria:** mostram onde olhar primeiro.
- **Acerto e erro por questão:** cada questão é ligada a uma habilidade da BNCC.
- **Diagnóstico no app:** desce pelos pré-requisitos até achar onde o aluno realmente trava. Exemplo: errou regra de três, o app testa frações; errou frações, testa multiplicação.

Além disso, o app identifica o **tipo de erro**. Quem responde 3/4 + 1/2 = 4/6 está somando numeradores e denominadores, um erro conceitual, e recebe uma explicação específica para ele.

### 3. Por onde começar?

Pela **lacuna de origem**, e não pelo conteúdo da série. A trilha segue o mapa de pré-requisitos da BNCC: o aluno do 8º ano que trava em frações começa em frações. A metodologia é uma só; o que se personaliza é o caminho de cada aluno: o quê, em que ordem e em que ritmo.

### 4. Quando?

**No mesmo dia e antes da prova.** O nivelamento já libera uma trilha provisória, para o aluno não ficar parado enquanto os dados da escola chegam. Quando o professor informa o conteúdo que vai cair na prova, o app gera uma **trilha de revisão pré-prova**. A repetição espaçada traz de volta o que o aluno está prestes a esquecer. O reforço acontece antes da nota baixa, e não depois.

### 5. Como fazer o aluno querer estudar?

Com uma experiência **100% gamificada**, no estilo Duolingo, mas com identidade própria:

- XP, níveis, sequência de dias (streak) e conquistas.
- **Ligas** de cerca de 20 alunos de nível parecido, sem ranking público da sala inteira.
- **Clãs cooperativos:** a turma é o clã e cumpre missões juntas. Exemplo: se 80% do 7ºB completar a trilha de frações, a turma sobe de nível.
- **Monitoria como recompensa:** quem domina uma habilidade vira monitor dela, com certificado e horas complementares.
- O sistema recompensa **progresso e domínio**, nunca volume de exercícios, para evitar pontos no chute.

### 6. Como ajudar o professor sem aumentar o trabalho dele?

A visão do professor é **totalmente relatorial**. O painel da turma mostra quem precisa de reforço e em quê, quem está evoluindo, quem parou de usar o app e uma **sugestão de ação para a aula**. O professor não monta trilha nem corrige exercício: o app faz isso, e ele decide como agir.

### 7. Como saber se funcionou?

Cada nova avaliação **mede a evolução** e realimenta o ciclo. A escola e a secretaria de educação recebem um relatório consolidado por série, por habilidade da BNCC e por evolução. As turmas são comparadas por **evolução e participação**, nunca por nota absoluta, para não punir a turma que começou mais fraca.

### 8. Como funciona com os recursos que a escola já tem?

O app usa **as provas que a escola já aplica**, as notas que já estão no sistema de gestão escolar e os professores que já estão em sala. Os próprios alunos que dominam uma habilidade viram monitores dos colegas. Os benefícios oferecidos são de custo zero, como ponto de participação, escolha de dupla e prioridade em atividades.

### 9. E a segurança dos dados dos alunos?

O sistema segue a **LGPD**. A contratação é feita pela escola, com consentimento dos responsáveis. Não há exposição pública individual, e a secretaria recebe dados agregados.

### 10. Quem paga?

A **escola contrata**. Na rede particular, a contratação é direta, com cobrança por aluno. Na rede pública, a contratação é pela secretaria de educação, via licitação. Prêmios externos, como gift cards ou intercâmbio, ficam como **sugestão de parceria** com governo, programas existentes e empresas locais, fora do custo do sistema.
