# FruitShop

import java.util.Scanner;

public class P28_FruitShop {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String fruit = scanner.nextLine();
        String dayOfWeek = scanner.nextLine();
        double ammount = Double.parseDouble(scanner.nextLine());

        double bananaWeekPrice = 2.50;
        double appleWeekPrice = 1.20;
        double orangeWeekPrice = 0.85;
        double grapefruitWeekPrice = 1.45;
        double kiwiWeekPrice = 2.70;
        double pineappleWeekPrice = 5.50;
        double grapesWeekPrice = 3.85;

        double bananaWeekendPrice = 2.70;
        double appleWeekendPrice = 1.25;
        double orangeWeekendPrice = 0.90;
        double grapefruitWeekendPrice = 1.60;
        double kiwiWeekendPrice = 3.00;
        double pineappleWeekendPrice = 5.60;
        double grapesWeekendPrice = 4.20;

        if (dayOfWeek.equalsIgnoreCase("monday") || dayOfWeek.equalsIgnoreCase("tuesday")
                || dayOfWeek.equalsIgnoreCase("wednesday")
                || dayOfWeek.equalsIgnoreCase("thursday")
                || dayOfWeek.equalsIgnoreCase("friday")) {

            switch (fruit) {
                case "banana":
                    System.out.printf("%.2f", ammount * bananaWeekPrice);
                    break;

                case "apple":
                    System.out.printf("%.2f", ammount * appleWeekPrice);
                    break;

                case "orange":
                    System.out.printf("%.2f", ammount * orangeWeekPrice);
                    break;

                case "kiwi":
                    System.out.printf("%.2f", ammount * kiwiWeekPrice);
                    break;

                case "grapefruit":
                    System.out.printf("%.2f", ammount * grapefruitWeekPrice);
                    break;

                case "pineapple":
                    System.out.printf("%.2f", ammount * pineappleWeekPrice);
                    break;

                case "grapes":
                    System.out.printf("%.2f", ammount * grapesWeekPrice);
                    break;

                    default:
                        System.out.println("error");
            }


        } else if (dayOfWeek.equalsIgnoreCase("saturday") || dayOfWeek.equalsIgnoreCase("sunday")) {

            switch (fruit) {
                case "banana":
                    System.out.printf("%.2f", ammount * bananaWeekendPrice);
                    break;

                case "apple":
                    System.out.printf("%.2f", ammount * appleWeekendPrice);
                    break;

                case "orange":
                    System.out.printf("%.2f", ammount * orangeWeekendPrice);
                    break;

                case "kiwi":
                    System.out.printf("%.2f", ammount * kiwiWeekendPrice);
                    break;

                case "grapefruit":
                    System.out.printf("%.2f", ammount * grapefruitWeekendPrice);
                    break;

                case "pineapple":
                    System.out.printf("%.2f", ammount * pineappleWeekendPrice);
                    break;

                case "grapes":
                    System.out.printf("%.2f", ammount * grapesWeekendPrice);
                    break;

                    default:
                        System.out.println("error");

            }

        }
        else {
            System.out.println("error");
        }

    }
}
