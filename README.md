# Campo-Minado
Código em c# com o jogo Campo Minado 
(1) OBJETIVO DO PROGRAMA:
O objetivo do programa é implementar um jogo de Campo Minado, onde o jogador deve revelar todas as células que não contêm bombas. 
O jogo termina quando o jogador revela todas as células seguras ou quando acerta uma bomba.

(2) DETALHES DE IMPLEMENTAÇÃO - MÉTODOS DESENVOLVIDOS:
Main(string[] args): O método principal que inicia o jogo. Lê as informações do tabuleiro a partir de um arquivo de texto, inicializa o tabuleiro, 
preenche as bombas e os números das células adjacentes.
IniciarJogo(): Método responsável por iniciar o jogo. 
Ele cria o tabuleiro, preenche as bombas e os números, e entra em um loop até que o jogo termine.
PreencherBombas(): Método para posicionar as bombas de forma aleatória no tabuleiro.
PreencherNumeros(): Método para preencher a quantidade de bombas adjacentes em cada célula.
ImprimirTabuleiro(): Método para imprimir o tabuleiro completo na tela.
RevelarPosicao(int linha, int coluna): Método para revelar uma célula do tabuleiro escolhida pelo jogador. 
Se a célula contiver uma bomba, o jogo termina; caso contrário, as células adjacentes são reveladas automaticamente.
DescobrirCelulasAdjacentes(int linha, int coluna): Método recursivo para revelar as células adjacentes a uma célula escolhida pelo jogador.
VerificarVitoria(): Método para verificar se o jogador venceu o jogo, ou seja, se todas as células seguras foram reveladas. O tipo de retorno
deste método é bool, retornando true se o jogador venceu o jogo e false caso contrário.
VerificarDerrota(): Método para verificar se o jogador perdeu o jogo, ou seja, se revelou uma célula com uma bomba. O tipo de retorno deste 
método é bool, retornando true se o jogador perdeu o jogo e false caso contrário.
Já os outros métodos não possuem um tipo de retorno, pois são do tipo void, e não retornam nenhum valor.

(3) COMO EXECUTAR O PROGRAMA:
Após executar o programa, o jogador deve informar seu nome e o programa irá ler as informações do tabuleiro a partir de um arquivo de texto 
chamado "arquivo.txt". 
O formato do arquivo deve ser: número de linhas, número de colunas e número total de bombas. Em seguida o jogo começará e o jogador 
poderá digitar as coordenadas das células a serem reveladas.

(4) DECISÕES DE IMPLEMENTAÇÃO:
O jogo utiliza uma matriz bidimensional para representar o tabuleiro.
As células com bombas são representadas pelo caractere '*' e as células vazias possuem um número inteiro indicando a quantidade de bombas 
adjacentes.
A leitura das informações do tabuleiro é feita a partir de um arquivo de texto.
O jogo imprime o tabuleiro atualizado na tela a cada jogada
