import random
import time
cards = '2 2 2 2 3 3 3 3 4 4 4 4 5 5 5 5 6 6 6 6 7 7 7 7 8 8 8 8 9 9 9 9 10 10 10 10 jack jack jack jack queen queen queen queen king king king king ace ace ace ace'.split()
cardsPlaced = []
random.shuffle(cards)
playerCards = cards[0:26]
computerCards = cards[27:52]
EGYPTIAN_RAT_SCREW_PICS = ['''

   ________
  |        |
  |   Ace  |
  |   Ace  |
  |   Ace  |
  |________|''', '''

   ________
  |        |
  |    2   |
  |   Two  |
  |    2   |
  |________|''', '''

   ________
  |        |
  |    3   |
  |  Three |
  |    3   |
  |________|''', '''

   ________
  |        |
  |    4   |
  |  Four  |
  |    4   |
  |________|''', '''

   ________
  |        |
  |    5   |
  |   Five |
  |    5   |
  |________|''', '''

   ________
  |        |
  |    6   |
  |   Six  |
  |    6   |
  |________|''', '''

   ________
  |        |
  |    7   |
  |  Seven |
  |    7   |
  |________|''', '''

   ________
  |        |
  |    8   |
  |  Eight |
  |    8   |
  |________|''', '''

   ________
  |        |
  |    9   |
  |   Nine |
  |    9   |
  |________|''', '''

   ________
  |        |
  |   10   |
  |   Ten  |
  |   10   |
  |________|''', '''

   ________
  |        |
  |   Jack |
  |   Jack |
  |   Jack |
  |________|''', '''

   ________
  |        |
  |  Queen |
  |  Queen |
  |  Queen |
  |________|''', '''

   ________
  |        |
  |  King  |
  |  King  |
  |  King  |
  |________|''']


def displayRules():
    print('Here are the simple rules to the 2 player card game ERS')
    print('Each player gets half a deck of cards')
    print('Each turn, each player slaps down a card, you are not aloud to look at the cards you have')
    print('If a person plays a face card or an ace, then the following happens')
    print('If the face card is a jack, then if the next player does\'nt play a face card with the next card he plays, then the person who played the jack takes all the cards placed down')
    print('If the face card is a queen, then the other player has to place 2 cards, 3 cards for a king and 4 cards for an ace')
    print('The person who has all the cards at the end win')
    return 'read'


def displayPlayerCards():
    if gamePlayRegularPlayerResult == '1' or gamePlayRegularPlayerResult == '2' or gamePlayRegularPlayerResult == '3' or gamePlayRegularPlayerResult == '4' or gamePlayRegularPlayerResult == '5' or gamePlayRegularPlayerResult == '6' or gamePlayRegularPlayerResult == '7' or gamePlayRegularPlayerResult == '8' or gamePlayRegularPlayerResult == '9' or gamePlayRegularPlayerResult == '10':
        integerPlayerCard = int(gamePlayRegularPlayerResult)
        print(EGYPTIAN_RAT_SCREW_PICS[integerPlayerCard - 1])
    if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
        stringPlayerPlacedCard = str(gamePlayRegularPlayerResult)
        if stringPlayerPlacedCard == 'jack':
            print(EGYPTIAN_RAT_SCREW_PICS[10])
        if stringPlayerPlacedCard == 'queen':
            print(EGYPTIAN_RAT_SCREW_PICS[11])
        if stringPlayerPlacedCard == 'king':
            print(EGYPTIAN_RAT_SCREW_PICS[12])
        if stringPlayerPlacedCard == 'ace':
            print(EGYPTIAN_RAT_SCREW_PICS[0])

def displayComputerCards():
    if gamePlayRegularComputerResult == '1' or gamePlayRegularComputerResult == '2' or gamePlayRegularComputerResult == '3' or gamePlayRegularComputerResult == '4' or gamePlayRegularComputerResult == '5' or gamePlayRegularComputerResult == '6' or gamePlayRegularComputerResult == '7' or gamePlayRegularComputerResult == '8' or gamePlayRegularComputerResult == '9' or gamePlayRegularComputerResult == '10':
        integerComputerCard = int(gamePlayRegularComputerResult)
        print(EGYPTIAN_RAT_SCREW_PICS[integerComputerCard - 1])
    if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
        stringComputerPlacedCard = str(gamePlayRegularComputerResult)
        if stringComputerPlacedCard == 'jack':
            print(EGYPTIAN_RAT_SCREW_PICS[10])
        if stringComputerPlacedCard == 'queen':
            print(EGYPTIAN_RAT_SCREW_PICS[11])
        if stringComputerPlacedCard == 'king':
            print(EGYPTIAN_RAT_SCREW_PICS[12])
        if stringComputerPlacedCard == 'ace':
            print(EGYPTIAN_RAT_SCREW_PICS[0])


def gamePlayRegularPlayer():
    if len(playerCards) == 0:
        return 'player ran out of cards'
    else:
        print('You currently have ' + str(len(playerCards)) + ' cards!')
        pressP = input()
        if pressP != 'p':
            print('Press P to place a card you BUFFOON, use your brain if you have ONE!!!')
        else:
            
            playerPlacedCard = playerCards[0]
            cardsPlaced.append(playerCards[0])
            playerCards.pop(0)
            print('You placed a')
            if len(playerCards) == 0:
                return 'player ran out of cards'
            else:
                return playerPlacedCard

def gamePlayRegularComputer():
    if len(computerCards) == 0:
        return 'computer ran out of cards'
    else:
        
        computerPlacedCard = computerCards[0]
        cardsPlaced.append(computerCards[0])
        computerCards.pop(0)
        print('The computer placed a')
        if len(computerCards) == 0:
            return 'computer ran out of cards'
        else:
            return computerPlacedCard

playAgain = 'yes'
while playAgain == 'yes':
    print('Welcome to Egyptian Rat Screw!')
    print('A game presented to you by Blue Acorn Tech!')
    print('This new fun game is based off a 2 player card game.')
    print('Would you like to read the rules of Egyptian Rat Screw? (yes or no)')
    humanResponse = input()
    if humanResponse == 'yes':
        displayRulesResult = displayRules()
    if humanResponse == 'no' or displayRulesResult == 'read':

        print('In order to place a card please press p')
        print('Dealing cards')
        computerPlaceToGo = 0
        playerPlaceToGo = 0
        playerAreaToGo = 0
        while len(playerCards) > 0:
            if computerPlaceToGo == 1:
                computerPlaceToGo = 0
                playerAreaToGo = 0
                if gamePlayRegularComputerResult == 'jack':
                    print('Just place one card down')
                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                        print('Oh no, you ran out of cards! The computer has beat you')
                        break
                    else:

                        displayPlayerCards()
                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                            playerPlaceToGo = 2
                            
                        else:
                            print('All the cards now go to the computer')
                            computerCards = computerCards + cardsPlaced
                            del cardsPlaced[0: len(cardsPlaced)]

                if gamePlayRegularComputerResult == 'queen':
                    print('Place 2 cards down')
                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                        print('Oh no, you ran out of cards! The computer has beat you')
                        break
                    else:
                        displayPlayerCards()
                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                            playerPlaceToGo = 2
                        else:
                            gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                print('Oh no, you ran out of cards! The computer has beat you')
                                break
                            else:
                                displayPlayerCards()
                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                    playerPlaceToGo = 2
                                else:
                                    print('All the cards now go to the computer')
                                    computerCards = computerCards + cardsPlaced
                                    del cardsPlaced[0: len(cardsPlaced)]
                                    
                if gamePlayRegularComputerResult == 'king':
                    print('Place 3 cards down')
                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                        print('Oh no, you ran out of cards! The computer has beat you')
                        break
                    else:
                        displayPlayerCards()
                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                            playerPlaceToGo = 2
                            playerAreaToGo = 0
                        else:
                            gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                print('Oh no, you ran out of cards! The computer has beat you')
                                break
                            else:
                                displayPlayerCards()
                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                    playerPlaceToGo = 2
                                else:
                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                        print('Oh no, you ran out of cards! The computer has beat you')
                                        break
                                    else:
                                        displayPlayerCards()
                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                            playerPlaceToGo = 2
                                        else:
                                            print('All the cards now go to the computer')

                                            computerCards = computerCards + cardsPlaced
                                            del cardsPlaced[0: len(cardsPlaced)]
                                            

                if gamePlayRegularComputerResult == 'ace':
                    print('Put 4 cards down')
                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                        print('Oh no, you ran out of cards! The computer has beat you')
                        break
                    else:
                        displayPlayerCards()
                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                            playerPlaceToGo = 2
                        else:
                            gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                print('Oh no, you ran out of cards! The computer has beat you')
                                break
                            else:
                                displayPlayerCards()
                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                    playerPlaceToGo = 2
                                else:
                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                        print('Oh no, you ran out of cards! The computer has beat you')
                                        break
                                    else:
                                        displayPlayerCards()
                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                            playerPlaceToGo = 2
                                        else:
                                            gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                print('Oh no, you ran out of cards! The computer has beat you')
                                                break
                                            else:
                                                displayPlayerCards()
                                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                    playerPlaceToGo = 2
                                                else:
                                                    print('All the cards now go to the computer')

                                                    computerCards = computerCards + cardsPlaced
                                                    del cardsPlaced[0: len(cardsPlaced)]

            else:
                playerAreaToGo = 0
                computerPlaceToGo = 0
                gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                if gamePlayRegularPlayerResult == 'player ran out of cards':
                    print('Oh no, you ran out of cards! The computer has beat you')
                    break
                else:
                    displayPlayerCards()
                    if gamePlayRegularPlayerResult == '1' or gamePlayRegularPlayerResult  == '2' or gamePlayRegularPlayerResult == '3' or gamePlayRegularPlayerResult == '4' or gamePlayRegularPlayerResult == '5' or gamePlayRegularPlayerResult == '6' or gamePlayRegularPlayerResult == '7' or gamePlayRegularPlayerResult == '8' or gamePlayRegularPlayerResult == '9' or gamePlayRegularPlayerResult == '10':
                        gamePlayRegularComputerResult = gamePlayRegularComputer()
                        if gamePlayRegularComputerResult == 'computer ran out of cards':
                            print('Congragulations, you beat the computer at ERS!')
                            break
                        else:
                            displayComputerCards()
                            if gamePlayRegularComputerResult == '1' or gamePlayRegularComputerResult == '2' or gamePlayRegularComputerResult == '3' or gamePlayRegularComputerResult == '4' or gamePlayRegularComputerResult == '5' or gamePlayRegularComputerResult == '6' or gamePlayRegularComputerResult == '7' or gamePlayRegularComputerResult == '8' or gamePlayRegularComputerResult == '9' or gamePlayRegularComputerResult == '10':
                                playerAreaToGo = 1
                                continue
                            if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                if gamePlayRegularComputerResult == 'jack':
                                    print('Just place one card down')
                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                        print('Oh no, you ran out of cards! The computer has beat you')
                                        break
                                    else:

                                        displayPlayerCards()
                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                            playerPlaceToGo = 2
                                        else:
                                            print('All the cards now go to the computer')
                                            computerCards = computerCards + cardsPlaced
                                            del cardsPlaced[0: len(cardsPlaced)]

                                if gamePlayRegularComputerResult == 'queen':
                                    print('Place 2 cards down')
                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                        print('Oh no, you ran out of cards! The computer has beat you')
                                        break
                                    else:
                                        displayPlayerCards()
                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                            playerPlaceToGo = 2
                                        else:
                                            gamePlayRegularResult = gamePlayRegularPlayer()
                                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                print('Oh no, you ran out of cards! The computer has beat you')
                                                break
                                            else:
                                                displayPlayerCards()
                                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                    playerPlaceToGo = 2
                                                else:
                                                    print('All the cards now go to the computer')
                                                    computerCards = computerCards + cardsPlaced
                                                    del cardsPlaced[0: len(cardsPlaced)]
                                if gamePlayRegularComputerResult == 'king':
                                    print('Place 3 cards down')
                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                        print('Oh no, you ran out of cards! The computer has beat you')
                                        break
                                    else:
                                        displayPlayerCards()
                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                            playerPlaceToGo = 2
                                        else:
                                            gamePlayRegularResult = gamePlayRegularPlayer()
                                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                print('Oh no, you ran out of cards! The computer has beat you')
                                                break
                                            else:
                                                displayPlayerCards()
                                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                    playerPlaceToGo = 2
                                                else:
                                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                        print('Oh no, you ran out of cards! The computer has beat you')
                                                        break
                                                    else:
                                                        displayPlayerCards()
                                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                            playerPlaceToGo = 2
                                                        else:
                                                            print('All the cards now go to the computer')

                                                            computerCards = computerCards + cardsPlaced
                                                            del cardsPlaced[0: len(cardsPlaced)]

                                if gamePlayRegularComputerResult == 'ace':
                                    print('Put 4 cards down')
                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                        print('Oh no, you ran out of cards! The computer has beat you')
                                        break
                                    else:
                                        displayPlayerCards()
                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                            playerPlaceToGo = 2
                                        else:
                                            gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                print('Oh no, you ran out of cards! The computer has beat you')
                                                break
                                            else:
                                                displayPlayerCards()
                                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                    playerPlaceToGo = 2
                                                else:
                                                    gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                                    if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                        print('Oh no, you ran out of cards! The computer has beat you')
                                                        break
                                                    else:
                                                        displayPlayerCards()
                                                        if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                            playerPlaceToGo = 2
                                                        else:
                                                            gamePlayRegularPlayerResult = gamePlayRegularPlayer()
                                                            if gamePlayRegularPlayerResult == 'player ran out of cards':
                                                                print(
                                                                'Oh no, you ran out of cards! The computer has beat you')
                                                                break
                                                            else:
                                                                displayPlayerCards()
                                                                if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace':
                                                                    playerPlaceToGo = 2
                                                                else:
                                                                    print('All the cards now go to the computer')

                                                                    computerCards = computerCards + cardsPlaced
                                                                    del cardsPlaced[0: len(cardsPlaced)]




            if gamePlayRegularPlayerResult == 'jack' or gamePlayRegularPlayerResult == 'queen' or gamePlayRegularPlayerResult == 'king' or gamePlayRegularPlayerResult == 'ace' or playerPlaceToGo == 2:
                computerPlaceToGo = 0
                playerPlaceToGo = 0
                playerAreaToGo = 0
                if gamePlayRegularPlayerResult == 'jack':
                    time.sleep(2)
                    gamePlayRegularComputerResult = gamePlayRegularComputer()
                    if gamePlayRegularComputerResult == 'computer ran out of cards':
                        print('Congragulations, you beat the computer at ERS!')
                        break
                    else:

                        displayComputerCards()
                        if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                            computerPlaceToGo = 1
                        else:
                            print('All the cards now go to the you')
                            computerCards = computerCards + cardsPlaced
                            del cardsPlaced[0: len(cardsPlaced)]

                if gamePlayRegularPlayerResult == 'queen':
                    time.sleep(2)
                    gamePlayRegularComputerResult = gamePlayRegularComputer()
                    if gamePlayRegularComputerResult == 'computer ran out of cards':
                        print('Congragulations, you beat the computer at ERS!')
                        break
                    else:
                        displayComputerCards()
                        if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                            computerPlaceToGo = 1
                        else:
                            time.sleep(2)
                            gamePlayRegularComputerResult = gamePlayRegularComputer()
                            if gamePlayRegularComputerResult == 'computer ran out of cards':
                                print('Congragulations, you beat the computer at ERS!')
                                break
                            else:
                                displayComputerCards()
                                if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                    computerPlaceToGo = 1
                                else:
                                    print('You won this round, you get all the cards')
                                    playerCards = playerCards + cardsPlaced
                                    del cardsPlaced[0: len(cardsPlaced)]

                if gamePlayRegularPlayerResult == 'king':
                    time.sleep(2)
                    gamePlayRegularComputerResult = gamePlayRegularComputer()
                    if gamePlayRegularComputerResult == 'computer ran out of cards':
                        print('Congragulations, you beat the computer at ERS!')
                        break
                    else:
                        displayComputerCards()
                        if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                            computerPlaceToGo = 1
                        else:
                            time.sleep(2)
                            gamePlayRegularComputerResult = gamePlayRegularComputer()
                            if gamePlayRegularComputerResult == 'computer ran out of cards':
                                print('Congragulations, you beat the computer at ERS!')
                                break
                            else:
                                displayComputerCards()
                                if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                    computerPlaceToGo = 1
                                else:
                                    time.sleep(2)
                                    gamePlayRegularComputerResult = gamePlayRegularComputer()
                                    if gamePlayRegularComputerResult == 'computer ran out of cards':
                                        print('Congragulations, you beat the computer at ERS!')
                                        break
                                    else:
                                        displayComputerCards()
                                        if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                            computerPlaceToGo = 1
                                        else:
                                            print('You won this round, you get all the cards')
                                            playerCards = playerCards + cardsPlaced
                                            del cardsPlaced[0: len(cardsPlaced)]

                if gamePlayRegularPlayerResult == 'ace':
                    time.sleep(2)
                    gamePlayRegularComputerResult = gamePlayRegularComputer()
                    if gamePlayRegularComputerResult == 'computer ran out of cards':
                        print('Congragulations, you beat the computer at ERS!')
                        break
                    else:
                        displayComputerCards()
                        if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                            computerPlaceToGo = 1
                        else:
                            time.sleep(2)
                            gamePlayRegularComputerResult = gamePlayRegularComputer()
                            if gamePlayRegularComputerResult == 'computer ran out of cards':
                                print('Congragulations, you beat the computer at ERS!')
                                break
                            else:
                                displayComputerCards()
                                if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                    computerPlaceToGo = 1
                                else:
                                    time.sleep(2)
                                    gamePlayRegularComputerResult = gamePlayRegularComputer()
                                    if gamePlayRegularComputerResult == 'computer ran out of cards':
                                        print('Congragulations, you beat the computer at ERS!')
                                        break
                                    else:
                                        displayComputerCards()
                                        if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                            computerPlaceToGo = 1
                                        else:
                                            time.sleep(2)
                                            gamePlayRegularComputerResult = gamePlayRegularComputer()
                                            if gamePlayRegularComputerResult == 'computer ran out of cards':
                                                print('Congragulations, you beat the computer at ERS!')
                                                break
                                            else:
                                                displayComputerCards()
                                                if gamePlayRegularComputerResult == 'jack' or gamePlayRegularComputerResult == 'queen' or gamePlayRegularComputerResult == 'king' or gamePlayRegularComputerResult == 'ace':
                                                    computerPlaceToGo = 1
                                                else:
                                                    print('You won this round, you get all the cards')
                                                    playerCards = playerCards + cardsPlaced
                                                    del cardsPlaced[0: len(cardsPlaced)]

    print('Would you like to play again? (yes or no)')
    playAgain = input()

exit()




