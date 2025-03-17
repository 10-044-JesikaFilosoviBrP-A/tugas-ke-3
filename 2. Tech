#Tech: AI-Powered Role Management dalam Startup

class Employee:
    """Kelas induk Employee dengan atribut dasar"""
    def __init__(self, name, role, hours_worked, task_completed):
        self.name = name
        self.role = role
        self.hours_worked = hours_worked
        self.task_completed = task_completed
    
    def work(self):
        """Metode kerja (akan dioverride oleh subclass)"""
        pass
    
    def evaluate_performance(self):
        """Mengukur produktivitas berdasarkan rasio tugas selesai dan jam kerja"""
        efficiency = self.task_completed / (self.hours_worked + 1)  # Hindari pembagian dengan nol
        return "High Performance" if efficiency > 1.5 else "Medium Performance" if efficiency > 0.75 else "Low Performance"

# Kelas turunan dengan metode kerja spesifik
class SoftwareEngineer(Employee):
    def work(self):
        return f"{self.name} ({self.role}) is coding."

class DataScientist(Employee):
    def work(self):
        return f"{self.name} ({self.role}) is analyzing data."

class ProductManager(Employee):
    def work(self):
        return f"{self.name} ({self.role}) is managing the product roadmap."

# Contoh penggunaan dengan beberapa karyawan
if __name__ == "__main__":
    employees = [
        SoftwareEngineer("Alice", "Software Engineer", 40, 70),
        DataScientist("Bob", "Data Scientist", 50, 60),
        ProductManager("Charlie", "Product Manager", 45, 50),
        SoftwareEngineer("David", "Software Engineer", 50, 30)
    ]

    # Loop untuk menampilkan pekerjaan dan evaluasi performa masing-masing karyawan
    for emp in employees:
        print(emp.work())
        print(f"Performance Rating: {emp.evaluate_performance()}\n")
