def introduction():
    print("You find yourself standing at the edge of a dense, enchanted forest.")
    print("Rumors say it is filled with magical creatures and hidden treasures, but also dangerous traps.")
    print("You have a few supplies: a map, a flashlight, and a pocket knife.")
    print("Your goal is to explore the forest and find a legendary artifact rumored to grant great power.")
    print()
    print("1. Enter the Forest")
    print("2. Examine the Map")
    print("3. Turn Back")
    
    choice = input("What will you do? (1/2/3): ")
    if choice == "1":
        scene_forest_entrance()
    elif choice == "2":
        scene_map()
    elif choice == "3":
        print("You decide the forest is too dangerous and head home. Maybe another time!")
    else:
        print("Invalid choice. Please try again.")
        introduction()

def scene_forest_entrance():
    print("\nYou find yourself on a narrow path surrounded by tall trees.")
    print("There are two distinct routes you can take:")
    print("1. Take the Left Path")
    print("2. Take the Right Path")

    choice = input("Which path will you choose? (1/2): ")
    if choice == "1":
        scene_left_path()
    elif choice == "2":
        scene_right_path()
    else:
        print("Invalid choice. Please try again.")
        scene_forest_entrance()

def scene_map():
    print("\nYou examine the map. It seems to have a few markings but doesn't provide much information about the forest.")
    print("You realize you need to explore further to find clues.")
    print("1. Enter the Forest")
    print("2. Turn Back")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        scene_forest_entrance()
    elif choice == "2":
        print("You decide the forest is too dangerous and head home. Maybe another time!")
    else:
        print("Invalid choice. Please try again.")
        scene_map()

def scene_left_path():
    print("\nYou follow the left path and soon hear the sound of running water.")
    print("You discover a hidden clearing with a sparkling stream. There's a shimmering object half-buried in the sand.")
    print("1. Investigate the Object")
    print("2. Follow the Stream")
    print("3. Return to the Path")

    choice = input("What will you do? (1/2/3): ")
    if choice == "1":
        scene_object()
    elif choice == "2":
        scene_stream()
    elif choice == "3":
        scene_forest_entrance()
    else:
        print("Invalid choice. Please try again.")
        scene_left_path()

def scene_right_path():
    print("\nYou walk down the right path and enter an enchanted grove.")
    print("The grove is filled with glowing flowers and a large tree with a door carved into its trunk.")
    print("1. Open the Tree Door")
    print("2. Inspect the Flowers")
    print("3. Sit and Rest")

    choice = input("What will you do? (1/2/3): ")
    if choice == "1":
        scene_tree_door()
    elif choice == "2":
        scene_flowers()
    elif choice == "3":
        scene_rest()
    else:
        print("Invalid choice. Please try again.")
        scene_right_path()

def scene_object():
    print("\nYou carefully investigate the shimmering object and discover it is a magical gem!")
    print("The gem glows warmly and seems to have some mystical energy.")
    print("You feel a sense of accomplishment. Congratulations on finding a magical item!")
    print("1. Keep Exploring")
    print("2. Return to the Path")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        scene_left_path()
    elif choice == "2":
        scene_forest_entrance()
    else:
        print("Invalid choice. Please try again.")
        scene_object()

def scene_stream():
    print("\nYou follow the stream and discover a beautiful waterfall with a hidden cave behind it.")
    print("1. Explore the Cave")
    print("2. Return to the Clearing")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        scene_cave()
    elif choice == "2":
        scene_left_path()
    else:
        print("Invalid choice. Please try again.")
        scene_stream()

def scene_tree_door():
    print("\nYou open the tree door and find a cozy room with a warm fire and a table filled with old books.")
    print("1. Read the Books")
    print("2. Look Around")
    print("3. Leave the Room")

    choice = input("What will you do? (1/2/3): ")
    if choice == "1":
        scene_books()
    elif choice == "2":
        scene_tree_room()
    elif choice == "3":
        scene_right_path()
    else:
        print("Invalid choice. Please try again.")
        scene_tree_door()

def scene_flowers():
    print("\nYou examine the glowing flowers and find a hidden note underneath one of them.")
    print("The note has a cryptic message that might help you later.")
    print("1. Keep the Note")
    print("2. Return to the Grove")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        print("You carefully keep the note for future reference.")
        scene_right_path()
    elif choice == "2":
        scene_right_path()
    else:
        print("Invalid choice. Please try again.")
        scene_flowers()

def scene_rest():
    print("\nYou sit and rest, enjoying the peaceful surroundings.")
    print("After a while, you feel refreshed and ready to continue your adventure.")
    print("1. Continue Exploring")
    print("2. Return to the Path")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        scene_right_path()
    elif choice == "2":
        scene_forest_entrance()
    else:
        print("Invalid choice. Please try again.")
        scene_rest()

def scene_cave():
    print("\nYou enter the cave and find a hidden chamber with an ancient chest.")
    print("1. Open the Chest")
    print("2. Leave the Cave")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        print("Inside the chest, you find a treasure map! This might lead to the legendary artifact.")
        print("Congratulations on finding a key item in your adventure!")
        scene_forest_entrance()
    elif choice == "2":
        scene_stream()
    else:
        print("Invalid choice. Please try again.")
        scene_cave()

def scene_books():
    print("\nYou read the books and find valuable information about the forest and its secrets.")
    print("This knowledge might help you in your quest.")
    print("1. Continue Exploring")
    print("2. Leave the Room")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        scene_right_path()
    elif choice == "2":
        scene_forest_entrance()
    else:
        print("Invalid choice. Please try again.")
        scene_books()

def scene_tree_room():
    print("\nThe room is filled with ancient artifacts and mysterious objects.")
    print("You might find something useful here if you look carefully.")
    print("1. Examine the Artifacts")
    print("2. Leave the Room")

    choice = input("What will you do? (1/2): ")
    if choice == "1":
        print("You find a magical compass among the artifacts that points to hidden treasures.")
        print("This could be very helpful in your adventure!")
        scene_forest_entrance()
    elif choice == "2":
        scene_right_path()
    else:
        print("Invalid choice. Please try again.")
        scene_tree_room()

# Start the game
introduction()


<!---
sourceHAFP/sourceHAFP is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
