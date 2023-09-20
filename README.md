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
    static void ex2B()
    
    {

        
        int a = 30;
        int b = 20;
        int c = a + b;
        System.out.println("Valor de C: " + c);
        b = 10;
        System.out.println("Valor de B: " + b + "\nValor de C: " + c);
        c = a + b;
        System.out.println("\nValor de A: " + a +"Valor de B: " + b + "\nValor de C: " + c);
    }
<img src ="/AssetsTeste/Ex3.png">

<br>
<h2>Exercício 2 - C </h2>
static void ex2C()

{


        int a = 10;
        int b = 20;
        int c = a;
        b = c;
        a = b;
        System.out.println("\nValor de A: " + a +"Valor de B: " + b + "\nValor de C: " + c);
    }
<img src = "/AssetsTeste/Ex4.png">
<br>
<h2>Exercício 2 - D</h2>

static void ex2D()
{

        
        int a = 10;
        int b = a + 1;
        a = b + 1;
        b = a + 1;
        System.out.println("Valor de A: " + a);
        a = b + 1;
        System.out.println("\nValor de A: " + a +"Valor de B: " + b);
    }
<img src = "/AssetsTeste/Ex5.png">

<br>
<h2>Exercício 2 - E</h2>

static void ex2E()
{

        
        int a = 10;
        int b = 5;
        int c = a + b;
        b = 20;
        a = 10;
        System.out.println("\nValor de A: " + a +"Valor de B: " + b);
    }
<img src = "/AssetsTeste/Ex6.png">

<br>
<h2>Exercício 2 - F</h2>
static void ex2F()
{

        
        int x = 1;
        int y = 1;
        int z = x + y;
        System.out.println("Valor de Z: " + z);
        x = 5;
        y = x + z;
        System.out.println("\nValor de X: " + x +"Valor de Y: " + y + "Valor de Z: " + z);
    }
<img src = "/AssetsTeste/Ex7.png">
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

# Exercícios de ArraySimples e ArrayList Prof Adriana

static void ex79ArraySimples(){


        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        double armaz_nota = 0;
        double media = 0;
        int maior_que_A_media = 0;
        for(int i = 0; i < notas.length; i ++ ){
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
            armaz_nota += notas[i];
        }
        media = armaz_nota / notas.length;
        for(int i = 0; i < notas.length; i ++ ){
            if(notas[i] > media){
                maior_que_A_media += 1;
            }
        }
        System.out.println("A média das notas dos alunos: " + media);
        System.out.println("Vezes em que a nota de algum aluno foi maior que a média: " + maior_que_A_media);
    }

<img src="/AssetsTeste/aula01.png">  
<br>
static void ex82ArraySimples(){


        int[] notasV = new int[5];
        int[] notasM = new int[5];
        Scanner sc = new Scanner(System.in);

        for(int i = 0; i < notasV.length; i ++ ) {
            System.out.println("Insira os números: ");
            notasV[i] = sc.nextInt();
        }
        System.out.println("Insira mais um número: ");
        int maisum = sc.nextInt();

        for(int i = 0; i < notasM.length; i++){
            notasM[i] = notasV[i] * maisum;
        }
        System.out.println("O Array Original: " + Arrays.toString(notasV));
        System.out.println("O Array Multiplicado: " + Arrays.toString(notasM));

    }
<img src="/AssetsTeste/aula02.png">  


<br>

static void ex84() {


        Scanner sc = new Scanner(System.in);

        int n = 0;
        System.out.println("Insira o valor de N: ");
        n = sc.nextInt();

        int[] Aba = new int[n];
        int[] Bab = new int[n];
        int[] Soma = new int[n];

        for (int i = 0; i < Aba.length; i++) {
            System.out.println("Insira os valores do vetor A: ");
            Aba[i] = sc.nextInt();

            System.out.println("Insira os valores do vetor B: ");
            Bab[i] = sc.nextInt();
        }
        
        for (int i = 0; i < Aba.length; i++) {
            Soma[i] = Aba[i] + Bab[i];
        }

        System.out.println("O vetor A: " + Arrays.toString(Aba));
        System.out.println("O vetor B: " + Arrays.toString(Bab));
        System.out.println("O vetor das somas de A e B: " + Arrays.toString(Soma));


    }

<img src="/AssetsTeste/aula03.png">  


