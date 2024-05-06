import java.util.Scanner;

public class ContaTerminal {
    public static void main(String[] args) {

        try (Scanner leitor = new Scanner(System.in)) {
            String nomeCliente;
            String agencia;
            int conta;
            double saldo;

            System.out.println("Por favor, digite o seu nome!");
            nomeCliente = leitor.nextLine();
            System.out.println("");

            System.out.println("Por favor, digite o número da agência!");
            agencia = leitor.nextLine();
            System.out.println("");

            System.out.println("Por favor, digite o número da conta!");
            conta = leitor.nextInt();
            System.out.println("");

            System.out.println("Por favor, digite o valor que irá depositar!");
            saldo = leitor.nextDouble();
            System.out.println("");

            System.out.println(
                    "Olá " + nomeCliente + ", obrigado por criar uma conta em nosso banco, sua agência é " + agencia
                            + ", conta " + conta + " e seu saldo " + saldo + " já está disponível para saque.");
        }

    }
}
