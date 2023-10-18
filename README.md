# 10 Exercícios + teste de mesa - Primeira Atividade - Matéria: LP1

<br>
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
77
        
        static void ex77()
        {
        int[] exV = {5,1,4,2,7,8,3,6};
        for (int i = 8;i >= 5; i --){
            int aux = exV[i];
            exV[i] = exV[7-i + 1];
            exV[7-i + 1] = aux;
        }
        exV[2] = exV[1];
        exV[exV[2]] = exV[exV[1]];

        System.out.println(Arrays.toString(exV));
    }

    
<img src="/AssetsTeste/ex77.png"> 
<br>
    
78
    
    static void ex78Vetor(){
        Scanner sc = new Scanner(System.in);
        ArrayList<String> pessoas = new ArrayList<>();
        for(int i = 0;i < 5 ;i++){
            System.out.println("Insira o nome da pessoa "+ (i+1)+"º");
            pessoas.add (sc.next());
        }
        System.out.println("Insira mais um nome: ");
        String nome = sc.next();
        pessoas.add(nome);
        for(int i = 0;i < 5 ;i++){
            if(nome.equals(pessoas.get(i))){
                System.out.println("O nome na posição: " + (i+1) + " = "+pessoas.get(i)+" é igual ao nome fornecido, o nome é: " + nome);
            }
        }
    }
    
<img src="/AssetsTeste/ex78.png"> 

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
80

        static void ex80ArraySimples(){
        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        double arma_media = 0;
        double media = 0;
        for(int i = 0; i < notas.length; i ++ ){
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
            arma_media += notas[i];
        }
        media = arma_media / notas.length;
        int maior = notas[0];
        int pos = 0;
        for(int i = 0; i < notas.length; i ++ ){
            if(maior < notas[i]){
                maior = notas[i];
                pos = (i+1);
            }
            else{
                pos = (i+1);
            }
        }
        System.out.println("O Aarray: " + Arrays.toString(notas));
        System.out.println("A média das notas: " + media);
        System.out.println("A maior das notas: " + maior);
        System.out.println("A posição do Maior é o número " + pos +" na lista");


    }

<img src="/AssetsTeste/ex80.png">     
<br>
81

                static void ex81ArraySimples(){
        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        double arma_media = 0;
        double media = 0;
        for(int i = 0; i < notas.length; i ++ ){
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
            arma_media += notas[i];
        }
        media = arma_media / notas.length;
        int menor = notas[0];
        int pos = 1;
        for(int i = 0; i < notas.length; i ++ ){
            if(menor > notas[i]){
                menor = notas[i];
                pos = (i+1);
            }
            else{
                pos = (i+1);
            }
        }
        System.out.println("O Array: " + Arrays.toString(notas));
        System.out.println("A média das notas: " + media);
        System.out.println("A menor das notas: " + menor);
        System.out.println("A posição do Maior é o número " + pos +" na lista");


    }


<img src="/AssetsTeste/ex81.png">     
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
83

        static void ex83ArraySimples(){
        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        for(int i = 0; i < notas.length; i ++ ) {
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
        }
        for(int i = 1; i < notas.length; i ++ ) {
            System.out.println("Da primeira até a ultima: " + i);
        }

        System.out.println("----------------------");

        for(int i = 1; i < notas.length; i ++ ) {
            System.out.println("Da última até o começo: " + notas[notas.length - i]);
        }
        System.out.println("Da última até o começo: " + notas[0]);
        System.out.println("O Array: " + Arrays.toString(notas));

    }

<img src="/AssetsTeste/ex83.png">    
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
<br>
85

        public class Exercicio85ArraySimples {
        public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int[] temperaturas = new int[365];
        
        // Leitura das temperaturas médias diárias
        for (int i = 0; i < temperaturas.length; i++) {
            System.out.println("Insira a temperatura média do dia " + (i + 1) + ": ");
            temperaturas[i] = sc.nextInt();
        }

        // Encontrar a menor e a maior temperatura do ano
        int menorTemp = temperaturas[0];
        int maiorTemp = temperaturas[0];
        int somaTemps = 0;

        for (int temp : temperaturas) {
            if (temp < menorTemp) {
                menorTemp = temp;
            }

            if (temp > maiorTemp) {
                maiorTemp = temp;
            }

            somaTemps += temp;
        }

        // Calcular a temperatura média anual
        double mediaAnual = (double) somaTemps / temperaturas.length;

        // Contar o número de dias com temperatura inferior à média anual
        int diasAbaixoMedia = 0;

        for (int temp : temperaturas) {
            if (temp < mediaAnual) {
                diasAbaixoMedia++;
            }
        }

        // Exibir os resultados
        System.out.println("Menor temperatura do ano: " + menorTemp);
        System.out.println("Maior temperatura do ano: " + maiorTemp);
        System.out.println("Temperatura média anual: " + mediaAnual);
        System.out.println("Número de dias com temperatura abaixo da média anual: " + diasAbaixoMedia);
            }
        }
<img src="/AssetsTeste/ex85.png"> 
<br>
86

            static void ex86ArraySimples(){
        Scanner sc = new Scanner(System.in);
        int[] vetorD = new int[9];
        for(int i = 0;i< vetorD.length;i++){
            System.out.println("Insira os valores desordenados: ");
            vetorD[i] = sc.nextInt();
        }
        System.out.println("O Array desordenado: " + Arrays.toString(vetorD));
        for(int i = 0;i< vetorD.length;i++){
            for(int j = i + 1;j< vetorD.length;j++){
                if(vetorD[i] > vetorD[j]){
                    int temporario = vetorD[i];
                    vetorD[i] = vetorD[j];
                    vetorD[j] = temporario;
                }
            }
        }
        System.out.println("O Array ordenado: " + Arrays.toString(vetorD));
    }
<img src="/AssetsTeste/ex86.png"> 
<br>
87

        public static void ex87ArrayNormal() {
        Scanner sc = new Scanner(System.in);

        int[] vetor = new int[11];
        int novoNumero;
        
        for (int i = 0; i < 10; i++) {
            System.out.println("Insira um número: ");
            vetor[i] = sc.nextInt();
        }

        System.out.println("Insira mais um número: ");
        novoNumero = sc.nextInt();
        
        int posicaoInsercao = 0;
        while (posicaoInsercao < 10 && novoNumero > vetor[posicaoInsercao]) {
            posicaoInsercao++;
        }
        
        for (int i = 10; i > posicaoInsercao; i--) {
            vetor[i] = vetor[i - 1];
        }
        
        vetor[posicaoInsercao] = novoNumero;
        
        System.out.println("Vetor com o novo número inserido e ordenado: " + Arrays.toString(vetor));
    }
<img src="/AssetsTeste/ex87.png"> 
<br>
88

        static void ex88ArraySimples(){
        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        for(int i = 0; i < notas.length; i ++ ) {
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
        }
        boolean existe = false;
        System.out.println("Insira mais um número: ");
        int maisum = sc.nextInt();
        for(int i = 0; i < notas.length; i ++ ) {
            if (maisum == notas[i]){
                existe = true;
            }
        }
<img src="/AssetsTeste/ex88.png"> 
<br>
89

        static void ex89(){
        int[] V1 = new int[5];
        int[] V2 = new int[5];

        int qtd_Vezes = 0;
        int msm_pos = 0;
        Scanner sc = new Scanner(System.in);
        for(int i = 0; i < V1.length; i ++ ) {
            System.out.println("Insira os números: ");
            V1[i] = sc.nextInt();
        }
        for(int i = 0; i < V1.length; i ++ ) {
            System.out.println("Insira os números VETOR 2: ");
            V2[i] = sc.nextInt();
        }
        for(int i = 0; i < V1.length; i ++ ) {
            if(V1[i] == V2[i]){
                qtd_Vezes += 1;
            }

        }
        System.out.println(Arrays.toString(V1));
        System.out.println(Arrays.toString(V2));
        System.out.println("Qtd vezes iguais em que é o mesmo número e na mesma posição: " + qtd_Vezes);


    }
<img src="/AssetsTeste/ex89.png"> 
<br>
90

       static void ex90ArraySimples() {
        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        for (int i = 0; i < notas.length; i++) {
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
        }
        int existe = 0;
        System.out.println("Insira mais um número: ");
        int maisum = sc.nextInt();
        for (int i = 0; i < notas.length; i++) {
            if (maisum == notas[i]) {
                existe += 1;
            }
        }

        System.out.println("A quantidade de vezes em que o número digitado aparece no array é: " + existe);
    }  
<img src="/AssetsTeste/ex90.png"> 
<br>
91

        static void ex91ArraySimples() {
        int[] notas = new int[5];
        Scanner sc = new Scanner(System.in);
        for (int i = 0; i < notas.length; i++) {
            System.out.println("Insira os números: ");
            notas[i] = sc.nextInt();
        }
        int mesmo = 0;
        for (int i = 0; i < notas.length; i++) {
            for(int j = i + 1; j < notas.length; j++){
                if(notas[i] == notas[j]){
                    mesmo += 1;
                    System.out.println("O número: " + notas[i] + " está repetido na posição: " + (i+1) + " e na posição: " + (j+1));
                }
            }
        }
    }
<img src="/AssetsTeste/ex91.png"> 
<br>
<br>
Fim
