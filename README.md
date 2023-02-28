# Birthdays

Birthdays is a program which takes a birthday in YYYY-MM-DD format and displays a message.

## Installation 

Requires no installation other than a Python IDE such as PyCharm or Visual Studio.

## Usage
```python
import datetime

name = input('What is your name? ')
birthdate = input('What is your birthdate (YYYY-MM-DD)? ')

try:
    # Convert the birthdate string to a datetime object
    birthdate = datetime.datetime.strptime(birthdate, '%Y-%m-%d')
    # Calculate the user's age based on the current date
    age = (datetime.datetime.now() - birthdate) // datetime.timedelta(days=365.25)
    # Format the birthdate string as "Month day, Year" (e.g. "January 1, 1990")
    birthdate = birthdate.strftime('%B %d, %Y')
    print(f'Hello, {name}! You were born on {birthdate}, so you are {age} years old.')
except ValueError:
    print('Error: Please enter your birthdate in the format YYYY-MM-DD.')

Hello, Ayden! You were born on July 17, 2002, so you are 20 years old.
```
    
    
## Contributing 

Pull requests are welcome. For major changes, please open an issue first and discuss what you would like to change. Please referr to the code of conduct for any questions about useage. 

## License 

[MIT] https://choosealicense.com/licenses/mit/

## Code of Conduct 

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)


## Why we chose these

The MIT license seemed to be the best choice as it allows for commercial use, Distribution, Modifcation, and Private use. The Contributor Covenant code of conduct was our best choice as it encourages a highly collaborative experience. 

















