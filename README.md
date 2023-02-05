# hazir_metotlar_string
using System;

namespace MyApp // Note: actual namespace depends on the project name.
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string degisken="Dersimiz CSharp, Hoşgeldiniz";
            string degisken2="Dersimiz CSharp";
            //lenght
            Console.WriteLine(degisken.Length);
            //ToUpper , ToLower
            Console.WriteLine(degisken.ToUpper());
            Console.WriteLine(degisken.ToLower());
            //Concat
            Console.WriteLine(string.Concat(degisken," merhaba!"));
            //compare , compareTo
            Console.WriteLine(degisken.CompareTo(degisken2));//0,1,-1
            Console.WriteLine(string.Compare(degisken,degisken2,false));//true dersek büyük küçük harf duyarsız hale gelir.
            Console.WriteLine(string.Compare(degisken,degisken2,true));

            //contains
            Console.WriteLine(degisken.Contains(degisken2));// değişkenin içinde değişken 2 var mı ?
            Console.WriteLine(degisken.EndsWith("Hoşgeldiniz"));
            Console.WriteLine(degisken.StartsWith("merhaba!"));
            //indexof
            Console.WriteLine(degisken.IndexOf("CS"));
            Console.WriteLine(degisken.LastIndexOf("i"));

            //Insert
            Console.WriteLine(degisken.Insert(0," merhaba!"));

            //padLeft ,PadRight
            Console.WriteLine(degisken + degisken2.PadLeft(30)); 
            Console.WriteLine(degisken + degisken2.PadLeft(30,'*'));
             Console.WriteLine(degisken.PadRight(50) + degisken2);
            Console.WriteLine(degisken.PadRight(50,'-') + degisken2);

            //remove
            Console.WriteLine(degisken.Remove(10));
            Console.WriteLine(degisken.Remove(5,3));
            Console.WriteLine(degisken.Remove(0,1));

            //replace
            Console.WriteLine(degisken.Replace("CSharp","c#"));
             Console.WriteLine(degisken.Replace(" ","*"));
            //split
            Console.WriteLine(degisken.Split(" ") [1]);
            // substring
            Console.WriteLine(degisken.Substring(4));
            Console.WriteLine(degisken.Substring(4,6));

        }
    }
}
