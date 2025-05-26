import pyautogui
import time
import sys

def main():
    # Немного подождем, чтобы дать пользователю время переключиться на окно приложения
    print("Программа начнется через 5 секунд.")
    time.sleep(5)

    # Имитация нажатия клавиш Win + R
    pyautogui.hotkey('win', 'r')

    # Дополнительно можно ввести команду (например, 'notepad')
    time.sleep(1)  # Ждем секунду, чтобы окно 'Выполнить' успело открыться
    pyautogui.write('notepad')  # Пишем 'notepad'
    pyautogui.press('enter')  # Нажимаем 'Enter'

if __name__ == "__main__":
    main()
