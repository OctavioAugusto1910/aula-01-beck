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

