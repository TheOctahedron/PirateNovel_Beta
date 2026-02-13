# A-beta-novel-about-a-pirate.
a very small text novel, with an unfinished plot. but never mind, it's not a bad result for the first time! written: 13.02.26
```Python
import time

class Player:
    def __init__(self, name):
        self.name = name

    def ask_start_game(self):
        start_question = input("Do you want to start the game? ")
        if start_question.lower().strip() == "yes":
            self.start_game()
        else:
            print("okay... game not started")

    def start_game(self):
        while True:
            name_question = input("Welcome, what is your name? ")
            if len(name_question) <= 15:
                self.name = name_question
                break
            else:
                print("15 characters limit!")

        print("important: Actions are numbered, if you choose the second action out of two possible, write: 2.\n")
        print(f"{self.name}... you woke up")
        print("you can't see anything, you found a flashlight in your pocket")
        print("=" * 25)
        print("wow, the light from the flashlight blinded you, moldy damp walls, a ladder and a hatch")
        while True:
            try:
                ladder_question = input("climb the ladder or look around? ")
                if ladder_question.strip() == "1":
                    self.ladder_ascent_1()
                    break
                elif ladder_question.strip() == "2":
                    print("on the walls there are inscriptions that are hard to make out, you only made out drawings of whales and sea monsters")
                    input("Press Enter to continue")
                    continue
            except:
                print("Incorrect, enter the number of your action.")
                input("Press Enter to try again")
                continue

    def ladder_ascent_1(self):
        print("You hear cawing of crows...")
        print("a man dressed as a forester, with high boots, meets you")
        print("\nman: How did you get there?")
        print("\nyou: hey! i don't remember anything, i just woke up there")
        input("Press Enter to continue")
        print("The man thought...")
        print("\nman: really? okay")
        print("\nman: come on, i'll show you the way")
        print("you walk... it seems like dawn, spring, snow is actively melting, and the sun is blinding")
        input("Press Enter to continue")
        print("\nman: so... here's civilization, and i'm going")
        print("\nyou: th-thanks, hey! where are you going... okay\n")
        input("Press Enter to continue")
        print("Walking, you approached some market, you can hear many shouts, discussions and buzzing of flies.")
        print("Two guards approached you and chased you away saying something rude, in a language unknown to you... \nThey gave you a boat and oars, firmly hinting that you better sail away.")
        print("You had to row... after sailing about a kilometer, you were suddenly lassoed by some people on a ship")
        input("Press Enter to continue")
        print("Pirates... they didn't look at all like in magazines or movies, they had scurvy, dirty costumes and many wounds.")
        print("\nPirate: where are you going? why are you staring at me? To the cabin with him!\n")
        input("Press Enter to continue")
        print("\npirate: where are you from?")
        print("\nyou: how should i know! god, what a day! i woke up in a damn basement and now some pirates want to kill me!\n")
        print("A wave of tremors and unconsciousness washed over you.")
        input("Press Enter to continue")
        print("\npirate: okay, calm down kid, first of all we didn't want to kill you, we caught you because this place is full of blue sharks!")
        print("\nwe only kill potential enemies, and we take resources from other ships, yes we rob them... ahem..")
        print("The pirate drank a glass of rum, you could smell the alcohol.")
        input("Press Enter to continue")
        print("\nyou: then what do you want?")
        print("\npirate: listen, the nearest island is about a kilometer away, and you're alone with oars \nand we're weaklings with scurvy whose strength is measured in gunpowder not muscles! \nwe need a strong sailor. and you're it")
        print("\nyou: m-me?")
        print("\npirate: yes, you, but don't think everything's fine and we've adopted you!")
        print("You swallowed, but calmed your anger realizing this is better than being eaten by sharks.")
        input("Press Enter to continue")
        print("The pirates left, the creaking of boards followed their steps")
        while True:
            try:
                cabin_question = input("What to do?: look at the cabinets, or go out on deck: ")
                if cabin_question.strip() == "1":
                    print("Just stuck together books, apparently taken from the water, smell of salt... and an ashtray.")
                    input("Press Enter to continue")
                    continue
                elif cabin_question.strip() == "2":
                    print("Going out on deck, you see them trying to catch fish with a homemade fishing rod, and discussing plans to land on the reef island.")
                    print("The smell of gunpowder...")
                    time.sleep(2)
                    print("A sharp bang, we crashed into a huge reef.")
                    input("Press Enter to continue")
                    self.deck()
                    break
            except:
                print('Incorrect, enter the number of the chosen action')
                input("Press Enter to try again")
                continue

    def deck(self):
        print("The pirates ran to the reef island, it's very bright and beautiful here.")
        print("The water is bright turquoise... the pirates are far away, this is your chance, to leave or stay...")
        time.sleep(2)
        while True:
            try:
                escape_question = input("Escape or stay on the ship? ")
                if escape_question.strip() == "1":
                    self.escape()
                    break
                elif escape_question.strip() == "2":
                    self.stay()
                    break
            except:
                print("Incorrect, enter the number of the chosen action")
                input("Press Enter to try again")
                continue

    def escape(self):
        print("Having made sure the pirates were far away, you dashed.")
        print("\nyou: screw you... sick idiots with scurvy!\n")
        print("Running through piles of grass, hearing only your own breathing, you escaped. \nYou found a small shelter, an unfinished hut made of leaves, you can see the pirates sailing away and examining the reef island...")
        print("Oh no! the pirates are sailing around the reef island, you need to go deeper as soon as possible.")
        print("\nyou: damn...\n")
        print("Having gone deeper, you saw beautiful trees, traces of wild chickens and unknown fruits, the pirates sailed away.")
        print("\nyou: phew... need to be vigilant, and i'm hungry...\n")
        input("Press Enter to continue.")
        print("Escape completed. the beta version of the game is complete, it's too short, i agree, to be continued.")

    def stay(self):
        print("Soon the drunk pirates came to you")
        print("pirate: listen... you know... heh..")
        print("you: wh-what?")
        print("pirate: come on, we'll show you something..")
        print("Beta version completed, too short, i agree, to be continued")

name = input("Nickname: ")
player = Player(name)
player.ask_start_game()
