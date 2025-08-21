C++ Konsolenanwendung für die Spielstandverfolgung

____________________________________________________________________
![ее](https://github.com/user-attachments/assets/d00c52fb-64c2-4d70-9e8e-cb337d815d89)
_______________________________________________________________________
___________________________________________________________________
![_33](https://github.com/user-attachments/assets/7db14474-c02a-4da4-a052-e9e74fa4e29f)

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
____________________________________________________________
________________________________________________________________


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
___________________________________________________________________________________________

____________________________________________________________________
___________________________________________________________________
#include <stdio.h>  // Стандартные функции ввода/вывода
#include <conio.h>  // Консольный ввод/вывод (используется для getch())
#include <locale.h> // Для поддержки локализации (русского языка)
#include <math.h>   // Математические функции (не используется в коде)
#include <windows.h> // Функции Windows API (не используется в коде)
_______________________________________________________________________
_________________________________________________________________________

#include <stdio.h>     // Стандартные функции ввода/вывода
#include <conio.h>      // Для getch() (можно заменить на более современные альтернативы)
#include <locale.h>     // Для поддержки локализации

int main()              // Явно указан тип возвращаемого значения
{
    setlocale(LC_ALL, "rus");  // Установка русской локали
    
   ![Консольное приложение C++ для отслеживания результатов - ](https://github.com/user-attachments/assets/205db9fd-75e9-406e-89c1-2b83bb5fb3c5)

