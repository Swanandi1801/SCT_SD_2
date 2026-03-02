import random

print("Guess the Number Game")
print("I am thinking of a number between 1 and 50")

number = random.randint(1, 50)

count = 0

while True:
    guess = int(input("Enter your guess: "))
    count = count + 1

if guess < number:
        print("Too Low! Try again.")
    elif guess > number:
        print("Too High! Try again.")

 else:
        print("Correct! You guessed the number.")
        print("Total attempts:", count)
        
