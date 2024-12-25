# MISPIS3

Правильная ссылка на код: https://github.com/artomas/MISPIS3ATT

1: Идентификация классов

University, Faculty, Institute, Dean, Employee, ResearchEmployee, AdministrativePersonal, Project, Course, Lecturer

2: Идентификация атрибутов
University: name;
Faculty: name;
Institute: name, address;
Dean: name, socialSecurityNumber, e-mail;
Employee: socialSecurityNumber, name, e-mail;
ResearchEmployee: researchArea;
Project: name, hours, startingDate, endDate;
Course: id, name, weeklyDuration;

3: Идентификация отношений
University → Faculty
  Композиция (сильная зависимость)

Faculty → Institute
  Композиция

Faculty → Dean
  Ассоциация

Institute → ResearchEmployee
  Ассоциация

ResearchEmployee → Project 
  Агрегация

ResearchEmployee → Course (Lecturer)
  Обобщение

Employee → ResearchEmployee, AdministrativePersonal
  Обобщение

4: Идентификация методов классов
University
  addFaculty(faculty: Faculty)

Faculty
  addInstitute(institute: Institute)

ResearchEmployee
  assignProject(project: Project)

Course
  addLecturer(lecturer: Lecturer)


5,6: Генерация кода (на языке Python) и его компиляция + Unit тест. Местоположение - https://github.com/artomas/MISPIS3ATT
![image](https://github.com/user-attachments/assets/dc2dbea0-e396-4c7c-80b3-eef61fb12a5d)
![image](https://github.com/user-attachments/assets/0632bbb6-36d9-48dc-a42f-393ba7cc6885)


7:Обратный инженеринг и генерация модели
![image](https://github.com/user-attachments/assets/35845172-5e0c-45d4-8e75-2b740a682901)

Шаг 8: Поведенческие диаграммы
Диаграмма прецедентов
![image](https://github.com/user-attachments/assets/f5a1c90a-9f63-4b57-9223-68224ca42ec3)

Диаграмма последовательностей
![image](https://github.com/user-attachments/assets/274b7e83-31a8-49e3-8c2c-ef9ae10407b7)

Диаграмма состояний
![image](https://github.com/user-attachments/assets/2dff3fb8-a3fa-4d2c-b650-b8f56103b5f4)

Диаграмма активностей
![image](https://github.com/user-attachments/assets/a4172dbb-137a-4808-b299-119534372bf7)


Результат:
Спроектирована и реализована информационная система с применением UML моделирования.
Получены статические и поведенческие диаграммы, демонстрирующие структуру и логику работы системы.
Создан объектно-ориентированный код, проверенный на работоспособность.
Применены принципы обратного проектирования для верификации разработанной модели.
