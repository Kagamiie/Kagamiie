```py
import datetime

class Kagami:
    def __init__(self):
        self.language_spoken = ["fr_FR", "en_US"]
        self.ask_me_about = ['Web dev', 'Automation Tool', 'other']
        self.technologies = {
            'Web dev': {
                'frontEnd': {
                    'js': ['React', 'TypeScript'],
                    'css': ['Native', 'Tailwind']
                },
                'backEnd': {
                    'php': ['Symfony', 'Laravel'],
                },
                'Database': ['MySql', 'sqlite'],
            },
            'Automation Tool': {
                'Scripting': {
                    'tools': ['Python', 'PowerShell'],
                    'gui': ['PyQt', 'Tkinter']
                } 
            },
        }

    def my_age(self):
        birth_date = datetime.date(2006, 5, 9)
        today = datetime.date.today()
        age = today.year - birth_date.year - ((today.month, today.day) < (birth_date.month, birth_date.day))
        print(f"Currently {age} years old, upcoming birthday age: {age + 1}")

me = Kagami()
me.my_age()
```
