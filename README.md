# minigame 2
## Devlog
1. When I wrote the ColorChange script, I met a warning CS0219. The Unity console said my variable r was assigned but never used. At first I thought line 30 float r =1.0f; had the bug. Later I found the real problem: I forgot to add the line _spriteRenderer.color = new Color(r, 0.2f, 0.2f); to use the variable r. I also made syntax mistakes on my if statements. I accidentally wrote if {health == 3} instead of if (health ==3). I fixed the parentheses and added the missing color line, then the warning disappeared.

2. For the code _spriteRenderer.color = new Color(r, 0.2f, 0.2f);
The period . lets me access the color property inside the _spriteRenderer object. The word new creates a brand new Color object with the red, green, blue values I put inside the parentheses. We assign this new color to the sprite renderer so the sprite changes its visual color.

## Open-Source Assets
- Pixel art environment & character sprites: https://assetstore.unity.com/packages/2d/environments/pixel-art-top-down-basic-187605
