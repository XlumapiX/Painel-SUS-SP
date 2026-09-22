# Caderno de Bordo SUS-SP

Um painel para organizar os estudos para a prova de residência médica do **SUS-SP**.
Ele mostra o que estudar em cada dia, registra os erros e aponta os temas que mais precisam de revisão.

**Para abrir o painel: https://xlumapix.github.io/Painel-SUS-SP/**
Funciona no computador e no celular, direto no navegador.

**Para entender o raciocínio por trás dele:** [Como o projeto foi pensado](COMO-FOI-PENSADO.md).

> **Esta é uma versão de demonstração.** Você pode testar tudo à vontade.
> O que você registrar fica salvo só no seu navegador e não afeta o painel original.
> Para apagar os seus testes, use o botão **Limpar demonstração**, no topo do painel.

## A ideia

A prova tem 100 questões, 20 de cada grande área. O painel foi montado a partir da análise de
**1.500 questões** de provas anteriores (SUS-SP, UNESP e FAMEMA, de 2022 a 2026), para priorizar
o que realmente cai.

- **Uma área por dia:** segunda Clínica Médica, terça Cirurgia, quarta Pediatria, quinta Ginecologia
  e Obstetrícia, sexta Preventiva. Sábado é dia de prova completa e domingo de revisão da semana.
- **Dois temas por dia,** escolhidos pelo peso que têm na prova.
- **Cada questão errada é registrada:** o que a questão pedia e qual era a resposta certa.
  Esses registros viram flashcards para revisar depois.
- **Os temas com pior desempenho voltam** para revisão na semana seguinte.

## As abas

| Aba | Para que serve |
|---|---|
| **Hoje** | Os temas do dia, o placar de acertos, o registro de questões erradas e a lista de tarefas |
| **Cronograma** | O plano completo, semana a semana, com o que estudar em cada tema |
| **Progresso** | Percentual de acertos, temas que precisam de revisão e histórico dos erros |
| **Peso** | Quantas vezes cada tema caiu nas provas anteriores |

Na lista de tarefas, toque numa linha para marcá-la como feita. O botão **⌄** mostra como a
prova costuma cobrar aquele tema.

## Arquivos

| Arquivo | O que é |
|---|---|
| `index.html` | O painel |
| `crono.js` | O cronograma, dia a dia |
| `dossie.js` | Como a prova cobra cada tema |
| `temas.js` | Quantas questões cada tema teve |
| `gab.js` | Gabaritos oficiais das provas |
| `COMO-FOI-PENSADO.md` | O raciocínio por trás do painel |

Os livros e o material de estudo usados na preparação não estão aqui, porque são protegidos por
direitos autorais.

## Sugestões

Ideias são bem-vindas: use a aba **Issues** aqui do GitHub (**New issue**) ou mande uma mensagem direto.
