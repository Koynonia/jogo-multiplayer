
<p align="center">
  <a href="https://www.youtube.com/watch?v=0sTfIZvjYJk&list=PLMdYygf53DP5SVQQrkKCVWDS0TwYLVitL&index=2">
    <img src="https://raw.githubusercontent.com/filipedeschamps/meu-primeiro-jogo-multiplayer/master/game-preview.gif" width="550">
  </a>
</p>

# jogo-multiplayer

Um jogo multiplayer simples o suficiente para qualquer pesssoa aprender conceitos importantes sobre **arquitetura** e **desenvolvimento de software**.

Ele foi projetado de uma forma modificável/hackeável para que você consiga implementar suas próprias idéias ou até reimplementar do zero em outras linguagens. Inclusive este é repositório é um **playground** de experimentos e qualquer tentativa será bem vinda.

Antes de prosseguir, é extremamente importante você assistir esse vídeo introdutório com toda explicação por trás deste projeto, inclusive todos os passos utilizados para programar ele: **[Assistir introdução no YouTube](https://www.youtube.com/watch?v=0sTfIZvjYJk&list=PLMdYygf53DP5SVQQrkKCVWDS0TwYLVitL&index=2)**

## Experimentos
| Autor | Descrição |
| :---: | :--- |
| <img src="https://avatars3.githubusercontent.com/u/4248081?s=460&v=4" width="170"> | **Prova de Conceito (POC) por [@filipedeschamps](https://github.com/filipedeschamps)**<br>Eu nunca tinha programado um jogo multiplayer e queria entender o que eu não entendia sobre o assunto para, em seguida, reimplementar um MVP com práticas melhores. Dessa experiência foi criada uma [Playlist no YouTube com 12 vídeos](https://www.youtube.com/playlist?list=PLMdYygf53DP5SVQQrkKCVWDS0TwYLVitL) sobre design pattern e arquitetura de software.<br>[Rodar no Gitpod](http://gitpod.io/#experiment=1st-proof-of-concept/https://github.com/filipedeschamps/meu-primeiro-jogo-multiplayer) / [Abrir código](https://github.com/filipedeschamps/meu-primeiro-jogo-multiplayer/tree/master/playground/1st-proof-of-concept) |
| <img src="https://avatars3.githubusercontent.com/u/1801285?s=460&v=4" width="170"> | **Estudo da implementação por [@koynonia](https://github.com/koynonia)**<br>Um estudo das tecnicas utilizadas para a programação deste jogo. |

Foi utilziado JavaScript + Node.js + Socket.io para programar o Frontend e Backend do jogo, separando suas diversas responsabilidades.

## Camadas


| Camadas | Descrição |
| :--- | :--- |
| Apresentação | É onde existe o contato com o jogo, mas é desprovida de toda funcionalidade. Como exemplo, podemos entendê-la como uma impressora que tem que receber um texto, visto que ela mesma não o produz. |
| Lógica + Dados | É onde são implementadas as funcionalidades de forma abstrata. Podemos entender como sendo nossa mente diante de um jogo de xadrez, que conhece todos os movimetos e regras possíveis. |
| Inputs | É a camada que recebe as entradas do teclado, que a camada de Lógica + Dados fazem uso para serem aplicadas. |
| Networking | Esta camada é uma das mais importante, pois é responsável por manter o sincronismo entre os diversos clients com o server. |

