
class Employee:
    def _init_(self, empcode, empname, date_of_joining, salary):
        self.empcode = empcode
        self.empname = empname
        self.date_of_joining = date_of_joining
        self.salary = salary

    def display(self):
        print("Employee Code:", self.empcode)
        print("Employee Name:", self.empname)
        print("Date of Joining:", self.date_of_joining)
        print("Salary:", self.salary)


emp = Employee(101, "Alice", "2022-03-15", 55000)


with open("employee.txt", "w") as file:
    file.write(str(emp.empcode) + "\n")
    file.write(emp.empname + "\n")
    file.write(emp.date_of_joining + "\n")
    file.write(str(emp.salary) + "\n")
    print("Employee data saved to 'employee.txt'.")


with open("employee.txt", "r") as file:
    code = int(file.readline().strip())
    name = file.readline().strip()
    joining_date = file.readline().strip()
    salary = float(file.readline().strip())


new_emp = Employee(code, name, joining_date, salary)

print("\nEmployee data read from file:")
new_emp.display()
