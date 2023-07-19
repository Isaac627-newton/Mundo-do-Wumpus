# Mundo-do-Wumpus

Universidade Federal do Pará

Disciplina: Inteligência Computacional

Professor: Otávio Noura Teixeira

Alunos: Horácio Santos e Isaque Oliveira.

Tema: Mundo do Wumpus: uma ferramenta para o desenvolvimento de raciocínio lógico.


# Introdução

Projeto voltado para obtenção de nota na disciplina de Inteligência Computacional, 7º Semestre, 2023.


# Etapa 01 (CONCLUÍDA) 

O código em C apresentado é um pequeno programa que tem como objetivo gerar um ambiente aleatório para um jogo, com base nas especificações fornecidas pelo usuário. O ambiente é representado por uma matriz bidimensional, onde diferentes objetos, como Poços (POCO), Wumpus (WUMPUS) e Ouro (OURO), são posicionados aleatoriamente. A seguir, faremos uma análise do funcionamento do código e das principais funcionalidades implementadas:

1. Entrada de Dados:
O programa inicia solicitando ao usuário a entrada de algumas informações fundamentais para a geração do ambiente. O usuário é convidado a fornecer o tamanho do ambiente, que corresponde a uma grade n x n, onde n é um número inteiro. Além disso, o usuário deve informar a quantidade desejada de Poços, Wumpus e Ouro no ambiente. Essas informações são cruciais para criar um ambiente desafiador e interessante para o jogo.

2. Alocação Dinâmica da Matriz de Ambiente:
O código implementa uma função chamada "Criar_Ambiente" que é responsável por alocar dinamicamente a matriz que representa o ambiente do jogo. Isso permite a criação de um ambiente de qualquer tamanho especificado pelo usuário.

3. Posicionamento dos Objetos:
A função "Posicionar_objetos" é responsável por posicionar aleatoriamente os objetos (Poços, Wumpus e Ouro) no ambiente criado. A lógica garante que nenhum objeto é colocado na posição inicial do jogador, que é representada pela célula (0, 0), e também verifica se a quantidade de objetos é válida para o tamanho do ambiente, para evitar conflitos ou excessos.

4. Exibição do Ambiente:
A função "Exibir_Ambiente" é usada para imprimir o ambiente gerado, mostrando visualmente ao usuário a posição dos objetos (Wumpus, Ouro e Poços) usando caracteres específicos ('W', 'O', 'P' e '.'). Essa visualização torna mais fácil para o jogador entender a configuração do ambiente.

5. Liberação de Memória:
Após a exibição do ambiente, o programa libera a memória alocada dinamicamente para a matriz de ambiente, garantindo que não haja vazamento de memória.

6. Tratamento de Erros:
O código também inclui tratamentos de erro para verificar se as entradas do usuário são válidas. Por exemplo, ele impede que o usuário crie um ambiente com tamanho menor que 3 e verifica se a quantidade total de objetos não excede o tamanho do ambiente menos uma célula (para evitar ocupar a célula inicial do jogador).

7. Geração Aleatória:
O programa utiliza a função "rand()" para gerar números aleatórios, e a semente do gerador é inicializada com "srand(time(NULL))", que usa o valor do relógio do sistema como semente para garantir que as posições dos objetos sejam diferentes em cada execução.


# ETAPA 02 (INCOMPLETA)

- Durante o processo de criação do código, optamos pela criação do código por etapas, com o intuito de aperfeiçoar melhor o tempo determinado para a conclusão deste trabalho.

- Todavia, a etapa 02 e as demais encontraram alguns obstáculos. Um dos principais foi a ausência de domínio de determinados assuntos em programação, o que acabou por ser um empecilho na condução e realização deste trabalho.
 
- Durante a criação do código houveram diversos desafios, mas o principal foi desenvolver uma boa lógica para a locomoção do agente pelo ambiente e as decisões que ele iria tomar caso encontrasse algum obstáculo durante o seu percurso pelo ambiente. 
