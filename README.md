# Hello-World-
public class Ugadaika {
 
 
    public static void main(String[] args) {
        int min, max;
        min = 0;
        max = 100;
        Random rand = new Random(100);
        System.out.println("Call a number from 1 to 100 ");
        System.out.println(" ");
        Scanner in = new Scanner(System.in);
        int number = in.nextInt();
        System.out.println("Your choice is: " + number);
 
        int guess = rand.nextInt(96);
        System.out.println("Is it..If not..press M(More), L(Less), Y(Yes)" + guess);
        Scanner gg = new Scanner(System.in);
        System.out.println("Enter string: ");
        Char str = in.nextLine();
 
 
 
            while (guess != number) {
                  if (str == 'Y') {
            System.out.println("You wonn");
                  }else
                  if (str == 'L') {
                    max = guess;
                    guess = guess - (max - min);
                } else if (str == 'M') {
                    min = guess;
                    guess = guess + (max - min);
                } //else break;
                System.out.print(guess + " ");
                System.out.println();
            }
            }
 
 
    }
