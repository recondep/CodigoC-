using System;

// La clase Circulo representa un círculo y contiene propiedades para su radio.
public class Circulo
{
    // Propiedad que almacena el radio del círculo
    public double Radio { get; set; }

    // Constructor que inicializa el radio
    public Circulo(double radio)
    {
        Radio = radio;
    }

    // CalcularArea es una función que devuelve un valor double, se utiliza para calcular el área de un círculo.
    public double CalcularArea()
    {
        return Math.PI * Radio * Radio; // Fórmula: π * r^2
    }

    // CalcularPerimetro es una función que devuelve un valor double, se utiliza para calcular el perímetro de un círculo.
    public double CalcularPerimetro()
    {
        return 2 * Math.PI * Radio; // Fórmula: 2 * π * r
    }
}

// La clase Rectangulo representa un rectángulo y contiene propiedades para su base y altura.
public class Rectangulo
{
    // Propiedades que almacenan la base y altura del rectángulo
    public double Base { get; set; }
    public double Altura { get; set; }

    // Constructor que inicializa la base y altura
    public Rectangulo(double baseRect, double altura)
    {
        Base = baseRect;
        Altura = altura;
    }

    // CalcularArea es una función que devuelve un valor double, se utiliza para calcular el área de un rectángulo.
    public double CalcularArea()
    {
        return Base * Altura; // Fórmula: base * altura
    }

    // CalcularPerimetro es una función que devuelve un valor double, se utiliza para calcular el perímetro de un rectángulo.
    public double CalcularPerimetro()
    {
        return 2 * (Base + Altura); // Fórmula: 2 * (base + altura)
    }
}

// Ejemplo de uso
class Program
{
    static void Main(string[] args)
    {
        // Crear una instancia de Circulo
        Circulo circulo = new Circulo(5);
        Console.WriteLine($"Área del círculo: {circulo.CalcularArea()}");
        Console.WriteLine($"Perímetro del círculo: {circulo.CalcularPerimetro()}");

        // Crear una instancia de Rectangulo
        Rectangulo rectangulo = new Rectangulo(4, 6);
        Console.WriteLine($"Área del rectángulo: {rectangulo.CalcularArea()}");
        Console.WriteLine($"Perímetro del rectángulo: {rectangulo.CalcularPerimetro()}");
    }
}
 CodigoC-
Tareas 2 utilizando GitHub
