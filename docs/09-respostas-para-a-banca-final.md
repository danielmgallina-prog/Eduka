# Eduka · Respostas para a banca (final)

Oct 30, 2026 · @Metropole

## Modelo comercial em quatro frases

O Eduka é gratuito para toda escola pública, com o núcleo pedagógico completo. A escola privada assina e paga por acompanhamento exclusivo, não por mais conteúdo. Assinaturas privadas, serviços de gestão para secretarias e parceiros de impacto sustentam o gratuito. O aluno e a família nunca pagam.

|  | Escola pública | Escola privada | Secretaria de educação |
| --- | --- | --- | --- |
| Preço | Gratuito | R$ 4 a 6 por aluno/mês (hipótese a validar) | Opcional, só serviços de gestão |
| Núcleo pedagógico | Completo | Completo | — |
| Suporte em problemas | Mesmo prazo para todos | Mesmo prazo para todos | Mesmo prazo para todos |
| Extra pago | — | Acompanhamento pedagógico dedicado, relatórios com a marca da escola, integração sob medida | Painel da rede, integração com o sistema de gestão escolar, formação presencial |
| Entrada | Implantação em grupo, a distância | Assinatura anual com 1º bimestre de garantia | Termo de cooperação e contrato de tratamento de dados |

Princípio para repetir: o público nunca recebe menos; o privado recebe atendimento exclusivo a mais.

## Perguntas comerciais

**"Como separam o preço entre pública e privada?"** A pública não paga: o núcleo é gratuito. A privada paga por serviço exclusivo, não por mais aprendizagem. Ninguém recebe versão pior.

**"Então quem paga a conta da escola pública?"** Três fontes: assinaturas privadas, serviços de gestão contratados pela secretaria (painel da rede, integração, formação) e parceiros de impacto, como fundações e editais de inovação. Há precedente: o Khan Academy chegou às escolas municipais de Manaus por parceria com a Fundação Lemann.

**"Por que uma escola privada assinaria?"** Recuperação mais barata e direcionada (a LDB já obriga a oferecer), resultado visível em avaliações e tempo do professor. O professor descobre em minutos quem precisa de reforço em quê.

**"Esse preço é real?"** É hipótese a validar com escolas. Como referência de mercado, o Rio Grande do Sul registrou plataforma de matemática a R$ 14,40 por aluno/ano.

**"O piloto gratuito não sai caro?"** Na privada não há piloto solto: é assinatura anual com o 1º bimestre de garantia. Só absorvemos custo de quem cancelar. Um bimestre pega um ciclo de prova, então a escola vê resultado.

**"O gratuito não vira mais um problema para a rede pública?"** O Eduka é desenhado para tirar trabalho: importação em vez de cadastro manual, formação curta, funciona no celular e com internet fraca. Se o professor gastar mais tempo do que economiza, o produto falhou.

**"Como vendem para governo?"** Implantação gratuita com termo de cooperação e contrato de tratamento de dados (LGPD). Serviços de gestão seguem as regras de compras públicas; uma ata de registro de preços permite que outras redes adiram, como Recife e Salvador fizeram na ata gaúcha de leitura.

**"E o Khan Academy, que é grátis?"** O Khan é ótimo conteúdo genérico. O Eduka parte das provas que a própria escola aplica e diz ao professor o que fazer na próxima aula.

## Perguntas sobre IA e dados

**"Vocês precisam treinar a IA?"** Não para começar. São três camadas:

1. Mapa de pré-requisitos da BNCC, montado por pessoas. É regra pedagógica e por isso explicável.
2. Estimativa de domínio por habilidade, com modelo estatístico simples que funciona com poucos dados. É ela que monta a trilha.
3. IA generativa já existente, sem treino próprio, para gerar a dica e a resolução passo a passo quando o aluno erra, e a sugestão ao professor. Dados vão sem nome do aluno.

Com os dados dos pilotos, ajustamos a estimativa e o banco de exercícios. A decisão é sempre do professor.

**"Como sabem que a lacuna foi resolvida?"** Cada exercício é uma medição. Um acerto isolado não fecha a lacuna: ela só fecha com acertos consistentes e espaçados no tempo, e a habilidade volta numa revisão curta se o aluno ficar sem praticar. Quando o professor importa a prova, ela confirma ou corrige o que o motor estimava. O aluno vê a própria evolução, sem comparação com colegas, e sai da fila de atenção do professor sem ninguém precisar marcar nada.

**"O que garante que o aluno aprende, e não só acerta?"** O erro vira ensino: o aluno recebe uma dica e tenta de novo; se errar outra vez, vê a resolução passo a passo. Essas dicas e resoluções são geradas pela IA generativa por tipo de erro e revisadas antes de entrar no ar, o que evita resposta inventada. A prova de que aprendeu é acertar de novo dias depois.

Frase para a final: "Cada exercício é uma medição. A lacuna só é dada como fechada quando o aluno acerta de novo, dias depois, e a prova da escola confirma."

**"E o volume de dados?"** O próprio uso gera os dados: nivelamento e exercícios diários. O banco inicial de questões vem de itens públicos (avaliações oficiais liberadas e olimpíadas) e das provas que o professor já aplica.

**"Como o desempenho do aluno chega ao sistema?"** Não é um CSV no fim do semestre, que chegaria tarde. Agora: o professor lança o resultado de cada prova em poucos minutos, por questão, e o mapeamento questão → habilidade fica salvo. Depois: integração direta com o diário e o sistema de gestão da escola. A maior parte dos dados vem do uso do aluno.

**"Quanto custa a IA por aluno?"** Pouco: a trilha não usa IA generativa, e cada dica é gerada uma vez por tipo de erro e reaproveitada para todos os alunos que cometem o mesmo erro. O custo real sai dos pilotos.

## Perguntas sobre engajamento e escopo

**"O que garante que o aluno vai querer usar?"** Ouvimos a banca: a gamificação fica mais forte, sempre coletiva e sem ranking individual. Exemplos: chefão da habilidade que a turma enfrenta junta, minijogos de 60 segundos, cartas de revisão que voltam em intervalos e o Kadu que evolui com a sequência de estudo do próprio aluno.

**"Baú com item aleatório não é lootbox? Isso é permitido para criança?"** O ECA Digital veda caixa de recompensa paga. O baú do Eduka não tem nenhum caminho de pagamento: nada se compra, não existe moeda, não há troca entre alunos. Ele abre revelando 3 itens e o aluno escolhe 1, com as probabilidades escritas na tela. É recompensa por prática, com escolha, não aposta.

**"E se só três alunos fizerem tudo pela turma?"** Cada aluno dá no máximo 60 golpes por dia, e exercícios de pré-requisito também contam. Assim quem tem lacuna é quem mais contribui, e ninguém carrega o clã sozinho.

**"O jogo não desvia o foco da aprendizagem?"** Toda mecânica tem razão pedagógica: a rodada é prática de recuperação, as cartas são repetição espaçada, os minijogos são intercalação, e o chefão só recebe golpe de exercício da trilha. A maior comemoração do app é "lacuna fechada", não ponto.

**"Por que não ranking individual?"** O desafio pede que nenhuma solução exponha ou rotule o aluno. Ranking deixa sempre alguém em último, justamente quem tem lacuna.

**"O que o professor vê?"** Quem precisa de reforço, em qual habilidade e uma sugestão para a próxima aula. Domínio em %, nunca ranking ou XP. A decisão é dele.

**"E a LGPD?"** Cadastro mínimo, sem dado de saúde ou social, consentimento por responsável, auditoria sempre ligada, relatório em PDF sem nomes e dados exportáveis pela escola.

## O que não dizer

- Não usar linguagem de evasão ("evitar que o aluno saia"): é tema do Desafio 1. Retorno da privada = recuperação, resultado e tempo do professor.
- Não dar números de custo por aluno como fechados: são hipóteses validadas nos pilotos.
- Não falar em "desconto de 60%": o modelo agora é público gratuito.
- Não prometer CSV no fim do semestre.
- Não dizer que vamos "treinar uma IA" do zero, nem a palavra "lootbox": é "baú", ganho por prática.

## Fontes

- [Governo do RS: atas de plataformas educacionais digitais (R$ 14,40 aluno/ano em matemática; adesões de Recife e Salvador)](https://estado.rs.gov.br/upload/arquivos/plataformas-educacionais-digitais.pdf)
- [Portal Amazônia: Khan Academy na rede municipal de Manaus, parceria com a Fundação Lemann](https://portalamazonia.com/educacao/plataforma-online-sera-usada-nas-aulas-de-matematica-da-rede-municipal-de-ensino-em-manaus/)
- [Contrato municipal de 2025 com trilhas personalizadas por habilidade (São Domingos do Norte, ES)](https://www.saodomingosdonorte.es.gov.br/uploads/contrato/contrato-51-anexo-0796bb19bf1ce3874edb4179e67b79eb.pdf)
