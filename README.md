# Super-Keword-in-python
Super Keyword Using inPython

#Super Keyword

class College:
    def __init__(self,college_name,college_address):
        self.college_name=college_name
        self.college_address=college_address

    def display(self):
        print (f"College_name:{self.college_name}")
        print (f"College_Address :{self.college_address}")


class Student(College):
    def __init__(self,college_name,college_address,student_name,student_pass):
        super().__init__(college_name,college_address)
        self.student_name=student_name
        self.student_pass=student_pass

    def display(self):
        super().display()
        print(f"student_name:{self.student_name}")
        print(f"student_pass:{self.student_pass}")
student=Student("Wise","Tpg","Rk","2025")


student.display()




