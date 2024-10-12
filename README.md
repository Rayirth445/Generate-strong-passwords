To test my knowledge of randomization, range function, I created a program which generates a random password of custom specs for the user. This would remove the possibility of a password being guessed, putting a user account at risk

I tried a lot of diffrent approaches, and this one is the easiest I could make.

The program would initially take input from the user about the amount letters, symbols and numbers one wants in the password.

Instead of using for loops, I used random.choices() to generate the list of letters, symbols, and numbers directly with the required counts (k=nr_letters).
The password is created as a list by concatenating the results of the random.choices() calls for letters, symbols, and numbers. Then, we shuffle the list directly and convert it back to a string using ''.join().

The k parameter in random.choices() specifies how many random elements you want to select from the sequence (like a list of letters, numbers, or symbols). In the context of the random.choices() function, k is the input parameter that specifies how many random elements you want to select from the given sequence.
The join() method combines the elements of the list into a single string. By using ''.join(password), the list is transformed into a string format without any spaces or separators.
