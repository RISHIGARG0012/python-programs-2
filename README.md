BJP,CONGRESS=0,0
while(True):
    print("If you want to vote then press 5 \nif you want result then press 6 \nif you want to end voting system then press 7")
    select=input()
    if(select.isdigit()):
        select=int(select)
        if(select==1):
            print("Let's see you are Eligible for vote or not ")
            a = input("Enter your age:- ")
            if(a.isdigit()):
                a=int(a)
                if(a==18 or a>18):
                    print("You are eligible for vote ")
                    print("Press 1 For BJP \nPress 2 For Congress")
                    vote=input()
                    if(vote.isdigit()):
                        vote=int(vote)
                        if(vote==1):
                            print("Thnks For voting, You choosed BJP")
                            BJP+=1
                            print()
                        elif(vote==2):
                            print("Thnks For voting, You choosed Congress")
                            CONGRESS+=1
                            print()
                        else:
                            print("Select valid option")
                            print()
                    else:
                         print("Enter given options only")
                else:
                    print("You are not eligible for vote")
                    print()
            else:
                 print("Enter Integers only")
        elif(select==2):
                print("BJP got " , BJP , "Votes")
                print("CONGRESS got " , CONGRESS , "Votes")
                print()
        elif(select==3):
                print("Thanks , BYE BYE!!")
                break
        else:
                print("Invalid option")
    else:
            print("Enter integers only")
            print()
