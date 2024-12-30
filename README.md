# QuizIniciante

## Índice
- [Descrição](#descrição)
- [Desenvolvedores](#desenvolvedores)
- [Perguntas](#perguntas)
- [Como incluir a sua pergunta](#como-incluir-a-sua-pergunta)
- [Como jogar](#como-jogar)
- [Diagrama de Classes](#diagrama-de-classes)

---

## Descrição

O **QuizIniciante** é um modelo de quiz, desenvolvido sem o uso de banco de dados.
O projeto foi elaborado como parte da Unidade Curricular de **Programação de Soluções Computacionais** da UniBH e implementado utilizando a linguagem **Java**.

---

## Desenvolvedores

Este projeto foi desenvolvido por:

- [João Paulo Leão](https://github.com/Joutos)
- [Felipe Santos](https://github.com/FelipeDoismil)
- [Giovana Altair](https://github.com/GiovannaAltair)
- [Lucas Lopes](https://github.com/Lucaslopes47)

---

## Perguntas

As perguntas do quiz são gerenciadas automaticamente a partir do arquivo `perguntas.txt`, localizado no diretório raiz do repositório.

### Como incluir a sua pergunta

Para adicionar novas perguntas ao quiz, edite o arquivo `perguntas.txt`. Cada linha do arquivo representa uma pergunta no seguinte formato:

```
ID;Texto da pergunta;Resposta correta;Alternativa A;Alternativa B;Alternativa C;Alternativa D
```

#### Exemplo

Se você deseja adicionar a seguinte pergunta:

- **Pergunta:** Quanto é 2 + 2?
- **Resposta correta:** C
- **Alternativas:**
  - A - 6
  - B - 2
  - C - 4
  - D - 5

A linha correspondente no arquivo `perguntas.txt` deve ser:

```
1;Quanto é 2+2?;C;A - 6;B - 2;C - 4;D - 5
```

---

## Como jogar

Ao executar o programa, você será apresentado à tela inicial com três opções:

1. **Jogar**: Inicia o jogo.
2. **Desenvolvedores**: Exibe informações sobre os criadores do projeto.
3. **Sair**: Encerra o programa.

### Passo a passo do jogo

1. **Escolha dos jogadores**:
   - Cada jogador escolhe seu personagem. O nome escolhido será utilizado pelo programa para identificá-los durante o jogo.

2. **Exibição das perguntas**:
   - Em cada rodada, uma pergunta é exibida com suas alternativas.
   - Cada jogador escolhe a alternativa que considera correta.

3. **Confirmação das respostas**:
   - Após escolherem, os jogadores têm a opção de revisar suas respostas antes de confirmá-las.
   - Caso um jogador decida alterar sua resposta, ambos precisarão responder novamente.

4. **Avaliação das respostas**:
   - Se a resposta estiver errada, o jogador perde 45% da sua vida.
   - Quando a vida de um jogador chega a 0%, ele é eliminado e o outro jogador vence.

5. **Condição de empate**:
   - Caso todas as perguntas terminem, o jogador com maior vida restante é declarado vencedor.
   - Se ambos tiverem a mesma vida, o jogo termina em empate.

---

## Diagrama de Classes

Abaixo está o diagrama de classes que representa a estrutura do projeto:

![Diagrama de Classes](https://github.com/Joutos/QuizIniciante/blob/main/ClassDiagram.png)

---

