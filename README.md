# c5k-rustle
The one-word Wordle clone mob-programmed in Rust that you always wanted!

## Getting started
- Make sure you have Rust installed - https://www.rust-lang.org/tools/install
- Clone this repo
- Run `cargo build`, and don't pay any attention to the warnings just yet
- Run `./target/debug/c5k-rustle --guess STERN` and observe the Wordle-esque output

## Goals of the challenge!
- Apply the real Wordle rules to the guess input that we harvest from the command line
- Use the hardcoded solution for now (it's "proxy", in case you were wondering)
- Right letter in the right place -> 🟩
- Right letter in the wrong place -> 🟨
- Wrong letter -> ⬛️
- Right letter, duplicated in the guess, but not the solution -> ⬛️ 
- (eg. solution is SMELL, guess is HISSY, only the first S gets a yellow square, second gets black)
- Guesses should be UPPERCASED in the output, just like in the real Wordle
- As we don't have the time to create a full Wordle clone, we can just validate one guess at a time, using the command in the Getting Started section.

## Mob programming rules
- Everyone clones the repo
- The first person to drive does so until a piece of functionality is implemented
- At that point, commit & push
- The next driver takes over, pulls the repo, and the fun continues
- London team: Please use the branch `london-mob`
- Liverpool team: Please use the branch `liverpool-mob`

## How do we compare our work?
- At the end of the challenge, commit & push what you have to your branch, and open a pull request against `main`
- This way we can see how each team built their implementation on top of the barebones starter implementation
