# Exercício 1

public static void ex1() {
        // Escreva um algoritmo que armazene o valor 10 em uma variável A e o valor 20 em uma variável B.
        // A seguir (utilizando apenas atribuições entre variáveis) troque os seus conteúdos fazendo com que o
        // valor que está em A passe para B e vice-versa. Ao final, escrever os valores que ficaram armazenados
        // nas variáveis.
        
        int a = 10;
        int b = 20;
        int aux;
        aux = a;
        a = b;
        b = aux;
        System.out.println("Variavel A = " + a);
        System.out.println("Variavel B = " + b);


    }

<img src="/AssetsTeste/Ex1.png">

# Exercício 2 - A

static void ex2A()
{

        int a = 10;
        int b = 20;
    System.out.println("Valor de B: " + b);
    b = 5;
    System.out.println("Valor de A: " + a + "\nValor de B: " + b);
    }

<img src="/AssetsTeste/Ex2.png">

<br>
<h2>Exercício 2 - B</h2>


<br>
<h2>Exercício 5</h2>

public static void ex5() {
        // Escreva um algoritmo para ler um valor (do teclado) e escrever (na tela) o seu antecessor

        Scanner scanner = new Scanner(System.in);

        System.out.println("Insira o numero:");
        int numero = scanner.nextInt();
        System.out.println("Antecessor = :" + (numero - 1));


    }

<img src="/AssetsTeste/Ex8.png">  

<br>
<h2>Exercício 6</h2>

public static void ex6() {
        // Escreva um algoritmo para ler as dimensões de um retângulo (base e altura),
        // calcular e escrever a área do retângulo.

        Scanner scanner = new Scanner(System.in);

        System.out.println("Insira a base do retangulo:");
        double base = scanner.nextDouble();
        System.out.println("Insira a altura do retangulo");
        double altura = scanner.nextDouble();
        System.out.println("A area do retangulo é:" + (base * altura));
    }

<img src="/AssetsTeste/Ex9.png">  
<br>
<h2>Exercício 7</h2>
public static void ex7() {
        // Faça um algoritmo que leia a idade de uma pessoa expressa em anos, meses e dias e escreva a idade
        // dessa pessoa expressa apenas em dias. Considerar ano com 365 dias e mês com 30 dias.
        
        Scanner scanner = new Scanner(System.in);

        System.out.println("Insira quantos anos voce tem:");
        int ano = scanner.nextInt();
        System.out.println("Insira quantos meses voce tem:");
        int mes = scanner.nextInt();
        System.out.println("Insira quantos dias voce tem:");
        int dia = scanner.nextInt();

        System.out.println("Voce tem " + ((ano * 365) + (mes * 30) + dia));

    }
<img src="/AssetsTeste/Ex10.png">  
