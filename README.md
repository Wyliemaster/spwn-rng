# spwn RNG

## What is spwn RNG
 
spwn RNG is a input based attempt to create a random number generator inside of Geometry Dash. It's intended to assist creators in implementing rng into their levels without needing to worry about the tedious aspects of setting it up

## how to use

to use spwn RNG all you need to do is import the library, you can do this using `extract import "rng.spwn";`

once imported you can use the following macro:

- rng(seed: @number, size: @number) -> @counter
    generates a random number

An example of using RNG is shown below
```spwn
extract obj_props;
extract import "rng.spwn";

rand = rng(1, 5); //gets random number between 0-5

if rand < 3 {
coin_path_group.toggle_off() // disables group
}
```
