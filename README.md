# lanchonete
Cardápio de Lanchonete criado no C#
Console.WriteLine("Lanches do Wellington");
//enunciado
//crie um programa usando array com o nome de 5 lanches e outro array com seus respectivos valores
//Imprima na tela o nome do lanche escolhido e o seu valor
string [] lanche ={"Hot Dog","Misto Quente","X-Burger","X-Calabresa","X-Frango"};
double [] valor ={6.55, 8.90, 9.99,10.89,11.20};

_etq:
System.Console.WriteLine($"Para o Lanche {lanche[0]} que custa {valor[0].ToString("c")} digite 0"); //ToString serve para setar o valor em reais
System.Console.WriteLine($"Para o Lanche {lanche[1]} que custa {valor[1].ToString("c")} digite 1");
System.Console.WriteLine($"Para o Lanche {lanche[2]} que custa {valor[2].ToString("c")} digite 2");
System.Console.WriteLine($"Para o Lanche {lanche[3]} que custa {valor[3].ToString("c")} digite 3");
System.Console.WriteLine($"Para o Lanche {lanche[4]} que custa {valor[4].ToString("c")} digite 4");

System.Console.Write("Qual sua escolha?");
int escolha = int.Parse(Console.ReadLine());
System.Console.Write("Gostaria de Adicionar Bebida por mais R$8,00? \n (1) SIM \n (2) NÂO");
int bebida = int.Parse(Console.ReadLine());
double totalbebida0 = (valor[0] + 8);
double totalbebida1 = (valor[1] + 8);
double totalbebida2 = (valor[2] + 8);
double totalbebida3 = (valor[3] + 8);
double totalbebida4 = (valor[4] + 8);
if (escolha == 0 && bebida == 2)
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[0]} que custa {valor[0].ToString("c")}");
}
if (escolha == 0 && bebida == 1 )
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[0]} que custa {valor[0].ToString("c")} mais uma bebida por R$8,00! \nTotal= {totalbebida0.ToString("c")} ");
}
if (escolha == 1 && bebida ==2)
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[1]} que custa {valor[1].ToString("c")}");
}
if (escolha == 1 && bebida == 1 )
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[1]} que custa {valor[1].ToString("c")} mais uma bebida por R$8,00! \nTotal= {totalbebida1.ToString("c")} ");
}
if (escolha == 2 && bebida ==2)
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[2]} que custa {valor[2].ToString("c")}");
}
if (escolha == 2 && bebida == 1 )
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[2]} que custa {valor[2].ToString("c")} mais uma bebida por R$8,00! \nTotal= {totalbebida2.ToString("c")} ");
}
if (escolha == 3 && bebida ==2)
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[3]} que custa {valor[3].ToString("c")}");
}
if (escolha == 3 && bebida == 1 )
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[3]} que custa {valor[3].ToString("c")} mais uma bebida por R$8,00! \nTotal= {totalbebida3.ToString("c")} ");
}
if (escolha == 4 && bebida ==2)
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[4]} que custa {valor[4].ToString("c")}");
}
if (escolha == 4 && bebida == 1 )
{
    System.Console.WriteLine($"VOCÊ ESCOLHEU {lanche[4]} que custa {valor[4].ToString("c")} mais uma bebida por R$8,00! \nTotal= {totalbebida4.ToString("c")} ");
}
if ( escolha != 0 && escolha != 1 && escolha != 2 && escolha != 3 && escolha != 4)
{
    System.Console.WriteLine("Opção de Lanche Inválida");
    goto _etq; 
}
      
Console.ReadKey();
