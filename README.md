# lab
# Основной класс
class Labzad1():
    def __init__(self):
        while 1:
            # Инициализация вспомогательного модуля как поля основного класса
            self.Core = Lab1Core()
            print('\nВведите два числа и знак:')
            self.k = int(input())
            self.f = int(input())
            self.i = input()
            self.k = self.Core.Calculate(self.k, self.f, self.i)
            print(' = ', self.k)
            print('\nДля продолжения введите 1 \nДля выхода введите 2')
            p = input()
            if p == '2':
                break;
                from modules.lab2Modules import Lab2Core


# Основной класс
class Labzad2():
    def __init__(self):
        while 1:
            # Инициализация вспомогательного модуля как поля основного класса
            self.Core = Lab2Core()
            print('\nВведите число:')
            self.Input = input()
            self.Output = self.Core.Sqrt(float(self.Input))
            print(round(self.Output, 5))
            print('\nДля продолжения введите 1 \nДля выхода введите 2')
            p = input()
            if p == '2':
                break;

# Основной класс
class Labzad3():
    def __init__(self):
        while 1:
            # Инициализация вспомогательного модуля как поля основного класса
            self.Core = Lab3Core()
            self.Result = self.Core.Calculate()
            print('Для прогрессии ')
            print(self.Core.Poly)
            print('полином будет равен ')
            print(self.Result)
            print('\nДля продолжения введите 1 \nДля выхода введите 2')
            p = input()
            if p == '2':
                break;
                # Основной класс
class Lab4App():
    def __init__(self):
        while 1:
            # Инициализация вспомогательного модуля как поля основного класса
            self.Core = Lab4Core()
            print('Введите X:')
            # Получаем скользящую кривую
            self.Result = self.Core.Calculate(input())
            print('Скользящая кривая: ')
            print(self.Result)
            # Строим график
            self.Core.BuildGraphic()
            print('\nДля продолжения введите 1 \nДля выхода введите 2')
            p = input()
            if p == '2':
                break;
# Основной класс
class Lab5App():
    def __init__(self):
        while 1:
            # Инициализация вспомогательного модуля как поля основного класса
            self.Core = Lab5Core()
            print('Обрабатываем информацию с сервера...')
            self.Core.DataBind()
            self.Core.SpamCheck()
            print('Среднее значение X-DSPAM-Confidence = ' + str(self.Core.SR_Spam))
            print('Стоит заблокировать - ' + self.Core.BanUser.name)
            self.Core.BuildGraph()
            print('\nДля продолжения введите 1 \nДля выхода введите 2')
            p = input()
            if p == '2':
                break;

