package com.company;

import java.util.*;
public class Main {
    public static void main(String args[]) {
        Scanner input = new Scanner(System.in);
        System.out.print("plaintext: ");
        String text = input.nextLine();
        System.out.print("Enter the key that the message will shift by (Give me a number!): ");
        int move = input.nextInt();
        String ciphertext = "";
        char letters;
        for(int i=0; i < text.length();i++)
        {
            // moves one character at a time
            letters = text.charAt(i);

            // if letter lies between a and z, same formular as p-k from instructions but this was easier
            if(letters >= 'a' && letters <= 'z')
            {
                // movesvletter down the alphabet
                letters = (char) (letters + move);
                // if move letter is greater than 'z'
                if(letters > 'z') {
                    // moves to starting position
                    letters = (char) (letters+'a'-'z'-1);
                }
                ciphertext = ciphertext + letters;
            }

            // if letters is between 'A'and 'Z'
            else if(letters >= 'A' && letters <= 'Z') {
                // shift letter
                letters = (char) (letters + move);

                // if move letters is greater than 'Z'
                if(letters > 'Z') {
                    //moves to starting position
                    letters = (char) (letters+'A'-'Z'-1);
                }
                ciphertext = ciphertext + letters;
            }
            else {
                ciphertext = ciphertext + letters;
            }

        }
        System.out.println("ciphertext : " + ciphertext);
    }
}
