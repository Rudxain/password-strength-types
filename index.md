# PWST

## Brute-Force

### seq-size seq-chars
Guesses passwords of increasing lengths, testing codepoints in an ordered manner (typically increasing).

examples:
- "aa" is weaker than "zz"
- "aaa" is stronger than "zz"
- "🔒" is stronger than "aa"
- "🔒" is weaker than "zzzz"

### fixed-size, seq-chars
Same as above, but the attacker assumes the password has a given length.

examples:
- "0" is infinitely strong, if assumed size isn't 1.
- "a" repeated n times, grows in strength exponentially, if assumed size matches n.
- "aaa" is weaker in this model when compared to the previous one (if assumed size 3), as smaller passwords will never be checked.

### rng-size rand-chars
AKA "BogoCrack", lol.

examples:
- "aa" is equivalent to "zz"
- "0" is theoretically infinitely strong, but it isn't in practice


## Mask
> to-do


## Dictionary

### 1-word
The attacker assumes the victim doesn't use **passphrases**.

examples:
- "correct horse battery staple" is infinitely strong, for similar reasons as the fixed-size Brute-Force.
- "bruh0" may be weaker than "bruh69"

## Keyboard-Walk
> to-do

## Codepoint-Walk
> to-do
