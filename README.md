# Pong

Trabalho realizado por:
- Gabriel Lima / 27935
- João Melo / 29940
- Henrique Brás / 27932

Desenvolvido na framework: [MonoGame](https://monogame.net/)

Repositório original: [Pong](https://github.com/ChrisChou-freeman/PongMonoGameExample)

Ficheiros que iremos documentar: 

1. Pasta Content
2. Pasta Lib
3. Game.cs
4. Program.cs
   

![Pong00](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExZmk1NTZ3ZHVjY3VreHl2aHRsamZ1eW91ZXBkYjJhOTYwY3lscDR5NiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/aTGwuEFyg6d8c/giphy.gif)

 
## Pasta Content

### Imagens:

• `Background.png`: Esta imagem é usada para representar o campo de jogo e tem a resolução de 800x480.

• `Ball.png`: É usada para representar a bola durante o jogo e tem a resolução de 16x16.

• `Bat.png`: Esta imagem representa a raquete do jogador e tem a resolução de 16x100.

### Sons:
• `Pong.wav`: Este som é usado quando a bola bate na raquete.

 ### Outros:

• `Content.mgcb`: Este arquivo é usado no desenvolvimento de jogos Monogame para gerenciar e compilar ativos de conteúdo, como texturas e sons, para o jogo.

• `Font.spritefont`: Define as características visuais de uma fonte usada no jogo, como estilo, tamanho e cor.

• `MenuFont.spritefont`: Especifica as propriedades visuais de uma fonte específica destinada a ser usada nos menus do jogo.

• `TimerFont.spritefont`: Define as características visuais de uma fonte usada para exibir o cronômetro dentro do jogo.


## Pasta Lib

 Esta pasta tem as classes principais para o funcionamento do jogo.

• `Ball.cs`: Está responsavel por representar a bola durante o jogo e controlar o seu comportamento como a fisica da bola , a sua velocidade , posição e direção.

• `Bat.cs`: Representa as duas raquetes durante o jogo e controla a as suas posições, a sua velocidade e a sua colisão com a bola.

• `FrameCounter.cs`: Conta o tempo, os frames e determina a média de frames por segundo, tal como os frames por segundo atuais.

• `Input.cs`: Define a classe Keys Up e Keys Down que são os inputs que controlam o movimento das raquetes.

• `Menu.cs`: Representa o menu principal antes do próprio jogo começar e permite escolher se quer jogar com 2 jogadores ou contra o computador.

• `PongSprite.cs`: É usada para apresentar na tela os sprites incluindo o incluindo o tempo de jogo, a pontuação, as raquetes e a bola.

• `Score.cs`: Toma conta dos pontos marcados por ambos os jogadores e dos sprites para a respetiva pontuação.

• `Timer.cs`: Apresenta o tempo restante tal como os sprites para o representar.


## Game.cs

É a principal do jogo Pong, desenvolvido utilizando a biblioteca MonoGame. Ela controla a lógica do jogo, incluindo inicialização, carregamento de conteúdo, atualização e renderização dos elementos do jogo.

### Funcionalidades Principais

- Início do Jogo: A classe gere a inicialização do jogo, configurando o tamanho do ecrã e outros parâmetros importantes.
- Carregamento de Conteúdo: Carrega os recursos necessários para o jogo, como texturas, fontes e sons.
- Atualização do Jogo: Atualiza o estado do jogo a cada fotograma, incluindo a lógica do jogo e interações do utilizador.
- Renderização do Jogo: Renderiza os elementos do jogo no ecrã, incluindo sprites, pontuações e cronómetros.

### Componentes Principais

- `GraphicsDeviceManager`: Gerencia as configurações gráficas do dispositivo.
- `SpriteBatch`: Utilizado para renderizar sprites no ecrã.
- `Score`: Controla e exibe a pontuação do jogo.
- `GamingTimer`: Cronómetro utilizado no jogo.
- `Menu`: Gerencia e exibe menus interativos.
- `FrameCounter`: Conta e exibe o número de fotogramas por segundo.
- `Bat` e `Ball`: Representações dos objetos do jogo, como as raquetes e a bola.

### Funções Principais

- `InitializeScreenSize`: Inicializa o tamanho do ecrã do jogo.
- `LoadContent`: Carrega os recursos gráficos e de áudio necessários para o jogo.
- `Update`: Atualiza o estado do jogo a cada fotograma.
- `Draw`: Renderiza os elementos do jogo no ecrã.

## Program.cs

O ficheiro `Program.cs` contém a classe principal `Program`, que serve como ponto de entrada do programa MonoPong.

## Funcionalidades Principais

- Função Main: O método `Main()` é o ponto de entrada do programa. Ele cria uma instância da classe `Pong`, que representa o jogo MonoPong, e a executa chamando o método `Run()`.

- Atributo STAThread: O atributo `[STAThread]` indica que a thread de aplicativo COM será apartada para processamento de mensagens. Isso é comum em aplicativos GUI do Windows para garantir a compatibilidade com certas APIs do Windows.

- Usando a Declaração: O uso da declaração `using` garante que o objeto `game` seja descartado corretamente após a execução do bloco de código, garantindo a liberação de recursos.

Este código é responsável por iniciar o jogo MonoPong e controlar o fluxo de execução do programa.


## Conclusão

Para resumir o projeto MonoPong é um exemplo de desenvolvimento que usa a framework do MonoGame, é um projeto simples mas bem executado e aberto a exploração e contributos pela comunidade.



