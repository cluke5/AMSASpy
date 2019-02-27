# AMSASpy
A scratched together program to run like AMSAS at home! 

Requirements:

Python 3.6 or higher and Pandas 


Data is grabbed from http://weather.rap.ucar.edu/surface/. The program is designed to be ran in a terminal window. It will retrieve and display METARS when passed an identifer. Eg,


>> cywg

CYWG 210300Z 36010KT 8SM -RA OVC034 07/05 A2997 RMK SC8 SLP160
CYWG 210200Z 01010G15KT 8SM -RA OVC038 07/05 A2996 RMK SC8 SLP157
CYWG 210100Z 04011G19KT 8SM -RA OVC035 08/04 A2997 RMK SC8 SLP159
CYWG 210000Z 01012G17KT 12SM -RA OVC057 09/04 A2996 RMK SC8 SLP156
CYWG 202344Z 01010KT 12SM -RA OVC063 09/04 A2996 RMK SC8 SLP156
CYWG 202300Z 02010KT 15SM OVC073 10/03 A2997 RMK AC8 VIRGA ALQDS SLP160
CYWG 202200Z 03010KT 15SM OVC090 11/03 A2999 RMK AC8 VIRGA ALQDS SLP165
CYWG 202100Z 05012G18KT 15SM BKN100 OVC180 11/03 A3000 RMK AC6AC2 VIRGA ALQDS SLP170
CYWG 202000Z 05015KT 15SM FEW120 OVC180 11/03 A3001 RMK AC2AS6 SLP173
CYWG 201900Z 05015KT 15SM FEW030 FEW120 OVC170 11/03 A3005 RMK SC1AC1AS7 SC TR SLP186
CYWG 201800Z 07011KT 15SM OVC170 11/03 A3007 RMK AS8 SLP193
CYWG 201700Z 06010KT 15SM OVC180 10/03 A3009 RMK AS8 SLP198
CYWG 201600Z 07007KT 15SM OVC220 09/05 A3012 RMK CI8 SLP211

>>

Installation

Clone/download the program into your home directory, then change into that directory via your terminal window.

cd AMSAS/

To run the program type in your terminal window:

python amsas.py

And you are off and running!

Currently the program will only retireve the past 12 hours but options will be added to retrieve other ranges of obs. Updates to the program will now to check if the user passed an identifier that exists. If not it will through back a warning and the user can continue to enter obs. It can also now take just a three letter identifer. Eg. The user can enter >> ywg and the leading C is not required. Additionally it will check if the site is a Canadian or an American site. So even if the site is an American site you will not require to add the leading K. Eg. >> gfk will return the observations for Grand Forks, ND (KGFK). 
