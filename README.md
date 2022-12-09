# Bandeira_do_Brasil
A nossa bandeira em HTML.

Nos exercícios anteriores já praticamos como desenhar retângulos e triângulos. Agora só falta lembrar do círculo. Aqui também devemos começar um path:

var tela = document.querySelector('canvas');
var pincel = tela.getContext('2d');

pincel.fillStyle="darkblue";
pincel.beginPath();

E, para desenhar o círculo, usamos a função arc:

var tela = document.querySelector('canvas');
var pincel = tela.getContext('2d');

pincel.beginPath();
pincel.arc(300, 200, 100, 0, 2*3.14);
pincel.fill();

Os primeiros dois parâmetros do método arc são as coordenadas X e Y do centro do círculo (no nosso caso, 300 e 200). O terceiro parâmetro é o valor do raio (no nosso caso, 100). O quarto e quinto parâmetros definem o ângulo inicial e final do círculo. Como queremos desenhar um círculo completo, os parâmetros são, respectivamente, 0 e 2 * PI (cujo valor é 3.14).
