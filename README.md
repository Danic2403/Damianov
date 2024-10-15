# Damianov
Dani
Масива който се дели на 2 долу

int[] array = new int[10];
    for (int i = 0; i < 10; i++)
    {
    array[i] = int.Parse(Console.ReadLine());
    }
int n = int.Parse(Console.ReadLine());
int left = 0;
int right = array.Length - 1;
    while (left <= right)
    {
        int middle = (left + right) / 2;
        if (array[middle] == n)
        {
            Console.WriteLine($"Числото {n} е намерено на позиция {middle}.");
            left = right + 1; 
        }
        else if (array[middle] < n)
        {
            left = middle + 1;
        }
        else
        {
            right = middle - 1;
        }
    }
    if (left > right)
    {
        Console.WriteLine($"Числото {n} не е намерено в масива.");
    }
    
    
