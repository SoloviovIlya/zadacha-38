// Задайте массив вещественных чисел. Найдите разницу между максимальным и минимальным элементов массива.
//[3 7 22 2 78] -> 76

void MaxMin(int[] a, int n)

{

    int max = a[0];
    
    int min = a[0];
    
    for (int i=0;i<n;i++)
    
    {
    
       if (a[i]> max)
       
       {
        max = a[i];
       }
       
        if (a[i]< min)
        
       {
        min = a[i];
       }
       
    }
    
    Console.WriteLine($"Разница между максимальным и минимальным элементами равна {max - min}");
    
}

int n = new Random().Next(5,11);

int[] a = new int[n];

for (int i = 0; i<n; i++)

{
    a[i] = new Random().Next(1,100);
    
    Console.WriteLine(a[i]);
    
}

MaxMin(a,n);
