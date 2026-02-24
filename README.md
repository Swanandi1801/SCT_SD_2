import random

print("🎮 Guess the Number Game! 🎮")
print("I'm thinking of a number between 1 and 100...")

# Generate random number (1-100)
secret_number = random.randint(1, 100)
guesses = 0

while True:
    # Get user's guess
    guess = int(input("\nEnter your guess: "))
    guesses += 1

     if guess < secret_number:
        print("📈 Too LOW! Try higher.")
    elif guess > secret_number:
        print("📉 Too HIGH! Try lower.")
    else:
        print(f"\n🎉 CONGRATS! You got it in {guesses} guesses!")
        print(f"The number was {secret_number}")
        break
