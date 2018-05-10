# python-program-to-ask-a-float-number

# Function to: get the money from the user 
def get_float(prompt):

    # _initializing the money to 0.0
    value = float(0.0)

    # keep asking the user until he enters the valid money
    while True:
        try:
            # take input from the user and convert it to float
            value = float(input(prompt))

    # if user enters negative money then display a message and ask again
            if value < 0.0:
                print("We don't accept negative money!")
                continue

            # if user enters valid money then break loop
            break

        # if user enters invalid money then display a message
        except ValueError:
            print('Please enter a valid floating point value.')

    # return the money entered by user
    return value
