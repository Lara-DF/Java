1. Entrada de Dados

String primeiroNumeroStr = JOptionPane.showInputDialog("Digite o primeiro número:");

Mostra uma janela para o usuário digitar o primeiro número.

<img width="960" height="540" alt="image" src="https://github.com/user-attachments/assets/af1d75cf-7e81-49d6-8060-849e676baacc" />


O valor digitado sempre é uma String (texto).

if (primeiroNumeroStr == null) {
    JOptionPane.showMessageDialog(null, "Entrada cancelada. Programa encerrado.");
    System.exit(0);
}

Esse bloco verifica se o usuário cancelou a entrada (clicou em "Cancelar" ou fechou a janela).

double primeiroNumero = Double.parseDouble(primeiroNumeroStr);
O mesmo processo é repetido para o segundo número.



2. Comparações

Aqui você verifica várias comparações entre os dois números usando if e else.

Exemplo:

if (primeiroNumero == segundoNumero) {
    mensagemFinal += primeiroNumero + " é IGUAL (==) a " + segundoNumero + "\n";
} else {
    mensagemFinal += primeiroNumero + " NÃO é igual a " + segundoNumero + "\n";
}

Se os números forem iguais, adiciona uma mensagem dizendo que são iguais.

Se não forem, adiciona uma mensagem dizendo que não são iguais.

Isso é repetido para outras comparações:

> maior que

< menor que

!= diferente

>= maior ou igual

<= menor ou igual

Todas as mensagens vão sendo juntadas numa variável chamada mensagemFinal.



3. Mostrar Resultado Final

JOptionPane.showMessageDialog(null, mensagemFinal, "Resultado das Comparações", JOptionPane.INFORMATION_MESSAGE);

Exibe uma janela com todas as mensagens de comparação que foram geradas.

Resumo

O programa pede dois números.

Converte esses números para o tipo numérico.

Compara os dois números usando diferentes operadores lógicos.

Mostra todas as comparações numa janela para o usuário ver.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/44c664f3-69f8-4e0e-a35e-077aac21bde3" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/913ef698-061c-4735-9339-b843264c69f0" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8d821534-60d0-4967-976c-047ed0ae83c4" />
