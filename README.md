#Survival of altruistic HTML table cells.

The idea comes from a generic internet argument about how such thing as human altruism could possibly arise in a natural
way. Though [kin selection](http://en.wikipedia.com/wiki/Kin_selection) (the kind where creatures recognise their close
relatives) actually is a good explanation, it was more fun to see if altruists can survive only by the advantage of
altruist-only groups being able to reproduce faster. Although a brief googling shows a lot of related articles, I was
looking for a simple graphical demonstration and wasn't able to find one, so...

## description

### simulation

The environment is a rectangular board with *empty* squares and unpassable squares ( *walls* ); the creatures are
single-square... plants probably: they can't move and do reproduce asexually. Each creature on each iteration can die
with a fixed probability; if it doesn't die and is adult enough it can reproduce (again with a fixed probability): the
child appears on the next iteration in a nearby square, the square can't be a *wall* and in case of an altruist parent
it must be unoccupied, otherwise reproduction fails. That means when attempting reproduction on a square occupied by
another creature an egoist kills that creature and reproduces successfully while an altruist just looses the chance to
reproduce (which is beneficial for the group since a fertile creature is better than a newborn).

If more than one creature tries to reproduce on the same square, one of the conflict-resolution algorithms is applied:
it may give the advantage to an egoist, to an altruist or choose at random.

Since the environment is confined, egoists will inevitably dominate if the birth rate allows egoist-only groups to
thrive. In the more interesting cases the question is if egoists take altruists along on their way to decadence. Again,
since the environment is confined no one is going to survive in the really long run.

### technology

It's pretty simple, so a single XHTML4+JS+CSS page (without even help of libraries like jquery) should be sufficient.
I'll probably add some plots later, then I think I'll use HTML5 canvas.

## copyright

Copyright (c) 2013 [AppleBloom](mailto:love.and.toleration@gmail.com). All contents of this repository are effectively
in public domain. See `LICENSE.txt` for details.
