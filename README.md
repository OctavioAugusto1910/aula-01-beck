function verificarSituacaoAluno(nota) {
  if (nota === 10) {
    console.log("Parabéns! Nota máxima! Você foi aprovado com excelência!");
  } else if (nota >= 7) {
    console.log("Aprovado! Muito bom trabalho!");
  } else if (nota >= 4 && nota <= 6) {
    console.log("Você está de recuperação. Continue se esforçando!");
  } else if (nota >= 0 && nota < 4) {
    console.log("Reprovado. Não desanime, tente novamente!");
  } else {
    console.log("Nota inválida. Por favor, insira uma nota entre 0 e 10.");
  }
}

function jogarParOuImpar() {
  let escolha = prompt("Você escolhe 'par' ou 'ímpar'?");
  escolha = escolha.toLowerCase();

  let numeroUsuario = parseInt(prompt("Digite um número entre 1 e 9:"));
  let numeroComputador = Math.floor(Math.random() * 9) + 1;
  let soma = numeroUsuario + numeroComputador;

  console.log(`Seu número: ${numeroUsuario}`);
  console.log(`Número do computador: ${numeroComputador}`);
  console.log(`Soma dos dois números: ${soma}`);

  let resultado = soma % 2 === 0 ? "par" : "ímpar";

  if (resultado === escolha) {
    console.log("Você venceu!");
  } else {
    console.log("Você perdeu!");
  }
}

jogarParOuImpar();



