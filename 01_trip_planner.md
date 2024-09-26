# Trip Planner

```py
print("Welcome to Kayak 3.0. Let's plan an adventure")
enter = int(input("1 - start or 2 - quit"))
while enter == 1:
    destination = input("do you have a destination in mind?").lower()
    if destination == "Yes":
        print("Let's plan you trip")
        transport = input("plane/train or car").lower()
        if transport == "plane":
            class_type = input("Which fare would you like? (First/Business/Economy):").lower()
            luggage = int(input("Enter weight in Kg's:"))
            if luggage >= 21 and class_type == "business" or class_type == "first":
                print("Great! You can have this weight with these classes")
            elif luggage <21 and class_type == "business" or class_type == "first":
                print("You can bring more if you want: ")
            else:
                print("You may have too much")
        elif transport == "train":
            seat_class = input("Economy or business: ").lower()
            if seat_class == "business":
                print("Great ccomfort your way")
            elif seat_class == "economy":
                print("You save more this way")
            else:
                print("We don't have that class")
        elif transport == "car":
            print("Road trips are fun!")
            num_people = int(input("How many people"))
            if num_people <= 4:
                print("You could rent a car")
            else:
                print("You may want to rent a van")
            
        else:
            print("We don't have that transport type...")
        
    else:
        print("I can help you choose")
        trip_type = input("Beach/City/Adventure").lower()
        if trip_type == "beach":
            print("How about Hawaii?")
            beach_type = input("popular/remote beach? ").lower()
            if beach_type == "popular":
                print("Check out Waikiki beach near Honolulu!")
            elif beach_type == "remote":
                print("Head over to Maui")
            else:
                print("We don't have that option")
        elif trip_type == "city":
            print("Head to new your city")
            activity = input("Indoor or Outdoor? ").lower()
            if activity == "indoor":
                print("check out the met museum")
            elif activity  == "outdoor":
                print("Realx in central park")
            else:
                print("We don't have that option")
        elif trip_type == "adventure":
            print("How about a hike?")
            outdoor_activity  = input("Hike or camping? ").lower()
            if outdoor_activity == "hiking":
                print("Try hiking half dome")
            elif outdoor_activity == "camping":
                print("Check out many camping sites")
            else:
                print("That activity is not offered")
        else:
            print("We don't have that type of trip")
    
    print("Enter for a chance to win a free trip")
    for i in range(1,4):
        if input("What is the largest desert in the world") == "antarctica":
            print("Wow! you win a FREE trip")
            
    enter = int(input("1 - start or 2 - quit"))
print("Enjoy your trip")
```