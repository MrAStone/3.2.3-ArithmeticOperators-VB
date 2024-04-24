<pre lang=vb.net>
Module Module1

    Sub Main()
        ' Addition
        ' add two integers
        Dim num1, num2 As Integer
        num1 = 12
        num2 = 13
        Dim num3 As Integer = num1 + num2
        Console.WriteLine(num3)

        ' add two decimals
        Dim dNum1, dNum2, dNum3 As Double
        dNum1 = 3.1596
        dNum2 = 9.3642
        dNum3 = dNum1 + dNum2
        Console.WriteLine(dNum3)

        ' add differnt numerical data types
        dNum3 = num1 + dNum2
        Console.WriteLine(dNum3)
        num3 = dNum1 + num2
        Console.WriteLine(num3) ' this rounds the number (Rounding at .5 goes to nearest even number) as it is stored in Integer


        ' Subtraction
        ' Subtract two integers
        num3 = num1 - num2
        Console.WriteLine(num3)

        ' subtract two decimals
        dNum3 = dNum2 - dNum1
        Console.WriteLine(dNum3)

        'mixture
        dNum3 = num1 - dNum2
        Console.WriteLine(dNum3)
        num3 = dNum2 - num1 ' will round the result to integer value

        'Multiplication
        ' Integers
        num3 = num1 * num2
        Console.WriteLine(num3)
        ' Decimals
        dNum3 = dNum2 * dNum1
        Console.WriteLine(dNum3)
        ' Mixture
        dNum3 = num1 * dNum2
        Console.WriteLine(dNum3)
        num3 = dNum1 * num1
        Console.WriteLine(num3) ' will round the result to integer value

        'Real division
        'Division will produce the result as a real number but will convert it to the data type used
        'storing the result of division in an integer will round it
        'The same rules apply for rounding accountancy rounding will round .5 to the nearest even number
        '3.5 and 4.5 both round to 4
        num1 = 7
        num2 = 3
        num3 = num1 / num2
        Console.WriteLine(num3) ' 2

        dNum3 = num1 / num2
        Console.WriteLine(dNum3) ' 2.3333333333...

        'Integer division Including remainders
        ' a = b \ c 
        ' note the opposite direction of the division symbol
        'Produces whole number (Does not round) so how many times c can go into b
        num3 = num1 \ num2 ' 2
        Console.WriteLine(num3)
        num1 = 10
        num2 = 2
        num3 = num1 \ num2 ' 5
        Console.WriteLine(num3)

        ' Remainders
        ' Using MOD in VB.NET uses the word MOD
        num3 = num1 Mod num2
        Console.WriteLine(num3) ' 0 as there is no remainder dividing 10 by 2
        num1 = 7
        num2 = 3
        num3 = num1 Mod num2
        Console.WriteLine(num3) '1 as 7\3 has a remainder of 1

        ' In VB.NET the following is true
        ' 11 \ 2 = 5
        ' 11 / 2 = 5.5
        ' 11 MOD 2 = 1
        Console.WriteLine(11 \ 2)
        Console.WriteLine(11 / 2)
        Console.WriteLine(11 Mod 2)

    End Sub

End Module
