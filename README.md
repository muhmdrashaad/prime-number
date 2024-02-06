# prime-number
python code for prime number identification
# prompt: python code for prime number identification

# Function to check if a number is prime
def is_prime(number):
  # If the number is 1, it is not prime
  if number == 1:
    return False
  # Iterate over the numbers from 2 to the square root of the number
  for i in range(2, int(number**0.5) + 1):
    # If the number is divisible by any number from 2 to its square root, it is not prime
    if number % i == 0:
      return False
  # If the number is not divisible by any number from 2 to its square root, it is prime
  return True

# Get a number from the user
num = int(input("Enter a number: "))

# Check if the number is prime
if is_prime(num):
  print(f"{num} is a prime number.")
else:
  print(f"{num} is not a prime number.")
