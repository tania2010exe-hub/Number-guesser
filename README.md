# Number-guesser
/*I decided to learn C# so now iv put the stuff iv learnt to use

first i set a constant value which is 'number' which is the number were guessing for since i dont know how to generate radom numbers yet,
i then set 'guess' as a int16 as it doesnt need to be a big value,
i then used do/while to create a loop to ensure user can have many chances at guessing,
i used switch instead of else/if because i only needed to check the guess value.
*/

'''const short number = 2;
short guess;

do
{
    
    guess = Convert.ToInt16(Console.ReadLine());
    switch (guess)
    {
        case short n when n > number:
            Console.WriteLine("too high");
            break;

        case short n when n < number:
            Console.WriteLine("too low");
            break;

        default:
            Console.WriteLine("you got it!");
            break;

    }


} while (guess!=number);'''
