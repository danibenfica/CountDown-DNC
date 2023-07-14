![COUNTDOWN-_online-video-cutter com_](https://github.com/danibenfica/CountDown-DNC/assets/103818625/0a85b050-a7b7-4e7e-b636-e6b3bc90de68)

## Countdown

[Link do projeto online aqui!](https://count-down-dnc.vercel.app/)

### Descrição do Projeto
O projeto  Countdown é uma aplicação simples desenvolvida em JavaScript. Ela exibe um contador regressivo que mostra a contagem de dias, horas, minutos e segundos até uma data específica de lançamento. Neste caso, a data atual é o natal deste ano(2023). O objetivo é estudar JavaScript com a manipulação
do DOM.


### Como Clonar
Para utilizar o projeto, siga as etapas abaixo para clonar o repositório:

1. Abra o terminal ou prompt de comando.
2. Execute o seguinte comando para clonar o repositório:
   ```
   git clone https://github.com/danibenfica/CountDown-DNC.git
   ```
3. Navegue até a pasta clonada:
   ```
   cd CountDown-DNC
   ```
4. Abra o arquivo `index.html` em um navegador web compatível.

Isso irá clonar o repositório do projeto para o seu computador e permitir que você execute a aplicação diretamente em seu navegador.

### Tecnologias Utilizadas

- HTML: Linguagem de marcação para estruturar a página web.
- CSS: Linguagem de estilização para definir a aparência e o layout dos elementos.
- JavaScript: Linguagem de programação para a lógica do contador e manipulação do DOM.

### Principais Funções

#### countDown()
A função `countDown()` é responsável por calcular o tempo restante até a data de lançamento definida. Ela utiliza objetos `Date` para obter a data atual e a data de lançamento, e em seguida, calcula a diferença em segundos. Com base nessa diferença, são calculados o número de dias, horas, minutos e segundos restantes. Por fim, os valores são atualizados no HTML para exibir a contagem regressiva.

Trecho do código:
```javascript
function countDown() {
   const dataLanc = new Date(lancamento);
   const hoje = new Date();

   const segTotal = (dataLanc - hoje) / 1000;

   const finalDias = Math.floor(segTotal / 60 / 60 / 24);
   const finalHoras = Math.floor(segTotal / 60 / 60) % 24;
   const finalMinutos = Math.floor(segTotal / 60) % 60;
   const finalSegundos = Math.floor(segTotal) % 60;

   dia.innerHTML = finalDias;
   hora.innerHTML = formatoTempo(finalHoras);
   minuto.innerHTML = formatoTempo(finalMinutos);
   segundo.innerHTML = formatoTempo(finalSegundos);
}
```

#### formatoTempo(tempo)
A função `formatoTempo(tempo)` é uma função auxiliar que recebe um valor de tempo (dias, horas, minutos ou segundos) e retorna uma string formatada. Se o valor for menor que 10, a função adiciona um zero à frente para manter um formato consistente.

Trecho do código:
```javascript
function formatoTempo(tempo) {
    return tempo < 10 ? `0${tempo}` : tempo;
}
```

### Conclusão
O projeto Countdown é uma implementação simples em JavaScript que oferece aos usuários uma contagem regressiva até uma data de lançamento especificada. Utilizando as tecnologias HTML, CSS e JavaScript, o projeto demonstra o uso básico de manipulação do DOM e cálculos de tempo. Com esse exemplo, é possível construir aplicações mais complexas e personalizadas de acordo com as necessidades de cada desenvolvedor.

Qualquer sugestão ou dúvida, pode me contatar! :heart: