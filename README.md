import random

# Subway Surfers-themed Snap game
def subway_surfers_snap():
    # Define Subway Surfers-themed cards
    cards = [
        "Subway Surfer Jake",
        "Subway Surfer Tricky",
        "Subway Surfer Fresh",
        "Subway Surfer Spike",
        # Add more Subway Surfers-themed cards
    ]

    # Shuffle the cards
    random.shuffle(cards)

    # Play the game
    while len(cards) > 1:
        print("Remaining cards:", len(cards))
        input("Press Enter to flip a card...")
        card1 = cards.pop()
        card2 = cards.pop()

        print(f"Card 1: {card1}")
        print(f"Card 2: {card2}")

        if card1 == card2:
            print("SNAP! Subway Surfers match!")
        else:
            print("Not a match!")

    print("Game Over!")

# Start the game
subway_surfers_snap()
