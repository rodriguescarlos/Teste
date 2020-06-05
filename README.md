1.       O que é classe?
	
	
2.       O que é interface? 
	
	
3.       O que é Abstração?
	
	
4.       O que é Encapsulamento?
	
	
5.       O que é Herança? Escreva um exemplo (pode ser em forma de código ou em representação gráfica)
	
	
6.       O que é Polimorfismo?
	
	
7.       O que é uma classe abstrata? 
	
	
8.       Cite os modificadores de acesso mais utilizados em classes, métodos e atributos.
	
	
9.       Qual a diferença entre uma interface e uma classe abstrata?
	
	
10.   O que é DML?
a.      (   )  São comandos de manipulação de objetos no banco de dados. (CREATE, ALTER, DROP)
b.      (   )  São comandos de manipulação de dados no banco de dados. (INSERT, UPDATE e DELETE)
c.      (   )  São comandos que garantem a integridade do banco de dados. (BEGIN TRANSACTION, TRIGGER, IDENTITY, FOREIGN KEY)
	
11.   O que é DDL?
a.      (   )  São comandos de manipulação de dados no banco de dados. (INSERT, UPDATE e DELETE)
b.      (   )  São comandos que garantem a integridade do banco de dados. (BEGIN TRANSACTION, TRIGGER, IDENTITY, FOREIGN KEY)
c.      (   )  São comandos de manipulação de objetos no banco de dados. (CREATE, ALTER, DROP)
	
12.   O resultado do comando SELECT * FROM TB_CLIENTES WHERE Ativo = ‘S’ é:
a.      (   )  Altera todos os clientes para ativo -  (Ativo = ‘S’) 
b.      (   )  Retorna todos os clientes, inclusive os inativos.
c.      (   )  Retorna todos os clientes, inclusive os ativos.
d.      (   )  Retorna apenas os clientes ativos.
	
13.   Qual a saído do código abaixo?
static void Main(string[] args)
{	
	int[] numeros = { 1, 2, 3, 5, 7, 8, 9, 11, 13, 17, 19, 23, 29, 31, 34, 36, 38, 40};
	
	for(int i = 0; i< numeros.Length; i++)
	if (Calcular(numeros[i]))
	Console.WriteLine(numeros[i]);
}	
public static bool Calcular(int n)
{	
	if (n == 1) return false;
	for(int i = 2; i * i <= n; i++){
		if (n % i == 0) return false;
	}
	return true;
}	

a.   (    )  Imprime os valores 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31
b.   (    )  Imprime os valores 2, 8, 34, 36, 38, 40
c.   (    )  Imprime todos os números
d.   (    )  Imprime somente os primeiros 10 números do vetor
e.   (    )  Não imprime nada
	
14.   Oque o trecho de código abaixo faz?
	static void Main(string[] args)
	{
		var listFunc = new Func<int>[10];
		for (int it = 0; it < 10; it++)
		{
			listFunc[it] = () => it;
			Console.WriteLine(listFunc[it]());
		}
	}	
		
15.   Qual o valor que será impresso quando o contador estiver com o valor 9 no código abaixo?
	
static void Main(string[] args)
{	
	for (int contador = 0; contador < 15; contador++){
		Console.WriteLine(Fibonacci(contador));
	}
}	


public static int Fibonacci(int n)
{	
	int a = 0;
	int b = 1;
	
	// In N steps compute Fibonacci sequence iteratively.
	for (int i = 0; i < n; i++)
	{
		int temp = a;
		a = b;
		b = temp + b;
	}
	return a;
}	


