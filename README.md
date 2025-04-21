C/C++
____________________________________________________________________
___________________________________________________________________

C++ Konsolenanwendung für die Spielstandverfolgung

Diese C++-Konsolenanwendung dient als digitale Anzeigetafel zur Verfolgung der Punkte zwischen zwei konkurrierenden Mannschaften. Sie implementiert ein schleifenbasiertes Menüsystem, das Benutzern folgende Funktionen bietet:

Aktuellen Spielstand in Echtzeit anzeigen

Punkte für beide Mannschaften verwalten (mit Optionen für 1, 2 oder 3 Punkte)

Das Spiel beenden und Endergebnisse anzeigen

Technische Merkmale:

Echtzeit-Scoreboard mit dynamischer Anzeige

Intuitive Menüführung mit zweistufiger Auswahl:

Hauptmenü zur Mannschaftsauswahl

Untermenü zur Punktevergabe

Klare visuelle Darstellung des Spielstands

Erweiterte Funktionen:

Punktestandsmanagement:

Verwendung von Integer-Variablen für die Punktzählung

Flexible Punktevergabe-Systematik (1-3 Punkte pro Aktion)

Programmsteuerung:

Do-While-Schleife für kontinuierlichen Betrieb

Option zum ordnungsgemäßen Spielabbruch

Anwendungsbeispiel:

Programmstart mit Anzeige des Initialstands (0:0)

Benutzer wählt Mannschaft 1 → 3 Punkte

Aktualisierter Spielstand (3:0)

Benutzer wählt Mannschaft 2 → 2 Punkte

Aktualisierter Spielstand (3:2)

Spielende mit Anzeige des Endergebnisses

Diese Lösung bietet eine robuste Basis für die Spielstandverfolgung, die durch sportspezifische Anpassungen 
(z.B. für Basketball oder Volleyball) erweitert werden kann, einschließlich der Möglichkeit, sportspezifische Punkteregeln und Zählweisen zu implementieren.
__________________________________________________________________


This C++ console application serves as a digital scoreboard for tracking points between two competing teams. 
It implements a loop-based menu system that allows users to:
View the current score in real-time
Add points to either team (with 1, 2, or 3 point options)
Terminate the match and display final results
________________________________________________________________

Консольное приложение C++ для отслеживания результатов

Это консольное приложение на C ++ служит цифровым табло для отслеживания очков между двумя соревнующимися командами. В нем реализована циклическая система меню, которая предоставляет пользователям следующие функции:

Просмотр текущего игрового процесса в режиме реального времени

Управление очками для обеих команд (с возможностью набрать 1, 2 или 3 очка)

Выйти из игры и просмотреть окончательные результаты

Технические характеристики:

Табло в реальном времени с динамическим отображением

Интуитивно понятное меню с двухэтапным выбором:

Главное меню для выбора команды

Подменю для начисления очков

Четкое визуальное представление игрового процесса

Расширенные возможности:

Управление состоянием очков:

Использование целочисленных переменных для подсчета очков

Гибкая система начисления баллов (1-3 балла за действие)

Управление программами:

Цикл выполнения во время непрерывной работы

Возможность правильного прекращения игры

Пример использования:

Запуск программы с указанием начального уровня (0:0)

Пользователь выбирает команду 1 → 3 очка

Обновленный счет матча (3:0)

Пользователь выбирает команду 2 → 2 очка

Обновленный счет матча (3:2)

Окончание игры с отображением конечного результата

Это решение обеспечивает надежную основу для отслеживания счета, которая может быть расширена за счет специальных настроек 
(например, для баскетбола или волейбола), включая возможность реализации правил подсчета очков и способов подсчета для конкретных видов спорта.



____________________________________________________________________
___________________________________________________________________
#include <stdio.h>  // Стандартные функции ввода/вывода
#include <conio.h>  // Консольный ввод/вывод (используется для getch())
#include <locale.h> // Для поддержки локализации (русского языка)
#include <math.h>   // Математические функции (не используется в коде)
#include <windows.h> // Функции Windows API (не используется в коде)
_______________________________________________________________________

#include <stdio.h>     // Стандартные функции ввода/вывода
#include <conio.h>      // Для getch() (можно заменить на более современные альтернативы)
#include <locale.h>     // Для поддержки локализации

int main()              // Явно указан тип возвращаемого значения
{
    setlocale(LC_ALL, "rus");  // Установка русской локали
    
    int score1 = 0, score2 = 0;  // Счет команд
    int menu1, menu2;            // Переменные для меню
    int fExit = 1;               // Флаг продолжения работы (1 - продолжать, 0 - выход)
    
    do
    {
        // Вывод текущего счета
        printf("Текущий счет %d : %d\n", score1, score2);
        
        // Основное меню
        printf("1. Команда 1\n");
        printf("2. Команда 2\n");
        printf("3. Завершение матча\n");
        printf("Введите номер пункта меню: ");
        scanf("%d", &menu1);
        
        switch(menu1)
        {
            case 1:  // Добавление очков для команды 1
                printf("\nВыберите количество очков для команды 1:\n");
                printf("1. Одно очко\n");
                printf("2. Два очка\n");
                printf("3. Три очка\n");
                printf("Ваш выбор: ");
                scanf("%d", &menu2);
                
                switch(menu2)
                {
                    case 1: score1 += 1; break;
                    case 2: score1 += 2; break;
                    case 3: score1 += 3; break;
                    default: 
                        printf("Неверный выбор количества очков!\n");
                        system("pause");
                        break;
                }
                break;
                
            case 2:  // Добавление очков для команды 2 (теперь реализовано)
                printf("\nВыберите количество очков для команды 2:\n");
                printf("1. Одно очко\n");
                printf("2. Два очка\n");
                printf("3. Три очка\n");
                printf("Ваш выбор: ");
                scanf("%d", &menu2);
                
                switch(menu2)
                {
                    case 1: score2 += 1; break;
                    case 2: score2 += 2; break;
                    case 3: score2 += 3; break;
                    default: 
                        printf("Неверный выбор количества очков!\n");
                        system("pause");
                        break;
                }
                break;
                
            case 3:  // Завершение матча (теперь реализовано)
                printf("\nМатч завершен! Финальный счет: %d : %d\n", score1, score2);
                fExit = 0;  // Устанавливаем флаг для выхода из цикла
                break;
                
            default:
                printf("Неверный выбор пункта меню!\n");
                system("pause");
                break;
        }
        
        system("cls");  // Исправлено с "sls" на "cls" - очистка экрана
        
    } while(fExit == 1);  // Цикл выполняется, пока fExit равен 1

    printf("\nНажмите любую клавишу для выхода...");
    getch();  // Ожидание нажатия клавиши перед выходом
    
    return 0;  // Явный возврат успешного статуса
}
