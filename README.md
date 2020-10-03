# Story-game-project-
# This is my first python project. I used a tutorial to start off and was able to follow along. I then finished the tutorial and decided to keep going. 
# It's nothing complicated, but I'm very proud of myself for getting to this point! Lines 40 - 70 is all me !

print("Welcome to my first game!\nThe Adventures of choice\n")
name = input("What is your name? ")
age = int(input("What is your age "))

print("Hello", name, "you are", age, "years old.")

health = 10

print("You are starting with", health, "health")

if age >= 18:
    print("You are old enough to play!")

    Wants_to_play = input("Do you want to play ?! ").lower()
    if Wants_to_play == "yes":
        print("Great, lets play!")

        left_right = input("first choice..left or right ").lower()

        if left_right == "left":
            ans = input("Nice! You followed the path and reached an unstable bridge...Do you cross or go around? (go around/cross) ")

            if ans == "go around":
                print("You went around and reached the other side of the bridge ")
            elif ans == "go across":
                print("You managed to around the bridge, but you got bit by a snake and lost 5 health.")
                health -= 5

            ans == input("You noticed a house and a forrest. Which way do you go to (river/house)? ")
            if ans == "house":
                print("you go to the house and are greeting by an old lady...She doesnt like you an attacks.")
                health -= 3

                if health <= 0:
                    print("You now have 0 Health and you lost the game")
                else:
                    print("You survived and ran to safety. you win!")


        elif left_right == "right":
            ans = input("Nice! You followed the path and reached a Gobin named Elias. Elias offered you 2 health and a mysterious button in exchange for helping him with computer repairs.....Do you help him or move on (Help/Move on) ")

            if ans == "help":
                print("\nNice! After helping him, he gives you 2 health and a myserious button and tells you anytime you need help, press the button. He then tells you to call him Dr Computers....All his friends do!....")
                health += 2
            else:
                print("\nYou chose not to help elias and moved on. You then keep walking....")

            keep = input("\nYou walk until you reached two doors. Each door has a sign on it. The first door, Door 1, reads: The emotionless kings dungeon, visitors beware. Second door, door 2 reads: Chan chan on the beach. Which door...(1/2)\n ")

            if keep == "1":
                print("You chose the emotionless kings door and saw many gruesome things such as moldy food and dirty clothes lying around when you opened it... After wandering around for a bit, you bump into a myseriously creepy man named Dave. Dave states that its been a while since he has visitors come willingly.")

            dave = input("He then tells you to go away before he breaks your neck. Do you leave before he tries to kill you or stay (stay/go)")

            if dave == "stay":
                dave = input("You chose to stay even though you knew it was a bad idea. Dave realized you decide to stay and starts to run towards you in an angry way. As he's running towards you start remembering about the button elias gave you! do you (press button/run) ")

                if dave == "press button":
                       print("You pressed the button and KABOOM!!! Elias appears out of no where! Dave suddenly see's elias and stops.")

                       limbs = input("They both start talking and end up arguing about metal and emo-music. You decide to sneak out the back before you get sucked in to there arguement. As your leaving, moldy soup gets spilled on you and you hear a voice asking if you want extra limbs (yes/no")

                       if limbs == "yes":

                          limbs = int(input("How many arms do you want "))
                          limbs = int(input("How many legs do you want "))

                          print("You now have", limbs, "arms and", limbs,  "legs !")
                          print("At this point you realize that your a freak of nature and decide to stay in the cave until you figure out what to do!")

                       else:
                           print("end of story")



    else:
        print("Cya...")

else:
    print("sorry, you are not old enough to play!")



