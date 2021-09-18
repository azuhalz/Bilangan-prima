# Bilangan-prima
package com.pemdas;

import java.util.Scanner;

public class bilanganPrima {
    
    public static void main(String[] args) {
        
        Scanner in = new Scanner(System.in);
        
        int angka = in.nextInt();
        int bagi = 0;
        
        for (int i = 1; i <= angka; i++){
            if (angka % i == 0){
                bagi++;
            }
        }
        if (bagi == 2){
            System.out.printf("%d merupakan bilangan prima\n", angka);
        } else {
            System.out.printf("%d bukan merupakan bilangan prima\n", angka);
        }
    }
}
