javascript

function verificarPalindromo(palavra) {
  // Remover espaços em branco e converter para letras minúsculas
  palavra = palavra.toLowerCase().replace(/\s/g, '');

  // Verificar se a palavra é um palíndromo
  for (let i = 0; i < palavra.length / 2; i++) {
    if (palavra[i] !== palavra[palavra.length - 1 - i]) {
      return false;
    }
  }
  return true;
}

// Escreva um programa que recebe