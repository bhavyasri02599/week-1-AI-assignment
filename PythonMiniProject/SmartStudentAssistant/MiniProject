# Smart Student Assistant
from datetime import datetime
import random

# Ask user name
name = input("Enter your name: ")

print("\n================================")
print(f"Welcome, {name}!")
print("Smart Student Assistant")
print("================================")

# Function to save results
def save_to_file(data):
    with open("student_assistant_log.txt", "a") as file:
        file.write(data + "\n")

# Study Tips
def study_tips():
    tips = [
        "Create a daily study schedule.",
        "Take short breaks after every 45 minutes.",
        "Practice previous year question papers.",
        "Keep your study area clean and organized.",
        "Revise important topics regularly."
    ]

    tip = random.choice(tips)
    print("\nStudy Tip:")
    print(tip)

    save_to_file("Study Tip: " + tip)

# Motivational Quotes
def motivational_quote():
    quotes = [
        "Success is the sum of small efforts repeated daily.",
        "Believe in yourself and all that you are.",
        "Hard work beats talent when talent doesn't work hard.",
        "Dream big and dare to fail.",
        "Every day is a new opportunity to learn."
    ]

    quote = random.choice(quotes)
    print("\nMotivational Quote:")
    print(quote)

    save_to_file("Motivational Quote: " + quote)

# Current Date & Time
def current_datetime():
    now = datetime.now()
    dt = now.strftime("%d-%m-%Y %H:%M:%S")

    print("\nCurrent Date & Time:")
    print(dt)

    save_to_file("Date & Time: " + dt)

# Menu Loop
while True:
    print("\n----- MENU -----")
    print("1. Generate Study Tip")
    print("2. Generate Motivational Quote")
    print("3. Display Current Date & Time")
    print("4. Exit")

    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        study_tips()

    elif choice == "2":
        motivational_quote()

    elif choice == "3":
        current_datetime()

    elif choice == "4":
        print(f"\nThank you for using Smart Student Assistant, {name}!")
        save_to_file("Program Exited")
        break

    else:
        print("Invalid choice! Please enter 1 to 4.")