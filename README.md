import java.util.Scanner;
public class Media {

    public static void main (String[]args) {
        Scanner scanner = new Scanner(System.in); 
        
        System.out.println("Digite seu nome:");
        String nome = scanner.nextLine(); // Captura o nome do aluno


        System.out.println("Olá " + nome + ", tudo bem?");
        System.out.println("Sabemos que a média final é algo que assusta muito, e para não ter complicações, desenvolvemos este algoritmo para te ajudar.");


        double ac1, ac2, ag, af, resultado;

         // Captura a nota da AC1
         System.out.println("A seguir você irá nos contar qual é a sua nota da AC1 (Avaliação Contínua 1), lembrando que essa prova tem peso de 0.15 no valor final.");
         System.out.println("Por favor, digite sua nota na AC1:");
         ac1 = scanner.nextDouble();
         System.out.println("Sua nota da AC1 é: " + ac1);
         System.out.println("Sua nota real da AC1 é: " + (ac1 * 0.15));
 

          // Captura a nota da AC2
        System.out.println("Agora, digite sua nota na AC2 (Avaliação Contínua 2), essa prova tem peso 0.30.");
        ac2 = scanner.nextDouble();
        System.out.println("Sua nota da AC2 é: " + ac2);
        System.out.println("Sua nota real da AC2 é: " + (ac2 * 0.30));

        // Captura a nota da AG
        System.out.println("Agora, digite sua nota na AG (Avaliação Geral), essa prova tem peso 0.10.");
        ag = scanner.nextDouble();
        System.out.println("Sua nota da AG é: " + ag);
        System.out.println("Sua nota real da AG é: " + (ag * 0.10));


          // Captura a nota da AF
          System.out.println("Agora, digite sua nota na AF (Avaliação Final), essa prova tem peso 0.45.");
          af = scanner.nextDouble();
          System.out.println("Sua nota da AF é: " + af);
          System.out.println("Sua nota real da AF é: " + (af * 0.45));
  
          // Cálculo da média final
          resultado = (ac1 * 0.15) + (ac2 * 0.30) + (ag * 0.10) + (af * 0.45);
          System.out.println("A sua média final é: " + resultado);
  
          scanner.close(); // Fecha o scanner para evitar vazamento de recursos
  
    }
}
