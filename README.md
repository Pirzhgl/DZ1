package ru.levelp;

import java.util.Scanner;

/**
 * Created by Student-23 on 20.02.2016.
 */
public class Main {

    /**
     * Метод main выполняется при старте программы
     * @param args
     */
    public static void main(String[] args) {
        System.out.println("Решение линейного уравнения ax + b = 0");
        Scanner reader = new Scanner(System.in);
        System.out.println("Введите число a:");
        float linearEquation;
        float a, b;
        if (reader.hasNextInt()) {
            a = reader.nextInt();
            System.out.println("Введите число b:");
            if (reader.hasNextInt()) {
                b = reader.nextInt();
                if (a == 0 && b != 0)
                    System.out.println("Нет действительных решений уравнения");
                else if (a == 0 && b == 0)
                    System.out.println("Решение - любое число");
                else {
                    float x = -b / a;
                    System.out.println("x = " + x);
                }
            }
        }

    }


}
