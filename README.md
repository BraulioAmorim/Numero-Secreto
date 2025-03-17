# Jogo do Número Secreto

Este é um jogo simples onde o jogador deve adivinhar um número secreto gerado aleatoriamente pelo sistema.

## Como Funciona

1. O jogo gera um número aleatório entre 1 e 50, garantindo que o mesmo número não seja repetido até que todos tenham sido sorteados.
2. O jogador insere um palpite no campo de entrada e clica em **"Verificar"**.
3. O sistema informa se o palpite está correto, ou se o número secreto é maior ou menor.
4. O jogo continua até que o jogador acerte o número secreto.
5. Ao acertar, o jogo informa quantas tentativas foram necessárias e habilita o botão de **"Reiniciar"**.
6. Ao clicar em **"Reiniciar"**, um novo número é sorteado e o jogo recomeça.

## Tecnologias Utilizadas

- HTML
- CSS
- JavaScript
- Biblioteca [ResponsiveVoice](https://www.responsivevoice.org/) para feedback por voz

## Estrutura do Código

```javascript
// Exibe um texto na tela e o reproduz por voz
function exibirTextoNaTela(tag, texto) {
    let campo = document.querySelector(tag);
    campo.innerHTML = texto;
    responsiveVoice.speak(texto, 'Brazilian Portuguese Female', {rate:1.2});
}
```

- **`exibirMensagemInicial()`**: Define a mensagem inicial do jogo.
- **`verificarChute()`**: Verifica se o palpite do jogador está correto e exibe a resposta adequada.
- **`gerarNumeroAleatorio()`**: Gera um número aleatório entre 1 e 50, evitando repetições.
- **`limparCampo()`**: Limpa o campo de entrada.
- **`reiniciarJogo()`**: Reinicia o jogo gerando um novo número e resetando as tentativas.

## Como Executar o Jogo

1. Clone o repositório:
   ```sh
   git clone https://github.com/seu-usuario/jogo-numero-secreto.git
   ```
2. Acesse a pasta do projeto:
   ```sh
   cd jogo-numero-secreto
   ```
3. Abra o arquivo `index.html` no navegador.
4. Insira um número no campo de entrada e clique em **"Verificar"**.
5. Siga as dicas para encontrar o número secreto.
6. Ao acertar, clique em **"Reiniciar"** para jogar novamente.

---

Divirta-se jogando! 🎲

