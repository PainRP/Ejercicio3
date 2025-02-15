# Ejercicio3
```csharp
    int num1,num2,selec;
void resultados(int resultados){
    Console.WriteLine($"El resultado es: {resultados}");
}
void resultadosFLOAT(float resultados){
    Console.WriteLine("El resultado es: "+resultados);
}

int suma (int n1, int n2){
    int resultado = 0;
    resultado = n1+n2;
    return resultado;
}

int resta (int n1, int n2){
    int resultado = 0;
    resultado = n1-n2;
    return resultado;
}

int multiplicacion (int n1, int n2){
    int resultado = 0;
    resultado = n1*n2;
    return resultado;
}

float division (int n1, int n2){
    float resultado = 0;
    resultado = (float)n1/n2;
    return resultado;
}

Console.WriteLine("Ingrese el primer numero: ");
num1 = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Ingrese el segundo numero: ");
num2 = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Ingrese lo que se quiere hacer (numero). \n1. suma \n2. resta \n3. multiplicacion \n4. division ");
selec = Convert.ToByte(Console.ReadLine());

switch (selec){
    case 1:
        int respuesta = suma(num1,num2);
        resultados(respuesta);
    break;
    case 2:
        int respuesta2 = resta(num1,num2);
        resultados(respuesta2);
    break;
    case 3:
        int respuesta3 = multiplicacion(num1,num2);
        resultados(respuesta3);
    break;
    case 4:
        float respuesta4 = division(num1,num2);
        resultadosFLOAT(respuesta4);
    break;   
    default:
        Console.WriteLine("Ingrese la opcion correcta");
    break; 
}
```
