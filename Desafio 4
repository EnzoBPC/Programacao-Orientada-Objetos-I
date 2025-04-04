import java.util.Scanner;
public class Desafio4 {
    public static void main(String[] args){
        Scanner leia = new Scanner(System.in);
        float wage,ajuste,truewage;
        byte wageb;
        do {
            System.out.println("Este programa irá receber um salário e fará um reajuste. A seguir terá uma tabela:");
            System.out.println("Até R$280.00 - terá um aumento de 20%");
            System.out.println("Entre R$280.00 e R$700.00 - terá um aumento de 15%");
            System.out.println("Entre R$700.00 e R$1500.00 - terá um aumento de 10%");
            System.out.println("De R$1500.00 em diante - terá um aumento de 5%");
            System.out.println("A inflação do período é de 3.8%");
            System.out.println(" ");
            System.out.println("Informe seu salário");
            if (!leia.hasNextFloat()) {
                System.out.println("Entrada inválida! Por favor, insira um número válido.");
                leia.next();
                continue;
            }
            wage = leia.nextFloat();
            if (wage > 0 && wage <= 280) {
                ajuste = 0.2f;
                wageb = 20;
            } else if (wage > 280 && wage <= 700) {
                ajuste = 0.15f;
                wageb = 15;
            } else if (wage > 700 && wage <= 1500) {
                ajuste = 0.1f;
                wageb = 10;
            } else if (wage > 1500) {
                ajuste = 0.05f;
                wageb = 5;
            } else {
                System.out.println("Valor inválido, o salário deve ser maior que zero");
                System.out.println(" ");
                continue;
            }
            System.out.println(" ");
            System.out.println("O percentual do ajuste será de " + wageb + "%");
            System.out.println("O valor do aumento foi de: R$"+wage*ajuste);
            ajuste = wage*ajuste;
            wage = wage+ajuste;
            System.out.println("O novo salário após o aumento é: "+wage);
            truewage = (float) (wage-(0.038*wage));
            System.out.println("O valor do aumento real descontado a inflação é: "+truewage);
            break;
        }while(true);
    }
}
