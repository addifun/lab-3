Поясненя 
Спочатку ми імпортуємо модуль sys. Це дозволить нам отримати аргументи командного рядка, які будуть передані скрипту.

Далі ми оголошуємо функцію find_pairs, яка приймає список чисел як вхідний параметр.

У функції find_pairs ми створюємо дві змінні: pairs - список для зберігання знайдених пар чисел, і seen - множину для відстеження чисел, які вже були переглянуті.

Потім ми проходимо через кожне число у вхідному списку numbers за допомогою циклу for. На кожній ітерації ми вираховуємо доповнення числа до 10 шляхом віднімання поточного числа від 10. Це зберігається у змінній complement.

Далі перевіряємо, чи знаходиться complement в множині seen. Якщо так, це означає, що ми знайшли пару чисел, сума яких дорівнює 10. Тоді ми створюємо кортеж (complement, num) і додаємо його до списку pairs.

Після цього ми додаємо поточне число num до множини seen, щоб врахувати його як вже переглянуте.

Після завершення циклу for ми повертаємо список pairs, який містить усі знайдені пари чисел.

У блоку if __name__ == "__main__": ми перевіряємо, чи скрипт виконується безпосередньо (а не імпортується як модуль). Це дає нам можливість запускати код, коли ми виконуємо файл pairs.py.
В цьому блоку ми отримуємо аргументи командного рядка, передані скрипту, за допомогою sys.argv[1:]. sys.argv - це список, який містить аргументи командного рядка, і sys.argv[1:] - це підрядок цього списку, який містить значення аргументів після імені файлу.

Потім ми перетворюємо отримані аргументи командного рядка у цілі числа, використовуючи генератор списку.

Після цього ми викликаємо функцію find_pairs зі списком чисел і зберігаємо результат у змінній pairs.

Нарешті, ми виводимо знайдені пари чисел, перебираючи їх у циклі for і використовуючи функцію print для виводу на екран.
