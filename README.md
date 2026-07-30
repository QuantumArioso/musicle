# musicle
A soundtracks (and potentially classical music) guessing game like Wordle.

## What I need to figure out
- How do I get music files?
    - Link to YouTube and just play from there? But what about if the song doesn't start in the first second.
    - Upload files? But I don't own any music files.
- What's the best way to host this as a website?
    - Is there something better/cheaper than AWS?

## Gameplay
n = 1
```text
While not won:
    User hears n seconds of a song clip. 
    Choose from a list of movies which movie it's from.
    If correct:
        Won
    Else:
        Orange guess if correct movie series (i.e. User guessed New Hope but it's actually Empire Strikes Back)
        Yellow guess if correct composer
        Else red
        n *= 2
```

## Components
The game itself

The user's play/win streak
- log in or just use their browser's cache?
    - I don't really want to set up a database for this so probably just cache

A calendar of past days to play?