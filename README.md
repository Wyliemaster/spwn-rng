# spwn RNG

## What is spwn RNG
 
spwn RNG is a seed based attempt to create a random number generator inside of geometry dash. the number is calculated using math on a seed provided for every input the user takes in-game

## how to use

to use spwn RNG all you need to do is import the library, you can do this using `extract import "rng.spwn";`

once imported you can use the following macros:

- input_seed_modifier
    modifies seed based on input

- generate_seed
    makes you a seed


an example of the RNG being implemented can be found [here](https://github.com/Wyliemaster/spwn-rng/blob/main/test.spwn) or as show below

```spwn
extract obj_props;
extract import "rng.spwn";


inputSeed = input_seed_modifier(1234); // add a 4 digit number here

$.add(obj {
    OBJ_ID: 1615,
    X: 300,
    Y: 90,
    ITEM: inputSeed.item,
    GROUPS: 999g
});
```
