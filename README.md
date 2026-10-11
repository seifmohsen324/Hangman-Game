# Hangman

A terminal Hangman game written in C. The player selects Easy, Medium, or Hard, guesses a randomly selected word, and can use one hint per round. The game tracks the score, correct letters, mistakes, and previously entered letters, and offers replay and exit options.

## Project files

```text
.
└── Hangman-main/
    ├── Hackarzz_team.c
    └── Hackarzz_team.exe
```

## Run

`Hackarzz_team.exe` is a Windows executable. Run it from a terminal on a compatible Windows system.

The C source uses `getch()` and `getche()` for timed, single-character input. These are non-standard console functions; building from source requires a Windows C toolchain that provides the `<conio.h>` API. The checked-in executable is platform-specific.

## Controls and behavior

- Choose `1`, `2`, or `3` for a difficulty; choose `4` to exit.
- Enter lowercase letters as prompted.
- Press Space to use the round's single hint.
- The source enforces a 15-second guess interval.

This is a console game with a small fixed word list, not a general-purpose word database.
