# Decrypting-Message
Just another repository
using System;

namespace _13.Decrypting_Messages
{
    class Program
    {
        static void Main(string[] args)
        {
            int key = int.Parse(Console.ReadLine());
            int n = int.Parse(Console.ReadLine());
            string word = string.Empty;

            for (int i = 0; i < n; i++)
            {
                char letter = char.Parse(Console.ReadLine());

                int transformLetters = letter + key;
                char letters = (char)transformLetters;
                word += letters;
            }

            Console.WriteLine(word);
        }
    }
}
