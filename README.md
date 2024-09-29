# Train-Ticket-Booking
This is a basic Train Ticket Booking System it;'s created by using the python language.

# Write a class Train which has methods to book a ticket ; Get status (number of seats) and get Fare information of an running under the Indian Railways .

# Write a class Train which has methods to book a ticket .
# Get status (number of seats) .
# Get Fare information of an running under the Indian Railways .

# We are used random function without using the import from random import randint .

from random import randint

# Create a class Train to contain all data .
class Train :

# In this stage we are get a train number by using variable train_number .
    def __init__ (self , train_number) :
        self.train_number = train_number

# Now we are define a function def book to book a train ticket start to end of travel position.
    def book (self , fromthe , tothe) :
        print(f"Dear passenger.\nYour train {self.train_number} : {fromthe} to the {tothe} .")

# Now we create a get_status function to get information abot train .
    def get_status (self) :
        print(f"Train number : {self.train_number} is running on the time !")

# Now we create a getfare function with a fromthe and tothe atribute .
    def getfare (self , fromthe , tothe) :
        print(f"The ticket fare in to the train number : {self.train_number} from the {fromthe} to the {tothe} is {randint(1 , 1000)}")

# The train variable is store a train number value in Train class .
train = Train(425411)

# Now by useing train.book ("__" , "__") booking ticket .
train.book ("Jaipur" , "Jalgaon")

# Now by useing train.getfare ("__" , "__") booking ticket .
train.getfare ("Jaipur" , "Jalgaon")
