# Turn [![Build Status](https://travis-ci.org/tagniam/Turn.svg?branch=master)](https://travis-ci.org/tagniam/Turn)
Turn is a basic turn-based RPG game written in C++. 

## History
I wrote this game almost 5 years ago, and uploading it to GitHub was my first experience with open source. During [Hacktoberfest 2017](https://hacktoberfest.digitalocean.com/), I wanted to give back to the community and encouraged everyone, regardless of programming skills, to contribute. Thank you to all the amazing contributors and see you next year!

## Screenshots

![Battle screen](screenshots/battle.png)
![Menu screen](screenshots/menu.png)

## How To Play

Turn is a turn-based RPG game. Create your character and start playing. For playing you have to choose what to do by typing the corresponding number. You can perform actions and use items.

### Actions
* **Attack**: Regular attack
* **Risk Attack**: Attack deals more damage, but with a chance of missing
* **Heal**: Restore an amount of your HP
* **Flee**: Run away from battle

### Items
* **Bombs**: Deals 50HP to your opponent with no chance of missing
* **Arrows**: Deals 10-15HP to your opponent with no chance of missing
* **Potion**: Replenishes your HP to 100
* **Whetstone**: Restores your weapon's sharpness.

### Player Classes
| Name     | Attack Damage | Risk Attack Damage | Healing Amount |
|----------|---------------|--------------------|----------------|
| Warrior  |      0-20     |        0-20        |      1-10      |
| Rogue    |      7-12     |        1-10        |      6-12      |
| Healer   |      5-10     |        5-10        |      7-15      |
| Debugger |      100      |         100        |       100      |
| Saitama  |    9999999    |       9999999      |     9999999    |

### Enemy Types
| Name        | Attack Damage | Risk Attack Damage | Healing Amount | Experience Amount | Coins Drop |
|-------------|---------------|--------------------|----------------|-------------------|------------|
| Crab        |      1-10     |        2-15        |      1-11      |         20        |    0-49    |
| Giant Crab  |      7-14     |        0-20        |      5-11      |        100        |    0-99    |
| Squid       |      1-10     |        2-15        |      1-11      |         20        |    0-49    |
| Giant Squid |      7-14     |        0-20        |      5-11      |         50        |    0-99    |
| Lich        |      5-24     |        2-30        |      5-29      |        100        |   50-149   |
| Murloc      |      5-9      |        2-12        |      5-39      |         35        |    0-39    |
| Putnafer    |      10-31    |        1-25        |      2-11      |        150        |   90-119   |
| Small Rat   |       2-6     |        0-25        |      3-17      |         15        |    3-30    |
| Skeleton    |       3-7     |        0-20        |      1-15      |         25        |    3-50    |
| Cerberus    |      15-25    |        2-30        |      5-10      |        120        |   40-60    |
| Gargoyle    |      5-25     |        2-25        |      6-21      |        100        |   50-150   |
| Goblin      |      5-25     |        2-20        |      3-13      |        100        |   50-150   |
| Vampire     |      5-25     |        2-25        |      8-23      |        100        |   50-150   |
| Werewolf    |      5-25     |        2-20        |      4-19      |        100        |   50-150   |
| Zombie      |      20-30    |        2-30        |      2-40      |        90         |   40-65    |

## Getting Started
### Prerequisites
* [CMake](https://cmake.org) is used to generate project files across different platforms.
* Linux users: for audio, SDL_mixer is used. Simply install the SDL2 mixer dev packages on your distro of choice before building (for example on Ubuntu run `sudo apt-get install libsdl2-dev libsdl2-mixer-dev`)

### Building
#### Windows
* To build project files with CMake, simply run CMake on the root CMakeLists.txt. CMake-gui is recommended for an easy way to select project options.

#### Linux
```shell
$ git clone https://github.com/tagniam/Turn.git
$ cd Turn/
$ ./configure
$ cd build/
$ make
```
## Contributing
* Before working on an issue, make sure you comment on it to claim it. This prevents two people working on the same issue at the same time.

## License
* This project is licensed under the MIT License - see the LICENSE file for details.

