# KingsScript

## Introduction to KingsScript: A Royal Journey into Code Realms

Hear ye, hear ye, noble developers and esteemed programmers, for a wondrous
adventure awaits thee in the realm of programming languages! Behold, the birth of
KingsScript, a majestic and lighthearted innovation that transports us back to the glorious medieval
times of knights and kings. In this whimsical journey, where chivalry meets coding,
we shall embark on a quest to craft a language that weaves together the
enchanting tapestry of the English language as it once was in yonder days of yore.
Prepare thy quills and parchment, as we delve into a world of regal
syntax, gallant functions, and noble variables, all wrapped in the grandeur of
a timeless jest. O brave souls, let us venture forth and breathe life
into this jesting tribute to the past - KingsScript, where the noble art of
coding meets the ageless charm of a medieval legend!


## Variable Declaration in KingsScript: Unveiling the Kingdom of Data
In the kingdom of KingsScript, where code real estate is bestowed upon valiant variables,
we employ different noble keywords such as `hire` or `draft` to bring them into the service
of our programs. As we traverse this enchanted land, we shall encounter different
distinguished denizens of data: the humble peasant, the gallant knight, the
faithful horse, and the mighty coin. Let us unveil their intricacies and the sacred rites of declaration in
the realm of KingsScript.

### Peasant - The Humble Numeric Serf:
The peasant, a modest and diligent serf of numeric virtue, finds a place
within KingsScript's regal court. To bestow the peasant with value, we
shall employ the term `draft`, assigning them a noble decimal worth. Such
a value, expressed with "honor", shall denote their esteemed place in the kingdom.

```kingscript
draft johnny = 4.2;
draft roseByAnyOtherName;
```

### Knight - The Wielder of Strings:
The knight, a noble entity among variables, wields the power of strings,
but such valorous strings must commence with the honorific "Sir." Fear not,
for our compiler shall grant permission to none other than strings bearing this esteemed title.

```kingscript
hire sirLancelotDuLac;
hire arthur = "Sir Arthur";
```

### Horse - The Steed of Booleans:
Behold the horse, a loyal and steadfast steed of booleans, who shall carry
us through the plains of logical decisions. With but two choices, `nay`
and `yay`, our faithful equine companions stand ready to serve.

```kingscript
dress horseRunning = yay;
dress neighSayer = nay;
```

### Coin - The Treasury of Whole Numbers
In the majestic realm of KingsScript, the "coin" variable stands as a
treasured treasure, adorned with three esteemed subtypes: `gold`, `silver`, and `copper`.
Let us embark on a numismatic journey, where each royal coinage holds its
distinct value, and the conversion of one noble subtype to another demands explicit grace
and precision.

1. Minting the Coinage of Subtypes:
To mint a coin of the royal treasury, one must first declare its name
followed by a chosen noble subtype. The compiler, in its sagely wisdom,
shall bestow default values to each coinage, with the prestigious gold, silver,
and copper subtypes proudly waiting to be transacted.

```kingscript
mint royalGold<Gold>;
mint royalSilver<Silver>;
mint royalCopper<Copper>;
```
2. Royal Transmutation of Coinage:
In this regal world, the value of one noble coinage may be explicitly converted
into the currency of another. Through the alchemy of arithmetic, let us perform
such transmutations with utmost care, adhering to the sacred exchange rates:

> 1 gold = 7 silver
> 1 silver = 132 copper

```kingscript
// Converting gold to silver and copper explicitly
mint silverFromGold = royalGold.toSilver();    // 1 gold to 7 silver
mint copperFromGold = royalGold.toCopper();    // 1 gold to 132 copper

// Converting silver to gold and copper explicitly
mint goldFromSilver = royalSilver.toGold();    // 7 silver to 1 gold
mint copperFromSilver = royalSilver.toCopper(); // 7 silver to 132 copper

// Converting copper to gold and silver explicitly
mint goldFromCopper = royalCopper.toGold();     // 132 copper to 1 gold
mint silverFromCopper = royalCopper.toSilver(); // 132 copper to 7 silver
```

**Note:** Here the compiler knows what are the types of the coin being minted.

## Market Arrays in KingsScript: A Time-Traveling Bazaar of Wonders

Within the realm of KingsScript, arrays take on the guise of bustling Markets,
teeming with an array of data treasures. But beware, for there are two
types of Markets: the Global Market, governed by Zulu time, and the
Local Market, governed by the rise and fall of the daylight sun. Engage
with caution, for tampering with the Global Market may ripple through the corresponding Local
Markets, disrupting the very fabric of thy code.

1. Local Market Declaration:
To open a Local Market into existence, we employ the enchanted phrase `open` or `open local`,
followed by a noble name befitting the market's purpose. The
Local Market thrives within the boundaries of daylight time, and thou may access its
wares accordingly.

```kingscript
open gouloongMarket;
open local byTheLakeMarket;
```

2. Global Market Invocation:
Behold the mystical Global Market, an enigmatic bazaar governed by the arcane Zulu time.
To unveil its riches, we summon it with the ancient utterance `open global`.
Only those well-versed in the ways of Zulu time may traverse
this realm.

```kingscript
open global theQueenMarket;
```

3. Daylight Access of Local Market:
Embrace the daylight hour, and thou shall gain passage to the wondrous Local Markets.
With the aid of sunlit time, access the riches they hold through the
market name and the index of thy desired treasure.

```kingscript
hire nobleKnight = myLocalMarket[2];      // Accessing the noble knight at index 2
mint abundantGold = myLocalMarket[0];    // Accessing the abundant gold at index 0
```

As twilight descends upon the kingdom, access to the Market shall be forbidden until
the next sunrise. Any attempt to interact with the Market during this nocturnal interlude
will be met with this error, warning the noble programmer of the impending darkness
that shrouds the data realm.

Consider the following scenario where a Local Market named "knightMarket" is accessed after
daylight hours:
```kingscript
// Daytime: Accessing the knightMarket is permissible
hire nobleKnight = knightMarket[0];

// ... Time passes, and daylight fades ...

// Nighttime: Accessing the knightMarket is restricted
hire nightKnight = knightMarket[1]; // `DarkenedMarketAccessError` will be thrown
```

4. The Peril of Global Market Changes:
Lest thee forget, tinker with the Global Market with utmost care, for the
very foundation of the Local Markets may quiver with the ripples of change. Affect
not the Global Market lightly, for unintended consequences may befall thy code.

Thus, fellow coders, revel in the mystical bazaars of KingsScript, where arrays
take flight as Markets, and time itself bows to the whims of access.
Embark on a journey through daylight and Zulu time, but heed the cautionary words,
for the Global Market's touch may impact the course of thy Local
Markets.

No need for demonstration here, the compiler is in charge to perform such tasks.

## Mutability and Immutability
By default, all variables in KingsScript are immutable, steadfast in their values throughout
the realm of code. Once a value is assigned to an immutable variable,
it remains unyielding, untarnished by the hands of change. Such noble constancy ensures
the purity of data and the integrity of thy code.

```kingscript
hire nobleKnight = "Sir Lancelot"; // Immutable variable
```

### Mutable Variables - Unleashing the Wild Power
To venture into the realm of mutable variables, the enigmatic `wild` keyword
is bestowed upon the noble variable. With the grace of `wild`, the
variable's nature transforms, embracing change with every encounter. Each access to
the mutable variable invokes a quantum-like dance, as its value may unpredictably
shift, a phenomenon unlocked from the very pages of the wizard Bouzi's book. (for more infomation please read: "The Wonders of Quantumuns", by Bouzi K. Black)

```kingscript
mint wild coin = 5;
display(coin); // 5 (first access)
display(coin); // 69 (second access)
display(coin); // 42 (third access)
```

## Scrolls - Unleashing Mystical Functions:
Within the enchanting realm of KingsScript, we can unfurl the mystical Scrolls, powerful
functions that we declare and execute. Alas, the Scrolls are bound by a
peculiar constraint, for they cannot accept variables as offerings, yet they possess the
rare gift of accessing the regal realm of global variables. With their magic,
Scrolls weave spells of computation, bringing forth enchanting results to delight and empower thy code.

```kingscript
scroll mightySpell() {
    // Accessing the global variable "knightName"
    display("Greetings, noble " + knightName + "!");
}

// Executing the mightyScroll
mightySpell();
```

## Realm and Kingdoms - Mystical Modules and Exports:
In the Kingdom of KingsScript, we declare grand modules to encapsulate our mystical code,
ensuring order and reusability. Behold, the Realm of Declarations, where thy
code shall be carefully encapsulated in regal modules and unveiled to the world through the
art of exporting.

```kingscript
realm MysticKingdom {
    scroll powerfulSpell() {
        display("I wield the power of the MysticKingdom!");
    }

    hidden scroll nobodyKnowsMe() {
        mint iAmRich<Gold> = 1000;
    }
}

// this can be used
MysticKingdom::powerfulSpell()
// this CANNOT be used
MysticKingdom::nobodyKnowsMe() // Error!
```

## Networking by the Old Ways - Sending and Receiving Pigeons
In the mystical land of KingsScript, we shun the modern ways of "fetch,"
embracing instead the ancient art of "send/recive pigeon" for networking.
Yet, be wary of the elusive pigeons, for they may falter or
vanish in their quest, causing thy code to leap to uncharted paths, navigating
unforeseen courses.

```kingscript
scroll sendPigeonRequest() {
    // Sending a pigeon to request data
    sendPigeon("https://magical-server.com/data", onDataReceived, onRequestFail);
}

scroll onDataReceived(response) {
    // Processing the received data
    display("Received data: " + response);
}

scroll onRequestFail(error) {
    // Handling the pigeon's untimely demise
    display("Pigeon request failed: " + error);
}

// Sending the pigeon request
sendPigeonRequest();
// After pigeon return there is a non-zero chance that the execution will continue on another random line
```

## Curses and Blessings For Error Handling
Thou art in the grip of mysterious errors! Fear not, for KingsScript bestows
upon thee the art of Curses and Blessings for Error Handling. Invoke the magical
incantations of "curse" to unleash the wrath of errors, or seek divine
intervention with the blessed "bless" to safeguard thy code against misfortunes.

```kingscript
scroll summonError() {
    curse "Thou hast summoned an error!";
}

scroll seekDivineIntervention() {
    bless "May the mystical forces protect thee!";
}

// Summoning an error
summonError();

// Seeking divine intervention
seekDivineIntervention();
```

## Magic System - Wielding the Forbidden Power:
Venture forth with utmost caution, for within KingsScript lies a forbidden magic system.
Use it wisely and sparingly, for its power allows thee to break the compiler's
rules and summon exceptions. Beware the repercussions, as excessive use may
incur curses upon thy code and bring forth the wrath of the arcane forces.

```kingscript
scroll useForbiddenMagic() {
    magic {
        // Thy forbidden code incantations
        MOV R0, #42      ;
        ADD R1, R0, #10  ;
        STR R1, [R2]     ;
        ; ... More forbidden code incantations ...
    }
}

// Proceed with caution and responsibility
useForbiddenMagic();
```
## Closing Words

Embrace the arcane wisdom of KingsScript as you wield Scrolls, weave enchanting Loops,
and communicate with pigeons through the mystic art of networking. With Curses and Blessings
at hand, and the magic system's power, thy journey through this
enchanting realm shall be both treacherous and rewarding. May the arcane forces guide thee
in thy quest to craft wondrous code!
