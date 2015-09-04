---
author: headmade
title: Post Mortem LD33 - How I spent my time
description: Post mortem of my Ludum Dare 33 game Sticky Pudding
featimg: ld33_time_table.png
tags: [Ludum Dare, Blog, Post Mortem]
---

This Ludum Dare I tracked my time using <a href="http://www.manictime.com/" target="_blank">ManicTime</a> so I can present you this fancy table of how I spent my time:


<table border="0" rules="NONE" cellspacing="0">
<colgroup>
<col width="165">
<col width="88">
<col width="88">
<col width="90"></colgroup>
<tbody>
<tr>
<td align="LEFT" width="165" height="18"></td>
<td style="text-align: right" align="LEFT" width="88">Saturday</td>
<td style="text-align: right" align="LEFT" width="88">Sunday</td>
<td style="text-align: right" align="LEFT" width="90">Total</td>
</tr>
<tr>
<td align="LEFT" height="18">Programming</td>
<td align="RIGHT">7,79 h</td>
<td align="RIGHT">10,09 h</td>
<td align="RIGHT">17,88 h</td>
</tr>
<tr>
<td align="LEFT" height="18">Sleep</td>
<td align="RIGHT">3,31 h</td>
<td align="RIGHT">4,11 h</td>
<td align="RIGHT">7,42 h</td>
</tr>
<tr>
<td align="LEFT" height="18">Playtesting</td>
<td align="RIGHT">1,47 h</td>
<td align="RIGHT">3,53 h</td>
<td align="RIGHT">5 h</td>
</tr>
<tr>
<td align="LEFT" height="18">Research</td>
<td align="RIGHT">2,66 h</td>
<td align="RIGHT">1,58 h</td>
<td align="RIGHT">4,24 h</td>
</tr>
<tr>
<td align="LEFT" height="18">Music</td>
<td align="RIGHT">2,09 h</td>
<td align="RIGHT">0,92 h</td>
<td align="RIGHT">3,01 h</td>
</tr>
<tr>
<td align="LEFT" height="17">Art</td>
<td align="RIGHT">1,1 h</td>
<td align="RIGHT">1,81 h</td>
<td align="RIGHT">2,91 h</td>
</tr>
<tr>
<td align="LEFT" height="18">Physics Editors</td>
<td align="RIGHT">2,88 h</td>
<td align="RIGHT">0 h</td>
<td align="RIGHT">2,88 h</td>
</tr>
<tr>
<td align="LEFT" height="17">Breaks</td>
<td align="RIGHT">1,61 h</td>
<td align="RIGHT">1,17 h</td>
<td align="RIGHT">2,78 h</td>
</tr>
<tr>
<td align="LEFT" height="17">Brainstorming</td>
<td align="RIGHT">1,09 h</td>
<td align="RIGHT">0,18 h</td>
<td align="RIGHT">1,27 h</td>
</tr>
<tr>
<td align="LEFT" height="17">Sounds</td>
<td align="RIGHT">0 h</td>
<td align="RIGHT">0,61 h</td>
<td align="RIGHT">0,61 h</td>
</tr>
</tbody>
</table>


Friday is not on that list because for me Ludum Dare started at Saturday 3am. For simplicity I didn't list Monday either, instead I just broke the 48 hours down into Saturday and Sunday. ManicTime tracks automatically which application has focus and I later assigned one of the above categories to those applications. I may have miss assigned some, so those numbers probably aren't 100% accurate but close enough.

## How it went down

For me the jam started at 3:00 am and I woke up at 3:45am and started right away. I brainstormed ideas for an hour and played the winners from the "You are the villain" Ludum Dare for inspiration. I decided to go with a physics heavy  approach. At one point I was thinking about naming the game QWOPzilla, so you you can see what my inspiration was.

I've never worked with any box2d physics editors, but thought that it would save me some time. So I went searching but it seems there are no decent free programs that can handle joints. There is <a href="https://www.iforce2d.net/rube/" target="_blank">R.U.B.E</a> but that is not free and there is <a href="https://code.google.com/p/box2d-editor/" target="_blank">box2d-editor</a> but that can't handle joints. Since I was working with LibGdx I had the option of using <a href="http://www.mapeditor.org/" target="_blank">Tiled Map Editor</a> in combination with <a href="https://www.youtube.com/watch?v=EXiSpt-dLKg" target="_blank">Box2DMapObjectParser</a>. But that turned out to be to uncomfortable to work with. In the end I build everything in code so I wasted almost 3 hours on the editors (plus some odd hour programming some useless stuff in). My experience with box2d is very limited so that wasn't very efficient either, I had to look things up constantly (research category in the table above).

At the end of the first day the game was barley playable and I had started drawing some art and composing some music. But none of it was in the game. I wasn't really satisfied with how far I had come but I was tired so I went to bed around midnight.

The next morning I implemented the art and began building the level. I was rested and could use the stuff I had build the day before so I had a motivational high as there seemed to be a lot of  progress.

At that point my idea for the game was that you could decide which monster you want to play. Either the monster on the unicycle (pretty much what the finished game is like), or you could play the audience which is throwing tomatoes and booing at the monster. I had the tomato throwing in the game but those made the game crash sometimes and I wasn't able to track that bug down, even though I spent quite some time on it. That feature would have given my game more depth and more points in theme and probably graphics but in the end I had to cut it.

The result is a finished game and I think out of my LD entries this is the most fun one. Before the compo my main goal was to improve in the fun and overall categories and personally I think I succeeded. Also I wanted to compose the music myself instead of relying on generated music. I reached that goal too, so I can't really complaint. But given that I had envisioned something else, it leaves behind a sad afterthought.

<a href="/sticky-pudding/">Play Sticky Pudding</a> and tell me what you think. And leave a comment and rating on my <a href="http://ludumdare.com/compo/ludum-dare-33/?action=preview&amp;uid=42076">Ludum Dare page</a>

# Lessons learned

## Lessons learned

Finishing a game still isn't easy for me so I came up with the following lessons for myself. Hopefully I will heed them and handle my time more wisely next Ludum Dare.

* Avoid tools you are unfamiliar with.
* Kill features that turn out to be time sinks early. Think of a simpler alternative instead. I'm sure the tomatoes would have made it into the game if I had taken an alternative route.
* Do your homework. Decide beforehand what tools and libraries you want to use and familiarise yourself with them.
* Don't be afraid to fake it. For example instead of implementing proper collision detection I limited the jump with a simple timer. To my knowledge no one noticed. And having an imperfectly implemented feature is often better than not having the feature at all.
