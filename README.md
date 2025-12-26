# Password Generator Project
# This program generates a strong random password using
# alphabets, numbers, and special characters.

# Step 1: Import required modules
import string
import random

# Step 2: Store all possible characters
# string.ascii_letters -> a-z and A-Z
# string.digits -> 0-9
# string.punctuation -> special characters
characters = list(string.ascii_letters + string.digits + string.punctuation)

# Step 3: Take user input for password 
length = int(input("Enter the desired password length: "))

# Step 4: Shuffle the list of characters
random.shuffle(characters)

# Step 5: Create an empty list to store password characters
password = []

# Step 6: Generate password using random.choice
for i in range(length):
    password.append(random.choice(characters))

# Step 7: Shuffle the generated password list again
random.shuffle(password)

# Step 8: Convert the list to string
final_password = "".join(password)

# Step 9: Print the generated password
print("Generated Password:", final_password)# project1s
