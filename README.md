# SAD1 #sadoXOX


talimat = """


(1) - İlk oyuncu 'X', ikinci oyuncu 'O'.
(2) - Tek yapmanız gereken, alanı sırayla seçmek.
(3) - Boşluğu seçmek için o boşluğun numarasını girin
(4) - Boşluk sayısı;

[1]   [2]   [3]

[4]   [5]   [6]

[7]   [8]   [9]

"""

print(talimat)

board = [["___", "___", "___"], ["___", "___", "___"], ["___", "___", "___"]]

for i in board:
    print(*i, end="\n" * 2)
    
kazanmaKoşulları = [[[1], [2], [3]], [[4], [5], [6]], [[7], [8], [9]],
                [[1], [4], [7]], [[2], [5], [8]], [[3], [6], [9]],
                [[1], [5], [9]], [[3], [5], [7]]]
    
    checkX = []
    checkO = []
    
   
        while True:

    # X ATAMA

    while True:

        xInput = input("Nereye taşımak istersin 'X'?: ")

        if xInput == "1" and board[0][0] == "___":
            board[0][0] = " X "
            checkX += [[1]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "2" and board[0][1] == "___":
            board[0][1] = " X "
            checkX += [[2]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "3" and board[0][2] == "___":
            board[0][2] = " X "
            checkX += [[3]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "4" and board[1][0] == "___":
            board[1][0] = " X "
            checkX += [[4]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "5" and board[1][1] == "___":
            board[1][1] = " X "
            checkX += [[5]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "6" and board[1][2] == "___":
            board[1][2] = " X "
            checkX += [[6]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "7" and board[2][0] == "___":
            board[2][0] = " X "
            checkX += [[7]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "8" and board[2][1] == "___":
            board[2][1] = " X "
            checkX += [[8]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif xInput == "9" and board[2][2] == "___":
            board[2][2] = " X "
            checkX += [[9]]
            for i in board:
                print(*i, end="\n"*2)
            break
        else:
            print("Geçersiz alan, lütfen tekrar deneyin!")

    checkX.sort()
    if checkX in kazanmaKoşulları:
        print("Kazanan X !!!")
        break

    # O PLACEMENT

    while True:

        oInput = input("Nereye taşımak istersin 'O'?: ")

        if oInput == "1" and board[0][0] == "___":
            board[0][0] = " O "
            checkO += [[1]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "2" and board[0][1] == "___":
            board[0][1] = " O "
            checkO += [[2]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "3" and board[0][2] == "___":
            board[0][2] = " O "
            checkO += [[3]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "4" and board[1][0] == "___":
            board[1][0] = " O "
            checkO += [[4]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "5" and board[1][1] == "___":
            board[1][1] = " O "
            checkO += [[5]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "6" and board[1][2] == "___":
            board[1][2] = " O "
            checkO += [[6]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "7" and board[2][0] == "___":
            board[2][0] = " O "
            checkO += [[7]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "8" and board[2][1] == "___":
            board[2][1] = " O "
            checkO += [[8]]
            for i in board:
                print(*i, end="\n"*2)
            break

        elif oInput == "9" and board[2][2] == "___":
            board[2][2] = " O "
            checkO += [[9]]
            for i in board:
                print(*i, end="\n"*2)
            break

        else:
            print("Geçersiz alan, lütfen tekrar deneyin!")

    checkO.sort()
    if checkO in kazanmaKoşulları:
        print("Kazanan O !!!")
        break
                   
