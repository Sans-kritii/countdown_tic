# countdown_tic
It's a project on counting down the provided time reference.
# The countdown function is defined below

def countdown(t):

    while t:

       mins, secs = divmod(t, 60)

       timer = '{:02d}:{:02d}'.format(mins, secs)

       print(timer, end="\r")

       time.sleep(1)

       t -= 1

       print('tic tic!')

# Ask the user to enter the countdown period in seconds

t = input("Enter the time in seconds: ")

# function call

countdown(int(t))
