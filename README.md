## Jogo Flappy Bird em Python com Pygame

Este projeto recria o clássico jogo Flappy Bird usando a biblioteca Pygame para gráficos e interação com o usuário. O objetivo é controlar um pássaro, fazendo-o voar entre canos sem colidir.
Estrutura do Projeto

    imgs/: Pasta contendo as imagens do jogo (bird1.png, bird2.png, bird3.png, pipe.png, base.png, bg.png).
    flappy.py: Arquivo Python com o código do jogo.
    README.md: Este arquivo de documentação.

## Classes Principais

* `Passaro:`
  * Representa o pássaro controlado pelo jogador.
  
  * Controla a posição, velocidade, ângulo e animação do pássaro.
  
  * Métodos principais: pular(), mover(), desenhar(), get_mask().
  
* `Cano:`
  
  * Representa os canos que o pássaro deve evitar.
  
  * Controla a posição, altura e movimento dos canos.
  
  * Métodos principais: definir_altura(), mover(), desenhar(), colidir().
        
* `Chao:`
  
  * Representa o chão do jogo.
    
  * Controla o movimento do chão para simular o deslocamento do cenário.
    
  * Métodos principais: mover(), desenhar().

## Lógica do Jogo

   * O jogo inicia com um pássaro e um conjunto de canos.
   
   * O jogador controla o pássaro pressionando a barra de espaço para fazê-lo pular.
   
   * Os canos se movem da direita para a esquerda da tela.
   
   * O pássaro deve evitar colidir com os canos e o chão.
   
   * A cada par de canos que o pássaro passa, a pontuação aumenta.
   
   * O jogo termina quando o pássaro colide com um cano ou com o chão.

## Como Jogar

   * Certifique-se de ter as imagens do jogo na pasta imgs/.
   
   * Execute o script flappy.py.
   
   * Pressione a barra de espaço para fazer o pássaro pular.
   
   * Tente evitar os canos e o chão para aumentar sua pontuação.

## Observações

   * O jogo utiliza máscaras de colisão (pygame.mask) para detectar colisões entre o pássaro e os canos.
    
   * A animação do pássaro é feita alternando entre as três imagens (bird1.png, bird2.png, bird3.png).
    
   * A velocidade do jogo é controlada pelo relogio.tick(30), que define o número de quadros por segundo.
    
**Observação:** Este projeto é uma recriação do Flappy Bird para fins de aprendizado e diversão. Divirta-se jogando e explorando o código!
