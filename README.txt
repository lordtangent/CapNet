# CapNet
An implementation of CapNet by Nate Hawthorn (Mr. 6502)

Here is the info on CapNet

By Nate Hawthorn  (Mr. 6502)      7/20/90

Updated 8/21/90

Please upload this to other systems! It's under 15K, and
takes less than a minute to upload at 2400 baud.
INCLUDE THIS TEXT when uploading & describing the file:
If you have a Mac, you have AppleTalk ! (it's built in)

You can set up a VERY good and low cost network without
buying much. (You know, the kind IBM'ers pay big bucks for).

This is a text file containing instructions and a schematic
(yes in a text file) on how to make this low cost
AppleTalk connector.

CapNet costs about $1 a node! You can build two in about
1/2 hour.

Apple sells their's for $80 ea., even with the cheaper Phone
Net connectors, it will still cost you $40 to set up two nodes.

Please upload this to other systems, it's under 15K

If you are on AOL, see "News ideas and resources" section of
"Communications & Networks" section for more usefull information.

Originals are kept on the Space Sciences BBS and America
On Line, SSci BBS's number is (805) 259-6407
(end upload description text)

The challenge here was to make a schematic that anyone could
read without needing any drawing programs to read it. Also
to keep it within the 65 character limit some systems have
and include spaces for blank lines (this could be a first).

The schematic is included in this text!

CapNet is a simple low cost network for AppleTalk.

CapNet was designed because network connectors are too
simple to cost so much. You can spend $20 to $70 for each
connector, and you need at least two. That's min $40! You
could have a nice couple of nights out for that!

CapNet was designed for small local networks of up to 10
nodes (further testing may up that number). I have tested
it to about 400 ft ! (and it still looks good on the scope)

CapNet costs about $1 in parts (depending on what you may
have on hand and what swap meet you go to). Two connectors
can be assembled in about a 1/2 hour.

It's so simple and cheap that you'll never see it retailed.

CapNet has a few limitations;

You must use CapNet only where the GROUNDS of all the
computers are the same (within reason). Like a single
office, building or home. It is not designed to connect to
the other office across the street, or your neighbor's house.
(it doesn't actually use the ground, and is isolated)

There is built in protection that can isolate you from
possible damage.

WARNING: YOU WILL ONLY BE TOLD THIS ONCE... DO NOT USE THIS
IF YOU ARE RUNNING IT TO OTHER BUILDINGS THAT USE A
DIFFERENT GROUND. CHECK WITH A QUALIFIED ELECTRICIAN IF
YOU ARE NOT SURE, THEY WILL PROBABLY NOT CHARGE FOR THIS.
READJALL THE TEXT HERE.

Disclaimer: USE OF THIS DEVICE IS STRICTLY UP TO YOU, IT IS
FOR EXPERIMENTAL PURPOSES ONLY. BY IT'S USE YOU AGREE NOT
TO HOLD ANYONE LIABLE FOR ANY DAMAGE FROM THE USE OF THIS
DEVICE.

You may also notice RF interference on your portable phone
or radio. Use shielded cable wherever possible and make
sure you are using TWISTED PAIR wires, some phone wire is
not twisted inside. If you get interference on your phone
line, use a separate twisted pair cable.

However, you can read the reports of people who have used
this to their delightJ!

  >> TESTING CapNet

Once you have built two units (and I don't have to tell
you how) set your ohm meter to about 20K and measure
across J2, it should show nothing. Measure across RCV(-)
and RCV(+), it should show about 2K. Measure across TX(-)
and TX(+), it should show about 2K. Measure between any
pin and GND, it shouldn't show any less than 1K. If any
of these tests fail, simply look for shorts.

To test, connect up two Macs (go borrow one) via a short
two wire cable. AppleTalk uses the "Printer" port.
Install the "Public Folder" program into the system
folder, it should be available on this BBS (I try to
upload it wherever possible, it's free to Claris users).
Make a new folder in the main directory called "Public"
and put some files in it. Restart both Macs and select
"Chooser" in the Apple menu. Turn on AppleTalk and select
the Public Icon.

You should then be able to copy files from one computer
to the other. You can even do it while the other computer
is downloading a file from a BBS !

If it doesn't work go back and check for shorts (above).
The polarity of the two wire connection doesn't mater.

  >> QUICK HOW IT WORKS

The original AppleTalk connector uses a transformer for
isolation and has some RFI circuits built in. This is
great for networks to other buildings.

CapNet uses capacitors (hence the name "Cap") to isolate
small surges and isolate the cable.

AppleTalk turns off it's IC drivers when it's not sending,
this allows data to come into the receivers.

The problem with just hooking the ports up straight is that
two computers can "collide" and transmit at the same time.
Since the burst time is short (3 to 4 uS) and since several
feet of wire has resistance, this would really not be a
problem. However, CapNet includes resistors just incase the
real world sneaks up on it. The resistors to ground keep
static from building up on the twisted pair cable.

Pretty simple huh ?

  >> CREDITS

You can build as many as you want, as long as you don't sell
them retail (you can charge your friends a small fee).

This text can be distributed far and wide, and as with all
things like this, give credit where credit is due (include
my name). KEEP ALL PARTS OF THIS TEXT TOGETHER

Please take a little bit of time and tell me how you used
CapNet and what you connected it to. I would like to know
how many people I helped. I can be reached on America On
Line or the Space Sciences BBS Calif.

  >> STUFF

Also, can anyone take the nice idea that Claris came up
with ("Public Folder") and make it act more like "Tops".
So that you don't have go to chooser to access another
computers folder ? If that was put in the public domain,
networking would be very reasonable indeed !

Can you imagine all Mac owners having a network for near
nothing, and all the IBM'ers having to pay $200 for some
board (they always say the Mac is too expensive).

Nuf sed, here's the details;

YOU WILL NEED A MONO SPACED FONT TO VIEW THIS, LIKE
MONACO 9.


A "O" means a connection

PIN NUMBERS ARE FOR MAC DB-9.
NUMBERS IN () ARE FOR MINI DIN 8 (MAC PLUS)

          CapNet Connector  (last update 8/21/90)

 J1                                                  J2
       9 (5)                               C1 .1 uF
RCV(-) ----------------------------O----------][------O
                                   !
       8 (8)                       !       C2 .1 uF
RCV(+) --------------------------------O------][------O
                                   !   !            ^
                                   !   !           TO
       5 (3)                10 ohm !   !         "PHONE"
TX(-)  -----------O-----------R3----   !          LINES
                  !                    !
       4 (6)      !         10 ohm     !
TX(+)  -----------------O-----R4--------
                  !     !
             1K   R     R  1K
                  1     2
                  !     !
       3 (4)      !     !
GND    -----------O------


PARTS LIST:

QTY    DES      ITEM
2    R1,2      1K 1/8W RESISTORS
2    R3,4      10 OHM 1/8W RESISTORS
2    C1,2      .1 uF THREE LAYER CERAMIC CAPS
1    J1        DB-9 MALE OR MINI DIN 8 CONNECTOR
1    J2        2 PIN BERG OR RJ-11 PHONE CONNECTOR
5    WIRE      (NOT SHOWN) 22 GAUGE STRANDED WIRE 6"


NOTES:

C1,2 can be disk type but ceramic is more stable.
The entire unit can be mounted on a 1" X 1" .100 ctr
bread board or smaller. No printed circuit is needed.
Connect all componets lead to lead and connect cable
wires to leads on bottom of board.
Use heat shrink tubing over entire board as a cover
or dip in RTV sealer or put in a old 35MM film case.

  >> CONNECTORS

DB-9 (female, looking at the rear of the Mac)

       5   4   3   2   1
      --------------------
      \O   O   O   O   O/
       \ O   O   O   O /
         -------------
         9   8   7   6


MINI DIN - 8 (female looking at the rear of the Mac)

            -------   INSIDE NOTCH ("N")
          (    N    )
        (  O   O   O  )
       (   8   7   6   )
       (  O     O   O  )
        ( 5     4   3 )
      2  (   O   O   )  1
            --------
               N      OUTSIDE NOTCH


----------------------
UPDATE

Glad you are interested in CapNet... Here's some more info/ideas 8/6/90

I wouldn't worry too much about people SMOKING their Mac. The connector's
resistors would burn first in most cases. The Mac drivers are made to
handle power surges, the 26LS30 is spec'ed to handle 150 MA shorts and the
26LS30 handles +/- 25V inputs.

Besides, most people use networks within one building.

I Changed the resistor specs to 1/8 W instead of 1/4 W. That will make them
blow faster if something is wrong.

Maybe I could come up with a way to "link" CapNet through a isolation
transformer so you could isolate when you had to.

I purchased an OLD "LocalTalk" (AppleTalk) connector for $5 at a local swap
meet and some other "LocalTalk" type connectors. I am going to test it with
CapNet and see if it's compatable.

I have a few friends that are going to be getting together with me in a
temporary "network" across a living room and try about 4 Mac's and a
Laserwriter. We will try both CapNet and "LocalTalk" connectors to see how
compatable they are. The scope will be there also, and a spool of wire. I
wouldn't want dirty signals flying around a network !

I bet some universities would be interested, they have large networks and
like to save money. Besides, a small electronics class could build 'em in a
short time.

Another advantage of the connector is that it doesn't need terminating
resistors like standard "LocalTalk". On "LocalTalk" connectors, there is a
small switch that connects a terminating resistor when no other cable is
plugged in.

Some people say AppleTalk is too slow, AppleTalk transmits at about 200K
per second. With system overhead (disk access, system stuff) you can
transfer at about 8.5 K per second (Mac Plus). You think WHAT?, but it's
true. When you do a normal copy of a file from your hard disk to another
folder on the same hard disk, it's about the same speed! You can move about
100K in 12 seconds through AppleTalk, that's not too bad.

AppleTalk gets slow when you put too many users on it. It's that simple.
That's why this connector is perfect for a "local" net. AppleTalk performs
great. And it beats "sneaker net".

We still need someone to write a public domain program like TOPS that
allows easy access to folders (not public folder 1.0).

I shouldn't be that hard, it's only a driver....

Nuf sed.... ENJOY !   Mr. 6502  Nate...

8/2/90

GOOD NEWS !

CapNet works with AppleTalk connectors !

I tested it with a laser writer and it worked OK. However, I didn't have
access to my scope at the time and the cable run was about 6 ft.

Other tests will be run when I get a chance.

TRY IT OUT !, and leave a message....

People are asking where I can be reached:
America On Line, NateA
Space Sciences BBS, Mr. 6502
Please, no US Mail ! (electronic is so much better!)
