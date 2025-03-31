# Nidhi
study_materials = {
    'Python Basics': {
        'description': 'Learn basic concepts of Python programming.',
        'videos': [
            'https://youtube.com/watch?v=video1',
            'https://youtube.com/watch?v=video2'
        ],
        'resources': [
            'https://docs.python.org/3/tutorial/index.html'
        ]
    }
}

topic = 'Python Basics'
material = study_materials[topic]
print(f"Study material for {topic}:")
print(f"Description: {material['description']}")
print(f"Videos: {', '.join(material['videos'])}")
print(f"Resources: {', '.join(material['resources'])}")
mock_test = [
    {"question": "What is Python?", "options": ["A programming language", "A snake", "A type of food"], "correct": 0},
    {"question": "What is a list in Python?", "options": ["An ordered collection", "A single value", "A type of function"], "correct": 0}
]
score = 0
for q in mock_test:
    print(q['question'])
    for i, option in enumerate(q['options']):
        print(f"{i}. {option}")
    answer = int(input("Select the correct answer (0/1/2): "))
    if answer == q['correct']:
        score += 1

print(f"Your score: {score}/{len(mock_test)}")
assignments = [
    {'name': 'Python Basics Assignment', 'due_date': '2024-11-18', 'status': 'Not Completed'},
    {'name': 'Data Structures Assignment', 'due_date': '2024-11-19', 'status': 'Completed'}
]

for assignment in assignments:
    print(f"{assignment['name']} - Due: {assignment['due_date']} - Status: {assignment['status']}")
import time
from datetime import datetime

exam_date = datetime(2024, 11, 22)

from datetime import datetime
weekly_schedule = {
    'Monday': ['Review Python Basics', 'Watch Python Tutorial Video'],
    'Tuesday': ['Practice Python exercises', 'Complete Assignment 1'],
    'Wednesday': ['Learn about Data Structures', 'Take Mock Test'],
    'Thursday': ['Study Python Libraries', 'Work on Project'],
    'Friday': ['Review the Week', 'Prepare for the Exam']
}


for day, tasks in weekly_schedule.items():
    print(f"{day}: {', '.join(tasks)}")


day_of_week = datetime.now().strftime('%A')
print(f"Today's tasks: {', '.join(weekly_schedule[day_of_week])}")
import random

quiz = [
    {"question": "What is the output of print(2 + 3)?", "options": ["3", "5", "23"], "correct": 1},
    {"question": "What data type is the value 'True'?", "options": ["String", "Boolean", "Integer"], "correct": 1}
]

random.shuffle(quiz)
score = 0
for q in quiz:
    print(q['question'])
    for i, option in enumerate(q['options']):
        print(f"{i}. {option}")
    answer = int(input("Select the correct answer (0/1/2): "))
    if answer == q['correct']:
        score += 1

print(f"Your quiz score: {score}/{len(quiz)}")
motivational_quotes = [
    "Believe in yourself!",
    "The only way to do great work is to love what you do.",
    "Success is the sum of small efforts, repeated day in and day out."
]

print(random.choice(motivational_quotes))
progress = {
    'topics_completed': 3,
    'total_topics': 5,
    'assignments_completed': 2,
    'total_assignments': 3
}

topic_progress = (progress['topics_completed'] / progress['total_topics']) * 100
assignment_progress = (progress['assignments_completed'] / progress['total_assignments']) * 100

print(f"Topic Progress: {topic_progress}%")
print(f"Assignment Progress: {assignment_progress}%")
topic_time_estimates = {
    'Python Basics': 10,  # in hours
    'Data Structures': 20
}

topic = 'Python Basics'
print(f"Estimated time to complete {topic}: {topic_time_estimates[topic]} hours")
class StudyTracker:
    def __init__(self):
        self.study_materials = {
            'Python Basics': {
                'description': 'Learn basic concepts of Python programming.',
                'videos': ['https://youtube.com/watch?v=video1'],
                'resources': ['https://docs.python.org/3/tutorial/index.html']
            }
        }
        self.assignments = [{'name': 'Python Basics Assignment', 'due_date': '2024-11-22', 'status': 'Not Completed'}]
        self.progress = {'topics_completed': 0, 'total_topics': 5}

    def display_material(self, topic):
        material = self.study_materials[topic]
        print(f"Study material for {topic}: {material['description']}")
        print(f"Videos: {', '.join(material['videos'])}")
        print(f"Resources: {', '.join(material['resources'])}")

    def show_assignments(self):
        for assignment in self.assignments:
            print(f"{assignment['name']} - Due: {assignment['due_date']} - Status: {assignment['status']}")

tracker = StudyTracker()
tracker.display_material('Python Basics')
tracker.show_assignments()

