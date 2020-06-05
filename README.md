1. A interface do usuário contém dois tipos de controles de entrada do usuário:
TextInput, que aceita todos os caracteres e NumericInput, que aceita apenas dígitos.

Implemente a classe TextInput que contem:
* Método público Add(char c) – adiciona o caracter ao valor atual
* Método público GetValue() – retorna o valor atual

Implemente a classe NumericInput que:
* Herde de TextInput
* Sobrescreva o método Add para que seja ignorado caracteres não numéricos.

Por exemplo, o método main() deverá apresentar o valor “10” como saída.

using System;

public class TextInput { }
public class NumericInput { }
public class UserInput
{
  public static void Main(string[] args)
  {
    TextInput input = new NumericInput();
    input.Add('1');
    input.Add('a');
    input.Add('0');
    Console.WriteLine(input.GetValue());
  }
}

2. Refatore as classes AlertService e AlertDAO:
* Crie uma nova interface, denominada IAlertDAO
* AlertDAO deve implementar a interface IAlertDAO
* AlertService deve ter um construtor que aceite IAlertDAO
* Os métodos RaiseAlert e GetAlertTime devem usar o objeto passado pelo construtor.
