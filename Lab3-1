# Lab-3
using System;
using System.Globalization;
using System.Linq;

class Program
{
    static void Main()
    {
        Console.Write("Введіть текстовий рядок: ");
        string input = Console.ReadLine();

        string lowercaseText = input.ToLower(new CultureInfo("uk-UA", false));
        Console.WriteLine($"Рядок з малими літерами: {lowercaseText}");

        string longestWord = FindLongestWord(lowercaseText);
        Console.WriteLine($"Найдовше слово: {longestWord}");
    }

    static string FindLongestWord(string text)
    {
        string[] words = text.Split(new[] { ' ', '.', ',', '!', '?', ';', ':' }, StringSplitOptions.RemoveEmptyEntries);
        return words.OrderByDescending(word => word.Length).FirstOrDefault();
    }
}
