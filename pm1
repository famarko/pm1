class Programmer:
    def __init__(self, last_name, num_programs, num_languages):
        self.last_name = last_name
        self.num_programs = num_programs
        self.num_languages = num_languages

    def quality(self):
        return self.num_programs * self.num_languages

    def display_info(self):
        print(f"Программист: {self.last_name}")
        print(f"Число программ: {self.num_programs}")
        print(f"Число языков программирования: {self.num_languages}")
        print(f"Качество (Q): {self.quality()}")


class AdvancedProgrammer(Programmer):
    def __init__(self, last_name, num_programs, num_languages, num_correct_programs):
        super().__init__(last_name, num_programs, num_languages)
        self.num_correct_programs = num_correct_programs

    def quality(self):
        base_quality = super().quality()
        return base_quality * self.num_correct_programs / self.num_programs

    def display_info(self):
        super().display_info()
        print(f"Число программ, которые работают правильно: {self.num_correct_programs}")
        print(f"Качество (Qp): {self.quality()}")


def main():
    #Ввод данных для базового класса
    print("Введите данные для программиста:")
    last_name = input("Фамилия: ")
    num_programs = int(input("Число программ: "))
    num_languages = int(input("Число языков программирования: "))

    prog = Programmer(last_name, num_programs, num_languages)
    print("\nОбъект класса 1-го уровня:")
    prog.display_info()

    #Ввод данных для класса 2-го уровня
    print("\nВведите данные:")
    last_name = input("Фамилия: ")
    num_programs = int(input("Число программ: "))
    num_languages = int(input("Число языков программирования: "))
    num_correct_programs = int(input("Число программ, которые работают правильно: "))

    adv_prog = AdvancedProgrammer(last_name, num_programs, num_languages, num_correct_programs)
    print("\nОбъект класса 2-го уровня:")
    adv_prog.display_info()

if __name__ == "__main__":
    main()
