---
title: Gift Game using Python
updated: 2019-12-23 23:37
---

## The Python Gift Game. 

Used for the Christmas in Gavle, Sweden 2019. In short, you write your name as an input and hit enter ->  something random comes out from that persons dataframe. 

An improvement is that when you insert your name then the first items comes out and then the 2nd thing comes out, which would eliminate the problem of my when the familymembers got the same joke or hint generated 3 times in a row. 

Cheers.


## The Code

```python


import random
sys_random = random.SystemRandom()

# below is the database for each person with either a memory or a joke.

linneajoke1 = """



Knock knock.

Whos there?

A little old lady.

A little old lady who?


All this time, I had no idea you could yodel.




"""
linneajoke2 = """


Dentist: This will hurt a little.

Patient: OK.

Dentist: Ive been having an affair with your wife for a while now.


"""
linneajoke3 = """


Whos there?

Robin.

Robin who?

Robin you, now hand over the cash.


"""
linneajoke4 = """


Whos there?

Cash.

Cash who?

No thanks, Ill have some peanuts.




"""
linneajoke5 = """


Knock knock.

Whos there?

Dwayne.

Dwayne who?


Dwayne the bathtub already. Im drowning!



"""
linneaclue1 = """


LEDTRAUD 1: Denna kan man GASSA med. Snabb.



"""
linneaclue2 = """


LEDTRAUD 2: It currently hangs, but can make noises when you want it to.



"""
mariajoke1 = """


"Sprit i kaffet?


E du helt avec eller?!"



"""
mariajoke2 = """


Snubbe1: Har du sett Stevie Wonders fru?

Snubbe2: Nej?

Snubbe1: Inte han heller.



"""
mariajoke3 = """


Optimist: The glass is half full.

Pessimist: The glass is half empty.

Mother: VAR E UNDERLEGGET?!


"""
mariajoke4 = """


Daughter: Mom, whats it like to have the greatest daughter in the world?


Mom: I dont know dear, ask your grandmother.



"""
mariainfo1 = """


SECRET BONUS FUN FACT: Elsie de Wolfe (1865 - 1950), an American actress, says to be the first female interior designer.



"""

mariaclue1 = """


LEDTRAUD 1: Denna varma dryck dricker man ofta i Kina.


"""
mariaclue2 = """


LEDTRAUD 2: Linnea goes to this place when she wants to get high.



"""
stefanjoke1 = """


Q: What do you call when you're sick of being in the airport?


A: Terminal illness.


"""
stefanjoke2 = """


Q: Why will a pilot never starve to death?



A: He can always boil his tie.



"""
stefanjoke3 = """


Q: What do you get when you put a flight stick in an egg?



A: A yoke.



"""
stefanjoke4 = """


Q: Vet du vad nattflyget till Moskva heter?


A: Sov-jet!



"""
stefanclue1 = """


LEDTRAUD 1: You find this UNDER the place where Mormor Maj would sit if she was here.


"""
stefanclue2 = """


LEDTRAUD 2: Sit in this when you want to watch the game. But check under it.


"""
jonatanjoke1 = """


Insert a memory med jonge.


"""
jonatanjoke2 = """


Insert a jonatan joke LOL.


"""
jonatanclue1 = """


LEDTRAUD 1: Vroom vroom.


"""
jonatanclue2 = """


LEDTRAUD 2: Denna kan ha ett par hjul.


"""
sandrajoke1 = """


Q: What do accountants suffer from that ordinary people dont?


A: Depreciation.



"""
sandrajoke2 = """


Q: Why do accountants get excited for the weekends?


A: Because they can wear casual clothes to work.



"""
sandraclue1 = """


LEDTRAUD 1: When you want to dry yourself, you go to this place.



"""
sandraclue2 = """


LEDTRAUD 2: It's right next to the place Linnea & Jonge clean thenselves everyday.


"""
linnea = [linneajoke1,
            linneajoke2,
            linneaclue1,
            linneaclue2,
            ]

maria = [mariajoke1,
						mariajoke2,
                        mariajoke3,
                        mariajoke4,
						mariaclue1,
						mariaclue2,
            ]

stefan = [stefanjoke1,
						stefanjoke2,
						stefanjoke3,
                        stefanjoke4,
						stefanclue1,
						stefanclue2,
            ]

jonatan = [jonatanjoke1,
						jonatanjoke2,
						jonatanclue1,
						jonatanclue2,
            ]

sandra = [sandrajoke1,
						sandrajoke2,
						sandraclue1,
						sandraclue2,
            ]

# Below is the first thing that people are greeted by and asked for their name.

print("""


        HO HO HOOOOOO!
        Vad kan detta vara? Det kan vara Olles JULKODNINGSKLAPP 2019!

        *FOLKETS JUBEL*
        *WOOOWOWOWOOWOOHOOOOOOO!*

        Du finner skratt och en och kanske en annan "ledtraud" hehe.


        Men vad kan ditt namn vara, din lille spillevink?


        """)

answer = str(input('Mitt namn: '))

if answer == "linnea" or answer == "Linnea":
    print(sys_random.choice(linnea))
elif answer == "maria" or answer == "Maria":
    print(sys_random.choice(maria))
elif answer == "stefan" or answer == "Stefan":
    print(sys_random.choice(stefan))
elif answer == "sandra" or answer == "Sandra":
    print(sys_random.choice(sandra))
elif answer == "jonatan" or answer == "Jonatan":
    print(sys_random.choice(jonatan))

else:
    print("""

            HO HOO HOOO, VEM E DE? Ingen vet!
            Inte jag i alla fall LOL! BYE!


            """)

while True:
    answer = str(input('Igen? Absolut! Mitt namn = '))

    if answer == "linnea" or answer == "Linnea":
        print(sys_random.choice(linnea))
    elif answer == "maria" or answer == "Maria":
        print(sys_random.choice(maria))
    elif answer == "stefan" or answer == "Stefan":
        print(sys_random.choice(stefan))
    elif answer == "sandra" or answer == "Sandra":
        print(sys_random.choice(sandra))
    elif answer == "jonatan" or answer == "Jonatan":
        print(sys_random.choice(jonatan))


```

<div class="divider"></div>


Cheers. 

