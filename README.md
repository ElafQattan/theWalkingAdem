# theWalkingAdem
package com.company;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int T = input.nextInt();

        String[] Cases = new String[T]; // Create array with cases

        Cases[0] = input.nextLine();
        for (int i = 0; i < T; i++) {
            Cases[i] = input.nextLine(); // Enter every case
        }

        for (int i = 0; i < T; i++) {
            int counter = 0;
            for (int b = 0; b < Cases[i].length(); b++) {

                if (Cases[i].charAt(b) == 'U')
                    counter++;

                else if (Cases[i].charAt(b) == 'D')
                    break;
            }
            System.out.println(counter);
        }


    }
}
