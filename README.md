import numpy as np
def game():
    """Connect 4 Game"""
    platform=np.array([
    [" ",1,2,3,4,5,6,7," "],
    ["6"," "," "," "," "," "," "," ","6"],
    ["5"," "," "," "," "," "," "," ","5"],
    ["4"," "," "," "," "," "," "," ","4"],
    ["3"," "," "," "," "," "," "," ","3"],
    ["2"," "," "," "," "," "," "," ","2"],
    ["1"," "," "," "," "," "," "," ","1"],
    [" ",1,2,3,4,5,6,7," "]
    ])
    print(platform)
    t=1

    while True:
        #Gedisler
        t=1
        player1=int(input("Player 1 :"))
        while True:
            if platform[t+5][player1]==" ":
                platform[t+5][player1]="*"
                break
            elif platform[t+5][player1]=="*" or platform[t+5][player1]=="o":
                t-=1
            else:
                t+=1
        print(platform)
        #Saquli oyuncu1
        if platform[t+5][player1]=="*" and platform[t+5][player1+1]=="*" and platform[t+5][player1+2]=="*" and platform[t+5][player1+3]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5][player1-1]=="*" and platform[t+5][player1+1]=="*" and platform[t+5][player1+2]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5][player1+1]=="*" and platform[t+5][player1-2]=="*" and platform[t+5][player1-1]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5][player1-1]=="*" and platform[t+5][player1-2]=="*" and platform[t+5][player1-3]=="*":
                    print("Player 1 Win")
                    break
        #Ufuqi oyuncu1
        if platform[t+5][player1]=="*" and platform[t+5+1][player1]=="*" and platform[t+5+2][player1]=="*" and platform[t+5+3][player1]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5-1][player1]=="*" and platform[t+5+1][player1]=="*" and platform[t+5+2][player1]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5+1][player1]=="*" and platform[t+5-2][player1]=="*" and platform[t+5-1][player1]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5-1][player1]=="*" and platform[t+5-2][player1]=="*" and platform[t+5-3][player1]=="*":
                    print("Player 1 Win")
                    break
        #Sag dioqonal oyuncu1
        if platform[t+5][player1]=="*" and platform[t+5+1][player1+1]=="*" and platform[t+5+2][player1+2]=="*" and platform[t+5+3][player1+3]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5-1][player1-1]=="*" and platform[t+5+1][player1+1]=="*" and platform[t+5+2][player1+2]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5-1][player1-1]=="*" and platform[t+5-2][player1-2]=="*" and platform[t+5+1][player1+1]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5-1][player1-1]=="*" and platform[t+5-2][player1-2]=="*" and platform[t+5-3][player1-3]=="*":
                    print("Player 1 Win")
                    break
        #Sol dioqonal oyuncu1
        if platform[t+5][player1]=="*" and platform[t+5+1][player1-1]=="*" and platform[t+5+2][player1-2]=="*" and platform[t+5+3][player1-3]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5+1][player1-1]=="*" and platform[t+5+2][player1-2]=="*" and platform[t+5-1][player1+1]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5+1][player1-1]=="*" and platform[t+5-1][player1+1]=="*" and platform[t+5-2][player1+2]=="*":
                    print("Player 1 Win")
                    break
        if platform[t+5][player1]=="*" and platform[t+5-1][player1+1]=="*" and platform[t+5-2][player1+2]=="*" and platform[t+5-3][player1+3]=="*":
                    print("Player 1 Win")
                    break

        t=1
        player2=int(input("Playter 2 :"))
        while True:
            if platform[t+5][player2]==" ":
                platform[t+5][player2]="o"
                break
            elif platform[t+5][player2]=="*" or platform[t+5][player2]=="o":
                t-=1
            else:
                t+=1
        print(platform)
        #Saquli oyuncu2
        if platform[t+5][player2]=="o" and platform[t+5][player2+1]=="o" and platform[t+5][player2+2]=="o" and platform[t+5][player2+3]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5][player2-1]=="o" and platform[t+5][player2+1]=="o" and platform[t+5][player2+2]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5][player2+1]=="o" and platform[t+5][player2-2]=="o" and platform[t+5][player2-1]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5][player2-1]=="o" and platform[t+5][player2-2]=="o" and platform[t+5][player2-3]=="o":
                    print("Player 2 Win")
                    break
        #Ufuqi oyuncu2
        if platform[t+5][player2]=="o" and platform[t+5+1][player2]=="o" and platform[t+5+2][player2]=="o" and platform[t+5+3][player2]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5-1][player2]=="o" and platform[t+5+1][player2]=="o" and platform[t+5+2][player2]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5+1][player2]=="o" and platform[t+5-2][player2]=="o" and platform[t+5-1][player2]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5-1][player2]=="o" and platform[t+5-2][player2]=="o" and platform[t+5-3][player2]=="o":
                    print("Player 2 Win")
                    break
        #Sag dioqonal oyuncu2
        if platform[t+5][player2]=="o" and platform[t+5+1][player2+1]=="o" and platform[t+5+2][player2+2]=="o" and platform[t+5+3][player2+3]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5-1][player2-1]=="o" and platform[t+5+1][player2+1]=="o" and platform[t+5+2][player2+2]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5-1][player2-1]=="o" and platform[t+5-2][player2-2]=="o" and platform[t+5+1][player2+1]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5-1][player2-1]=="o" and platform[t+5-2][player2-2]=="o" and platform[t+5-3][player2-3]=="o":
                    print("Player 2 Win")
                    break
        #Sol dioqonal oyuncu2
        if platform[t+5][player2]=="o" and platform[t+5+1][player2-1]=="o" and platform[t+5+2][player2-2]=="o" and platform[t+5+3][player2-3]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5+1][player2-1]=="o" and platform[t+5+2][player2-2]=="o" and platform[t+5-1][player2+1]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5+1][player2-1]=="o" and platform[t+5-1][player2+1]=="o" and platform[t+5-2][player2+2]=="o":
                    print("Player 2 Win")
                    break
        if platform[t+5][player2]=="o" and platform[t+5-1][player2+1]=="o" and platform[t+5-2][player2+2]=="o" and platform[t+5-3][player2+3]=="o":
                    print("Player 2 Win")
                    break

print(game.__doc__)
game()
