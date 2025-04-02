# Class
```python
class People:  
    def __init__(self, name, age):  
        self.name = name  
        self.age = age  
  
    def 자기소개(self):  
        print(f"제 이름은 {self.name}이구요, 나이는 {self.age}에요.")  
  
a = People("김영환", 20)  
b = People("황서연", 13)  
a.자기소개()  
b.자기소개()
```