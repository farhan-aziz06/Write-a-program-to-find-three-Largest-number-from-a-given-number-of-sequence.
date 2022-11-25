# Write-a-program-to-find-three-Largest-number-from-a-given-number-of-sequence.
Write a program to find three Largest number from a given number of sequence. Java Program

import java.util.Scanner;

public class Main {
    public static void main(String[] args){
  
        Scanner console = new Scanner(System.in);
        int counter =0;
        int num;
        int Largest = 0;
        int Largest1=0;
        int Largest2=0;
        while (counter<10){
            num = console.nextInt();

            if(num>Largest){
                Largest2 = Largest1;
                Largest1 = Largest;
                Largest=num;
            } else if (num>Largest1) {
                Largest2=Largest1;
                Largest1=num;

            } else if (num>Largest2) {
                Largest2=num;
            }

            counter++;
        }
        System.out.println(Largest +" is 1st largest numbers: ");
        System.out.println(Largest1 +" is 2nd largest numbers: ");
        System.out.println(Largest2 +" is 3rd largest numbers: ");

    }
}
