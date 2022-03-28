using System;

class Matrix
{
    static void Main(string[] args)
    {
        int[,] Matrix = new int[3, 3];
        Random random = new Random();

        for (int ElementsLength = 0; ElementsLength < Matrix.GetLength(0); ++ElementsLength)
        {
            for (int ElementsHeight = 0; ElementsHeight < Matrix.GetLength(1); ++ElementsHeight)
            {
                Matrix[ElementsLength, ElementsHeight] = random.Next();
            }
        }

        for (int Length = 0; Length < Matrix.GetLength(0); ++Length)
        {
            for (int Height = 0; Height < Matrix.GetLength(1); ++Height)
            {
                Console.Write(Matrix[Length, Height] + "\t");
            }
            Console.WriteLine();
        }

    }
}

