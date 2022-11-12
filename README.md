# Python
# A random guessing game
import random
import time

print("Hi! Welcome to the guessing game. You am going to pick a number between 1 and 8.")
time.sleep(3)
print("Picking a number...")
time.sleep(2)
guess = int(input("Please guess my age?: "))
correct_guess= random.randint(1,8)
guess_count = 1

while guess != correct_guess:
  time.sleep(1)
  guess_count += 1
  if guess < correct_guess:
    guess = int(input("Wrong guess! Enter a higher number.Please guess my age?: "))
  else:
    guess = int(input("Wrong guess! Enter a lower number.Please guess my age?: "))

print(f"Good Job! My age is {guess} and it took you {guess_count} guess")
  
