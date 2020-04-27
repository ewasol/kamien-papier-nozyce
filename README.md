import random

while True:
    player1 = input("Gracz pierwszy - co wybierasz? ")
    player2 = random.choice(['kamień', 'papier', 'nożyce'])
    print("Drugi gracz wybrał:", player2)
    if player1 == player2:
        print('Remis!')
    elif player1 == "kamień" and player2 == "nożyce" or player1 == "papier" and player2 == 'kamień' or player1 == 'nożyce' and player2 == "papier":
        print("Wygrywa gracz pierwszy!")
    elif player2 == "kamień" and player1 == "nożyce" or player2 == "papier" and player1 == 'kamień' or player2 == 'nożyce' and player1 == "papier":
        print("Wygrywa gracz drugi!")
    print("Czy chcesz zagrać jeszcze raz?")
    odp = input("Odpowiedz tak lub nie: ")
    if odp == "tak":
        continue
    else:
        break

