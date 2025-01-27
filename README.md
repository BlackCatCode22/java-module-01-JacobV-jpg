//1.HelloWorld
public class Main {

    public static void main(String[] args) {
        String str = "Hello World";

        System.out.println(str);

    }
}


//2.VarAndMath
public class Main {

    public static void main(String[] args) {

        int a = 9;
        int b = 10;
        int c = a + b;
        System.out.println("a = " + a);
        System.out.println("b = " + b);
        System.out.println("a+b="+c);
    }
}


//3.SimpleGreeting
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        String a = sc.next();

        System.out.println("Hi "+a);
    }
}

//4.FavNum
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        System.out.println("What's your favorite Number?");
        Scanner sc = new Scanner(System.in);
        String a = sc.next();
        System.out.println("So, your favorite is number "+a);

    }
}

//5.CircleArea
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        System.out.println("I will calculate the area of a circle for you. Type in the radius.");
        Scanner sc = new Scanner(System.in);
        double radius = sc.nextDouble();
        double area = Math.PI * radius * radius;
        System.out.println("The area of a circle is " + area + " :).");
    }
}

//6.TempConverter
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        System.out.println("I will convert a fahrenheit temperature to celsius.");
        System.out.println("Type in a number.");
        Scanner sc = new Scanner(System.in);
        int fahrenheit = sc.nextInt();
        int celsius = ((fahrenheit-32) *5/9);
        System.out.println("Its about "+celsius+" degree celsius");
    }
}

//7.Simple Calculator
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        System.out.println("Type in two numbers and some basic arithmetic with them.");
        System.out.println("Don't type in characters other than numbers.");
        System.out.println("First Number: ");
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        System.out.println("Second Number: ");
        Scanner scc = new Scanner(System.in);
        int b = scc.nextInt();
        int c = a + b;
        System.out.println("Adding these two numbers together gives you: "+c);
    }
}

//8.CharDetails
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        System.out.println("Enter in a character and I will find the unicode for it.");
        Scanner sc = new Scanner(System.in);
        char a = sc.next().charAt(0);
        int unicodeValue = Character.getNumericValue(a);
        System.out.println("The unicode value for this character is " + unicodeValue);
    }
}

//9.Madlibs
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {




        System.out.println("I will ask for a series of words and make a story out of them.");
        Scanner s = new Scanner(System.in);
        System.out.println("Type in a noun.");
        String noun = s.nextLine();
        System.out.println("Type in a Verb.");
        String verb= s.nextLine();
        System.out.println("Type in a adjective.");
        String adjective = s.nextLine();
        System.out.println("I can't believe that " + noun + " "+ verb + " that, which was quite " + adjective + "." );
    }
}

//10. Simple Interest
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        System.out.println("I will calculate simple interest for you.");
        Scanner sc = new Scanner(System.in);

        System.out.println("Enter a rate.");
        int r = sc.nextInt();
        double rate = r / 100.0;

        System.out.println("Enter principal.");
        int p = sc.nextInt();

        System.out.println("Enter the a time.");
        int n = sc.nextInt();


        double value = p * Math.pow(1 + rate, n);
        System.out.println("The amount of interest gained with principal is " + value);

    }
}
