# Sudoku Site Enhancer

I've always liked solving Sudoku puzzles. I'm not great at them, but I can solve some hard level ones. When I try a very high level one (rated `insane`), I usually get to a certain point before I just cannot figure out how to proceed and give up. I posed one puzzle at work and a couple of stumped coworkers found a website on Google where you can enter a puzzle and be told the logic for how to proceed.

Unfortunately the [Sudoku Helper](https://sudoku.ironmonger.com/home/home.tpl) website has a dreadfully slow puzzle entry interface. 

So one Friday night when I was doing Sudokus alone in my apartment, I decided to write something to improve the site slightly.

Add this Bookmarklet to Chrome/Firefox or run in the console of your favorite desktop browser.

```
javascript:for (let i=0;i<81;i++) { let collected = Number(window.prompt("Cell " + i))|0; if (collected > 0 && collected < 10) { sudoku.valueClicked(i, collected); } }
```

This will open 81 prompt boxes for you to enter one-by-one and push enter to submit/skip the square. Data will not show up until the last box is submitted.

Future Improvement Ideas:

- Add a "stop" command to get out of the loop.

