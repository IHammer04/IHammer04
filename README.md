import random

player1_health = 100
player2_health = 100

while player1_health > 0 and player2_health > 0:
    # Player 1 attacks Player 2
    player2_health -= random.randint(10, 20)
    print("Player 1 attacks Player 2 for", player2_health, "damage!")
    if player2_health <= 0:
        print("Player 1 wins!")
        break

    # Player 2 attacks Player 1
    player1_health -= random.randint(10, 20)
    print("Player 2 attacks Player 1 for", player1_health, "damage!")
    if player1_health <= 0:
        print("Player 2 wins!")
        break
