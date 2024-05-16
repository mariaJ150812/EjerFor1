using EjerFor1.Class;

EjerciciosFor1 ejerciciosFor1 = new EjerciciosFor1();

ejerciciosFor1.EjerFor1();

Console.Read();

namespace EjerFor1.Class
{
    public class EjerciciosFor1
    {
        public void EjerFor1()
        {
            Console.WriteLine("Ingrese la cantidad de nmueros enteros que desea verificar:");
            int cantidad = Convert.ToInt32(Console.ReadLine());

            int contador = 0;

            for (int i = 0; i < cantidad; i++)
            {
                Console.Write($"Ingrese el numero {i + 1}: ");
                int numero = Convert.ToInt32(Console.ReadLine());

                if (numero >= 1000)
                {
                    contador++;
                }
            }

            Console.WriteLine($"La cantidad de numeros mayores o iguales a 1000 es: {contador}");
        }
    }
}
