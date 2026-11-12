# Eduka

**Reforço escolar gamificado em matemática e português para o 6º ao 9º ano, contratado pela escola.**

Projeto da equipe **Abençoados f.c** (Daniel, Gabriel, Lucas e Mateus) no **Hackathon UniCesumar e Elotech 2026**, Desafio 2: *"Aprender no tempo certo"* (28 a 30/10/2026).

## A ideia em uma frase

> A escola já aplica a prova; o Eduka mostra qual peça falta e leva o reforço certo para o aluno certo.

Cada questão da prova que a escola já aplica é ligada a uma habilidade da BNCC. O sistema desce pelo mapa de pré-requisitos até achar a **origem da lacuna** (o aluno erra regra de três porque trava em frações, conteúdo de dois anos antes), monta para o aluno uma **trilha que começa nessa lacuna** e entrega ao professor **grupos de reforço com sugestão para a próxima aula**.

## Como funciona

1. **Escola** importa turmas, alunos e professores e libera o nivelamento.
2. **Aluno** faz o nivelamento no app; o sistema acha o ponto de partida e monta a trilha.
3. **Professor** cadastra a prova e publica a trilha de revisão.
4. **Aluno** faz a revisão antes da prova.
5. **Professor** importa os resultados por questão; o sistema atualiza as lacunas.
6. A trilha se ajusta e o professor vê os grupos que precisam de reforço.
7. O professor registra o reforço feito em sala; a próxima prova mede o resultado.

## Os três públicos

| Perfil | O que faz |
| --- | --- |
| Aluno (app lúdico, com o mascote Kadu) | Nivelamento, trilha, exercícios com dica no erro, missão do clã da turma |
| Professor (painel sóbrio) | Grupos de reforço, ficha do aluno, provas, importação de resultados, relatório |
| Escola / gestão | Implantação, cadastro e acessos, currículo, privacidade |

## Estrutura do repositório

```
docs/            todos os documentos do projeto, em ordem cronológica (01 a 13)
design-system/   identidade visual: guia (README), tokens.json e componentes
prototipos/      páginas HTML: apresentação web da final, protótipo funcional e painel de entregas
DECISOES.md      as decisões de produto e o porquê de cada uma
HISTORICO.md     o que foi feito, dia a dia
```

Os protótipos abrem direto no navegador (duplo clique no `.html`).

## Material original

Todo o material foi produzido como artefatos e documentos no Claude. Os links abaixo são privados (abrem só para quem tem acesso).

| Material | Onde está aqui |
| --- | --- |
| Guia de marca / Design System Eduka | `design-system/` |
| Interface (canvas com 59 telas e modo Play) | só no link original |
| Apresentação (deck da classificatória) | só no link original; roteiros em `docs/06` e `docs/10` |
| Apresentação web "Jornada da Ana" (final) | `prototipos/apresentacao-web-jornada-da-ana.html` |
| Protótipo funcional | `prototipos/prototipo-funcional.html` |
| Painel de entregas da equipe | `prototipos/painel-de-entregas.html` |

## Dados

Todas as pessoas, escolas e números de alunos nos protótipos são **fictícios**, como exige o regulamento (art. 9º). A pesquisa com 14 professores foi anônima.
