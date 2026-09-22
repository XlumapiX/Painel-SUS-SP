# Como o projeto foi pensado

Esta página explica o raciocínio por trás do painel: o problema que ele tenta resolver,
as escolhas que foram feitas e por quê. A ideia é que quem ler consiga discordar, sugerir
e pensar em melhorias.

---

## 1. O problema

A prova de residência do SUS-SP tem **100 questões, 20 de cada grande área**: Clínica Médica,
Cirurgia, Pediatria, Ginecologia e Obstetrícia e Medicina Preventiva.

O tempo de preparação é curto, cerca de dez semanas, e não dá para estudar tudo com a mesma
profundidade. Então o painel tenta responder a três perguntas:

1. **O que estudar primeiro?** O que a prova mais cobra.
2. **Como estudar?** Resolvendo questões, no formato da prova.
3. **O que revisar?** O que a pessoa mais erra, e não o que ela já sabe.

---

## 2. De onde vêm as prioridades

Foram analisadas **1.500 questões** de provas anteriores: SUS-SP, UNESP e FAMEMA, de 2022 a 2026.
Cada questão foi classificada, uma a uma, por área, tema e subtema, e os gabaritos foram conferidos
com as grades oficiais de cada prova (1.500 de 1.500).

Duas medidas definem o peso de um tema:
- **Tamanho:** quantas questões o tema teve.
- **Recorrência:** em quantos anos o assunto caiu.

**Um cuidado importante: agrupar antes de contar.** Assuntos que são a mesma coisa aparecem com nomes
diferentes. Exemplo: "anemia falciforme", "sequestro esplênico", "síndrome torácica aguda" e
"crise aplástica" são todos doença falciforme. Contados separados, cada um parece ter caído em
poucos anos. Contados juntos, o assunto caiu em quase todas as provas e vira um dos mais importantes
da Pediatria.

A nota de prioridade de cada tema combina as duas medidas:

```
prioridade = 10 × (questões do tema ÷ questões do maior tema da área)
           +  3 × (anos em que o assunto principal caiu)
```

A primeira parte premia os temas grandes. A segunda premia o que cai todo ano.

---

## 3. A semana

| Dia | O quê |
|---|---|
| Segunda | Clínica Médica |
| Terça | Cirurgia |
| Quarta | Pediatria |
| Quinta | Ginecologia e Obstetrícia |
| Sexta | Medicina Preventiva |
| Sábado | Prova completa, cronometrada |
| Domingo | Correção da prova e revisão da semana |

**Por quê:** as cinco áreas aparecem toda semana (a prova cobra as cinco por igual), o ritmo é
previsível e o sábado treina a resistência de uma prova inteira.

---

## 4. O dia

- **Dois temas novos por dia**, na ordem de prioridade.
- Para cada tema, uma lista de questões **filtrada pelo tema, e não pelo subtema**. Filtrar por um
  subtema muito específico esgota as questões disponíveis, e a plataforma completa a lista com
  questões fora do nível da prova. O subtema aparece no painel como **alvo**: o que prestar mais
  atenção dentro daquele tema.
- No fim, o **placar** do tema: quantas acertou de quantas.

---

## 5. A revisão tem vagas fixas

A ideia mais comum seria rever cada tema uma semana depois e de novo três semanas depois. A conta não
fecha: com 10 temas novos por semana, seriam 20 revisões por semana, e a lista de atrasados cresceria
sem parar (cerca de 30 temas atrasados já na terceira semana).

**A solução:** a revisão tem **duas vagas por dia**, e quem ocupa essas vagas são os temas com o
**pior acerto medido**. Assim, o tempo de revisão vai sempre para onde há mais erro. A memória de
longo prazo fica com os flashcards (o Anki faz esse espaçamento sozinho).

---

## 6. Cada erro é registrado, e o tipo de erro importa

Para cada questão errada, o painel registra:
- **o que a questão pedia** e **qual era a resposta certa**;
- **por que errou:** não sabia o conteúdo · sabia a doença, mas errou a conduta · confundiu duas coisas
  parecidas · errou um número (dose, valor de corte) · leu errado · sabia uma versão antiga da diretriz;
- **como chegou na resposta:** tinha certeza · estava em dúvida · chutou. Acertar no chute conta
  como erro.

**Por quê:** cada tipo de erro pede um remédio diferente.

| Se o erro mais comum é… | O remédio é… |
|---|---|
| Leitura | Treinar enunciado com tempo, e não estudar mais conteúdo |
| Confusão entre duas coisas | Tabela comparativa, e não reler a apostila |
| Errar tendo certeza | Revisar a fonte, porque algo foi aprendido errado |

Questões acima do nível da prova e listas de temas variados são registradas, mas **não entram na
estatística por tema**, para não distorcer a fila de revisão.

---

## 7. Flashcards só dos próprios erros

Em vez de baralhos prontos, com milhares de cartões genéricos, os flashcards nascem **só das questões
erradas**:
- **frente:** o que a questão pedia;
- **verso:** a resposta certa.

Antes de entrar no baralho, **cada cartão é conferido** em livros de referência e, quando preciso,
em diretrizes oficiais atualizadas. Essa conferência já pegou anotações com dose errada, que teriam
virado um cartão errado.

**Por quê:** poucos cartões, todos relevantes, todos corretos.

---

## 8. O dossiê: como a prova cobra cada tema

Para cada tema, o painel tem um resumo feito a partir da análise das questões: o que caiu em cada
ano, os subtemas que se repetem, as pegadinhas e as "pistas" (quando aparece X no enunciado, a
resposta costuma ser Y). No cronograma, o botão **⌄** abre o dossiê do tema do dia.

---

## 9. Os dados não podem se perder

Numa versão antiga, o painel apagou registros sem querer: ao abrir a página, ele gravava uma cópia
vazia do dia por cima dos dados verdadeiros. A correção virou regra de projeto:

- cada questão registrada é guardada **separada**, e nada que se grave depois consegue apagá-la;
- **apagar não apaga:** o registro vai para uma lixeira e pode voltar;
- toda edição **guarda a versão anterior**;
- se a internet cair, o registro fica no aparelho e é enviado depois;
- há um botão de **backup completo**.

Cada versão nova do painel passa por testes automáticos que simulam internet lenta, internet caída
e dois aparelhos ao mesmo tempo, antes de ser publicada.

---

## 10. O que não está aqui

- Os livros e o material de estudo usados como referência, protegidos por direitos autorais.
- As provas em PDF e o banco de questões classificadas.
- Dados pessoais e de desempenho.

---

## 11. Perguntas em aberto

Algumas decisões ainda estão em definição, e ideias são bem-vindas:

- Quantas questões de revisão por dia são o ideal?
- Como medir, de forma simples, se o desempenho está melhorando de uma semana para a outra?
- O que mais o painel poderia mostrar para ajudar a decidir o que estudar?

Sugestões: aba **Issues**, aqui no GitHub, ou mensagem direta.
