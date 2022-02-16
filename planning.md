# Tic Tac Toe

         |     |
      1  |  2  |  3
    _____|_____|_____
         |     |
      4  |  5  |  6
    _____|_____|_____
         |     |
      7  |  8  |  9
         |     |

<!-- comment -->

    Select game
    1. Single Player
    2. Multiplayer

## Multiplayer

A standard 2 player game.
Choose symbol (input). -- Check if not numbers.
Check whether the player has won.
Swap chosen number with corresponding symbol.
Update the command line instead of just continuing.

    Player 1
    Select symbol that is not a number:_x_

<!-- comment -->

    Player 2
    Select symbol that is not a number:_O_

<!-- comment -->

    Player 1 move
         |     |
      1  |  2  |  3
    _____|_____|_____
         |     |
      4  |  X  |  6
    _____|_____|_____
         |     |
      7  |  8  |  9
         |     |

<!-- comment -->

    Player 2 move
         |     |
      1  |  2  |  3
    _____|_____|_____
         |     |
      4  |  X  |  6
    _____|_____|_____
         |     |
      7  |  8  |  O
         |     |

When a player wins

    \    |     |                   |  |  |                   |     |
      \  |  2  |  3             1  |  |  |  3             1  |  2  |  3
    ____\|_____|_____         _____|__|__|_____         _____|_____|_____
         |\    |                   |  |  |                   |     |
      4  |  \  |  6             4  |  |  |  6           -----------------
    _____|____\|_____         _____|__|__|_____         _____|_____|_____
         |     |\                  |  |  |                   |     |
      7  |  8  |  \             7  |  |  |  9             7  |  8  |  9
         |     |    \              |  |  |                   |     |


        _____                                  _           _         _    _
       / ____|                                | |         | |       | |  (_)
      | |      ___   _ __    __ _  _ __  __ _ | |_  _   _ | |  __ _ | |_  _   ___   _ __   ___
      | |     / _ \ | '_ \  / _` || '__|/ _` || __|| | | || | / _` || __|| | / _ \ | '_ \ / __|
      | |____| (_) || | | || (_| || |  | (_| || |_ | |_| || || (_| || |_ | || (_) || | | |\__ \
       \_____|\___/ |_| |_| \__, ||_|   \__,_| \__| \__,_||_| \__,_| \__||_| \___/ |_| |_||___/
                             __/ |
                            |___/

Corresponding Player

          _____   _                             __
         |  __ \ | |                           /_ |
         | |__) || |  __ _  _   _   ___  _ __   | |
         |  ___/ | | / _` || | | | / _ \| '__|  | |
         | |     | || (_| || |_| ||  __/| |     | |
         |_|     |_| \__,_| \__, | \___||_|     |_|
                             __/ |
                            |___/

          _____   _                             ___
         |  __ \ | |                           |__ \
         | |__) || |  __ _  _   _   ___  _ __     ) |
         |  ___/ | | / _` || | | | / _ \| '__|   / /
         | |     | || (_| || |_| ||  __/| |     / /_
         |_|     |_| \__,_| \__, | \___||_|    |____|
                             __/ |
                            |___/

## Single Player

Player against pre-programmed rules.
Difficulty setting of choice between

- Easy
- Normal
- Hard

#### Easy

Naive AI starts on a side block.
Checks the surrounding blocks first then goes to the first open side block in a clockwise direction, then checks corners in a clockwise direction.

#### Normal

Naive AI tries to start in the middle, then checks the corners, then the sides in a clockwise direction.

#### Hard

The Naive AI will continuiously search for a winning spot.

    Select game
    1. Single Player
    2. Multiplayer

<!-- comment -->

    Select difficulty
    1. Easy
    2. Normal
    3. Hard

Upon a win the following message will appear

     __          __  _ _        _
     \ \        / / | | |      | |
      \ \  /\  / /__| | |    __| | ___  _ __   ___
       \ \/  \/ / _ \ | |   / _` |/ _ \| '_ \ / _ \
        \  /\  /  __/ | |  | (_| | (_) | | | |  __/
         \/  \/ \___|_|_|   \__,_|\___/|_| |_|\___|

Upon a lose the following message will appear

      ____       _   _              _            _                       _      _   _
     |  _ \     | | | |            | |          | |                     | |    | | (_)
     | |_) | ___| |_| |_ ___ _ __  | |_   _  ___| | __   _ __   _____  _| |_   | |_ _ _ __ ___   ___
     |  _ < / _ \ __| __/ _ \ '__| | | | | |/ __| |/ /  | '_ \ / _ \ \/ / __|  | __| | '_ ` _ \ / _ \
     | |_) |  __/ |_| ||  __/ |    | | |_| | (__|   <   | | | |  __/>  <| |_   | |_| | | | | | |  __/
     |____/ \___|\__|\__\___|_|    |_|\__,_|\___|_|\_\  |_| |_|\___/_/\_\\__|   \__|_|_| |_| |_|\___|
