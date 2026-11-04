Projeto: Sistema de Monitoramento de Temperatura
1. Identificação
Aluno: [Seu nome]
Disciplina: [Nome da disciplina]
Professora: Profa. Karla Sartin
Título: Sistema de Monitoramento de Temperatura
2. Objetivo

O objetivo deste projeto é desenvolver um programa em linguagem C capaz de monitorar temperaturas, identificar valores acima de um limite estabelecido e emitir um alerta quando ocorrerem três temperaturas consecutivas acima desse limite.

O programa também apresenta um relatório final com informações estatísticas das leituras realizadas.

3. Funcionamento do programa

Inicialmente, o programa solicita ao usuário um limite máximo de temperatura. Esse valor deve ser numérico e não pode ser negativo.

Em seguida, o sistema começa a receber as leituras de temperatura.

As entradas inválidas, como letras ou números negativos, são rejeitadas, solicitando uma nova informação ao usuário.

Quando uma temperatura ultrapassa o limite estabelecido, o programa apresenta uma mensagem de alerta e incrementa os contadores de temperaturas acima do limite e de temperaturas consecutivas.

Caso uma temperatura esteja dentro do limite, o contador de temperaturas consecutivas é reiniciado.

Quando são identificadas três temperaturas consecutivas acima do limite, o monitoramento é encerrado automaticamente.

Ao final, o programa apresenta:

Quantidade total de leituras;
Maior temperatura registrada;
Menor temperatura registrada;
Média das temperaturas;
Quantidade de temperaturas acima do limite;
Percentual de temperaturas acima do limite.
4. Estruturas de repetição utilizadas

Foram utilizadas as estruturas do...while e while.

do...while

Foi utilizada na validação do limite de temperatura, garantindo que o usuário informe um valor válido.

Essa estrutura executa o bloco pelo menos uma vez antes de verificar a condição.

while

Foi utilizada no monitoramento das temperaturas, permitindo que o programa receba várias leituras até que a condição de encerramento seja atingida.

Também foi utilizada na validação das temperaturas informadas pelo usuário.

A estrutura while foi escolhida porque permite verificar a condição antes de cada repetição.

5. Como executar

É necessário possuir um compilador C, como o GCC.

Para compilar, utilize:

bash
gcc monitoramento.c -o monitoramento


Para executar no Linux:

bash
./monitoramento


No Windows:

bash
monitoramento.exe

6. Testes realizados
Teste 1: Validação de entradas inválidas

Foi informado um valor inválido para o limite e também uma temperatura negativa.

Resultado esperado: O programa rejeita as entradas inválidas e solicita novos valores.

Teste 2: Temperaturas acima do limite, porém não consecutivas

Limite: 30°C.

Leituras: 35°C, 28°C, 36°C, 29°C, 38°C.

Resultado esperado: O programa identifica as temperaturas acima do limite, mas não encerra o monitoramento porque elas não são consecutivas.

Teste 3: Três temperaturas consecutivas acima do limite

Limite: 30°C.

Leituras: 32°C, 35°C, 38°C.

Resultado esperado: O programa identifica três temperaturas consecutivas acima do limite, apresenta um alerta crítico e encerra automaticamente o monitoramento.

7. Reflexão final

Escolhi utilizar as estruturas while e do...while porque ambas atendem às necessidades do sistema de monitoramento.

A estrutura do...while foi importante na validação inicial do limite de temperatura, pois garante que a solicitação seja executada pelo menos uma vez.

Já a estrutura while foi utilizada no monitoramento das temperaturas, pois permite repetir a leitura enquanto a condição de encerramento não for atingida.

A diferença entre testar a condição antes ou depois da execução foi importante para garantir que o limite fosse solicitado ao usuário pelo menos uma vez e que o monitoramento continuasse somente enquanto necessário.
