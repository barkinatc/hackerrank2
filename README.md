class Solution
{
    public static void Main(string[] args)
    {
        var mealCost = double.Parse(Console.ReadLine());
        var tipPercent = int.Parse(Console.ReadLine());
        var taxPercent = int.Parse(Console.ReadLine());

        var tip = tipPercent * mealCost / 100;
        var tax = taxPercent * mealCost / 100;

        var totalCost = Math.Round(tip + tax + mealCost);
        Console.WriteLine(totalCost);
    }
}
