# DZ-end.string
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner text = new Scanner(System.in);
        System.out.println("Введите текст :");

        String a = text.nextLine();

        System.out.println(" Введите слово которое желаете вырезать :");
        String word = text.nextLine();

        int start = a.indexOf(word);
        String befor = a.substring(0,start);

        String after = a.substring(start + word.length());
        String result = befor + after;

        System.out.println(result);
    }
}
