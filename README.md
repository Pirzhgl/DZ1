package ru.levelp;

import java.util.Scanner;

/**
 * Created by Student-23 on 19.02.2016.
 */
public class Main {

    /**
     * Метод main выполняется при старте программы
     * @param args
     */
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        System.out.println("Введите a:\t");

        float a, b;
        if (reader.hasNextInt()) {
            a = reader.nextInt();
            System.out.println("Введите b:");
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

    /*
    Домашнее задание
    дома пишете программу для решения линейных уравнений

    a*x + b = 0
    1) Линейные уравнения
    2) Найти как пользователю вводить в командную строку данные
    3) Пользователь вводит а и b с клавиатуры, после чего выводится ответ:
    x = ответ
    4) читать про типы данных и дапазоны значений в Java

    с помощью каких команд
     */
}
