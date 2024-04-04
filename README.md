# conditions
using System;

public class Program
{
  public static void Main(String [] args)
  {
    // int num =0;
    int  UserEntry1 = 0;
    int  UserEntry2 = 0;
    int  UserEntry3 = 0;
    
    // bool IsOk1 = false;
    // bool IsOk2 = false;
    // bool IsOk3 = false;
    
    while ( UserEntry3 != 10000 )
    {
       Console.WriteLine("Limite inférieure Entrez un nombre ou q pour quitter.");
      string ligne = Console.In.ReadLine();
      if(  ligne != "q" ){
      try
      {
          UserEntry1= int.Parse(ligne);
      }
      catch (Exception e)
      {
          Console.Out.WriteLine("L'erreur suivante s'est produite : " + e.Message);
      }
        }else{ Environment.Exit(0);}

       Console.WriteLine("Limite supérieure Entrez un nombre ou q pour quitter.");
      string ligne2 = Console.In.ReadLine();
      if (  ligne2 != "q" ){
      try
      {
        UserEntry2 = int.Parse(ligne2);
      }
      catch (Exception e)
      {
          Console.Out.WriteLine("L'erreur suivante s'est produite : " + e.Message);
      }
        }else{ Environment.Exit(0);}
       Console.WriteLine("Entrez un nombre ou q pour quitter.");
      string ligne3 = Console.In.ReadLine();
      if(  ligne3 != "q" ){
      try
      {
        UserEntry3 = int.Parse(ligne3);
      }
      catch (Exception e)
      {
          Console.Out.WriteLine("L'erreur suivante s'est produite : " + e.Message);
      }
        }else{ Environment.Exit(0);}
       Console.Out.WriteLine("x = " + UserEntry3);
       // IsOk1 = int.TryParse(UserEntry1 , out num);
       // IsOk2 = int.TryParse(UserEntry2 , out num);
       // IsOk3 = int.TryParse(UserEntry3 , out num);
       if (UserEntry3 < UserEntry1){
          Console.Out.WriteLine("You have entered" + UserEntry3 + "which is lower than" + UserEntry1 + "which is the minimum");

         
       }
      if (UserEntry3 > UserEntry2){
          Console.Out.WriteLine("You have entered" + UserEntry3 + "which is higher than" + UserEntry2 + "which is the maximum");


       }
    }
    
  }
}