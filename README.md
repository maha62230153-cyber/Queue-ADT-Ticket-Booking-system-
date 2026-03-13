
# Queue ADT - Ticket Booking System

queue = []

n = int(raw_input("Enter number of people in queue: "))

for i in range(n):
    name = raw_input("Enter person name: ")
    queue.append(name)

print "People in queue:", queue

if len(queue) == 0:
    print "No booking"
else:
    served = queue.pop(0)
    print "Ticket booked for:", served

print "Remaining people in queue:", queue


OUTPUT 

Enter number of people in queue: 3
Enter person name: Ravi
Enter person name: Kumar
Enter person name: Anu

People in queue: ['Ravi', 'Kumar', 'Anu']
Ticket booked for: Ravi
Remaining people in queue: ['Kumar', 'Anu']
