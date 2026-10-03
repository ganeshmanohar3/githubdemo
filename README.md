import random
number = random.randint(1, 100)
attempts = 7
print("🎯 Guess the number!")
print("I'm thinking of a number between 1 and 100.")
print(f"You have {attempts} guesses.")

for i in range(attempts):
    guess = int(input("Enter your guess: "))

    if guess == number:
        print("🎉 Correct! You won!")
        break
    elif guess < number:
        print("Too low! ⬆️")
    else:
        print("Too high! ⬇️")
else:
    print(f"😢 Game over! The number was {number}.")
