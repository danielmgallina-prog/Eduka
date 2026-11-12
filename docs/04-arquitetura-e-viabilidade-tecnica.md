# Eduka – Arquitetura e viabilidade técnica

Oct 29, 2026 · @Metropole · Equipe Abençoados f.c

## Resumo em 30 segundos

O Eduka é construível hoje, com tecnologia comum de mercado, por uma equipe pequena: um MVP para uma escola-piloto cabe em cerca de 4 meses.

Frase para o pitch: *"O Eduka tem três partes. O app do aluno, o painel do professor e um motor que conhece o mapa da BNCC: ele sabe que regra de três depende de frações, e frações dependem de multiplicação. Cada resposta do aluno, no app ou na prova da escola, atualiza o quanto ele domina cada habilidade. Quando ele trava, o motor desce pelo mapa até achar a origem do problema e monta a trilha a partir dali. Nenhuma caixa-preta: o professor sempre vê o motivo de cada indicação e pode discordar."*

Três ideias que sustentam a viabilidade:

- **Não depende de integração.** As notas entram por planilha, que toda escola já tem. Integração com sistemas da escola vem depois, como melhoria.
- **O motor é explicável.** Usa regras e um modelo estatístico clássico de aprendizagem, não uma IA que decide sozinha sobre a criança.
- **Privacidade desde o desenho.** Cadastro mínimo, cada escola isolada das outras, cada professor vê só as próprias turmas e todo acesso fica registrado.

## Stack escolhida e por quê

A regra foi escolher tecnologias populares, gratuitas e com muita gente no mercado para manter, usando uma linguagem só (TypeScript) em quase tudo e Python apenas no motor.

| Camada | Tecnologia | Por quê |
| --- | --- | --- |
| App do aluno | React Native com Expo | Um código só para Android e iOS; roda em celular simples; guarda exercícios para usar sem internet. Versão web para o laboratório da escola. |
| Painel do professor e da gestão | React com Next.js | Responsivo: o professor usa no celular, a gestão no computador. Mesmo kit de componentes do design. |
| API | Node.js com NestJS (TypeScript) | Organizada em módulos (turmas, provas, reforços, importação); validação e permissões em um lugar só. |
| Motor de trilhas | Python com FastAPI | Melhor ecossistema para estatística de aprendizagem; serviço separado que a API chama. |
| Banco de dados | PostgreSQL | Relacional, gratuito, maduro; isola cada escola com segurança por linha (Row-Level Security). |
| Fila e cache | Redis | Importações de planilha e recálculo de trilhas rodam em segundo plano, sem travar a tela. |
| Arquivos | Armazenamento de objetos (padrão S3) | Planilhas importadas e PDFs de relatório, criptografados. |
| Login | Professor: e-mail ou conta Google/Microsoft da escola, com verificação em duas etapas. Aluno: código da escola ou QR Code + PIN | Criança não precisa de e-mail nem de rede social. |
| Hospedagem | Containers Docker em nuvem com região no Brasil (São Paulo) | Dados ficam no país; escala conforme o número de escolas. |
| Monitoramento | Logs centralizados e painéis de métricas (ex.: Grafana) | Saber antes da escola quando algo cai ou fica lento. |
| Entrega contínua | GitHub com testes automáticos a cada mudança | Atualização sem parar o uso em sala. |
