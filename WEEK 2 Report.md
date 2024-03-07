```
class StuData:
    def __init__(self, filename):
        self.data = []
        with open(filename, 'r') as file:
            for line in file:
                line = line.strip().split()
                name, stu_num, gender, age = line
                age = int(age)
                self.data.append([name, stu_num, gender, age])

    def AddData(self, name, stu_num, gender, age):
        self.data.append([name, stu_num, gender, age])

    def SortData(self, attribute):
        attribute_dict = {'name': 0, 'stu_num': 1, 'gender': 2, 'age': 3}
        index = attribute_dict[attribute]
        self.data.sort(key=lambda x: x[index])

    def ExportFile(self, filename):
        with open(filename, 'w') as file:
            for student in self.data:
                file.write(' '.join(str(attr) for attr in student) + '\n')
```