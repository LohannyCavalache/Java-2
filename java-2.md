package questao2;
import java.util.Scanner;

public class Questao2 {

    public static void main(String[] args) {
        //declaração de variáveis
        String [] nomes = new String[2];
        int [] idades = new int [2];
        
        //entrada de dados
        for(int i = 0; i < nomes.length; i++){
            Scanner entradaNome = new Scanner(System.in);
            System.out.println("Digite seu nome: \n");
            nomes[i] = entradaNome.nextLine();
            Scanner entradaIdade = new Scanner(System.in);
            System.out.println("Digite sua idade: \n");
            idades[i] = entradaIdade.nextInt();
        }
        
        //verificação de condições
        if(idades[0] < idades[1] && idades[1] >= 60){
            System.out.println("Quarto A: " + nomes[1] + " tem 40% de desconto. \n");
            System.out.println("Quarto B: "+ nomes[0] + "\n");
        }else if(idades[0] < idades[1]){
            System.out.println("Quarto A: " + nomes[1] + "\n");
            System.out.println("Quarto B: " + nomes[0] + "\n");
        }
        if(idades[0] > idades[1] && idades[0] >= 60){
            System.out.println("Quarto A: " + nomes[0] + " tem 40% de desconto. \n");
            System.out.println("Quarto B: " + nomes[1] + "\n");
        }else if(idades[0] > idades[1]){
            System.out.println("Quarto A: " + nomes[0] + "\n");
            System.out.println("Quarto B: " + nomes[1] + "\n");
        }

    } 
}
