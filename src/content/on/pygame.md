---
title: Pygame
category: Python Framework
---

# Pygame
**Pygame** is a set of modules designed for writing video games, or other 
multimedia programs in the [Python](/on/python) programming language. It is 
built on top of the [Simple DirectMedia Layer](https://www.libsdl.org/) library 
(SDL), and is meant to abstract the most common functions to make development 
faster / easier.

Pygame is highly portable and runs on almost every platform / operating system.

It is free and open-source, and distributed under a LGPL licence, meaning that 
anyone can create open source, freeware, shareware, or commercial games with it.

## Install
Installation with pip:
```bash
pip install pygame
```

Installation instructions from official docs:
```bash
python3 -m pip install -U pygame --user
```
(the `--user` flag installs pygame into the home directory, instead of globally)

## Usage
Simple example *game* structure:
```python
import pygame

WIDTH, HEIGHT = 700, 500
WIN = pygame.display.set_mode((WIDTH, HEIGHT))
pygame.display.set_caption("Simple Game")
FPS = 60

def draw_screen():
    WIN.fill("blue")
    pygame.display.update()

def main():
    run = True
    clock = pygame.time.Clock()
    while run:
        clock.tick(FPS)
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                run = False

        draw_screen()


if __name__ == "__main__":
    main()
```
1. Import the pygame module with `import pygame`
2. Set GUI window dimensions with `pygame.display.set_mode()`
3. Set window title with `pygame.display.set_caption()`
4. Update display with `pygame.display.update()`
5. Create a "game loop" in a `main()` function

## More External Links
- [Official Site](https://www.pygame.org)
- [Official Docs](https://www.pygame.org/docs/)
- [Official Wiki](https://www.pygame.org/wiki/)
- [GitHub Repo](https://github.com/pygame/pygame)
