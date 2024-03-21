# Resposta-Estagio-Ribeirao-Preto-2024
Resposta para o processo seletivo para a vaga de estágio

1) Observe o trecho de código abaixo:

<pre><code>int INDICE = 13, SOMA = 0, K = 0;

enquanto K < INDICE faça

{

K = K + 1;

SOMA = SOMA + K;

}

imprimir(SOMA);</code></pre>



Ao final do processamento, qual será o valor da variável SOMA? Ao final a variável SOMA vai ter o valor <b>91</b>

2) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.



IMPORTANTE:

Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;

Resposta em JavaScript:
<pre>
<code>function verificarNumero(numero) {
    let a = 0;
    let b = 1;
    while (a <= numero) {
        if (a === numero) {
            return true;
        }
        let temp = b;
        b = a + b;
        a = temp;
    }
    return false;
}

let numero = 55;
if (verificarNumero(numero)) {
    console.log(`O número ${numero} pertence à sequência de Fibonacci.`);
} else {
    console.log(`O número ${numero} não pertence à sequência de Fibonacci.`);
}</code></pre>

3) Descubra a lógica e complete o próximo elemento:



a) 1, 3, 5, 7, <b>9</b> 

b) 2, 4, 8, 16, 32, 64, <b>128</b> 

c) 0, 1, 4, 9, 16, 25, 36, <b>49</b>

d) 4, 16, 36, 64, <b>100</b>

e) 1, 1, 2, 3, 5, 8, <b>13</b>

f) 2,10, 12, 16, 17, 18, 19, <b>200</b>


4) Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada.

Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada? Primeiro ligaria um interruptor e aguardaria alguns minutos, depois iria apagar e ligaria outro interruptor, por fim iria até a sala de lâmpadas. Se a lampada estiver acessa, pertence ao interruptor 2, se estiver desligada e quente pertence ao interruptor 1, se estiver desligada e fria pertence ao interruptor 3.

5) Escreva um programa que inverta os caracteres de um string.


IMPORTANTE:

a) Essa string pode ser informada através de qualquer entrada de sua preferência ou pode ser previamente definida no código;

b) Evite usar funções prontas, como, por exemplo, reverse;

Resposta em JavaScript:
<pre><code>function inverterString(str) {
    let resultado = '';
    for (let i = str.length - 1; i >= 0; i--) {
        resultado += str[i];
    }
    return resultado;
}

const string = "Tenha um ótimo dia";
const stringInvertida = inverterString(string);
console.log(`A string "${string}" invertida fica "${stringInvertida}"`);</code></pre>
