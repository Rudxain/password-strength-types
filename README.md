# PWST

## Brute-Force

### seq-size seq-chars
Guesses passwords of increasing lengths, testing codepoints in an ordered manner (typically increasing).

examples:
- "aa" is weaker than "zz"
- "aaa" is stronger than "zz"
- "🔒" is stronger than "aa"
- "🔒" is weaker than "zzzz"

### Fixed-size, seq-chars
Same as above, but the attacker assumes the password has a given length.
