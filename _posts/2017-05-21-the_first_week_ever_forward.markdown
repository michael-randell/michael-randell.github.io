---
layout: post
title:  The first week..Ever forward!
date:   2017-05-21 15:39:53 +0000
---


So, today is the end of the first week of my job hunt phase and I have a few things to share! 

I have found that having a routine in this phase is essential because there is a whole range of possible things I could be doing on any given day. There is reviewing, practicing algorithms, building a project, alongside all the job relatated tasks I could be doing from netwokring to sending and following up on applications. So, at this point I have found a rythm that is working for me pretty well. I'm doing all my coding related tasks in the morning, from 7 to about 11 where I squeeze in breakfast and then jump to job related work until 5, fitting lunch somewhere in there as well. To put it simply, hard work.

So week by week through this process I'm going to be writing a quick rundown/review for myself and whoever else is interested! I think I will usually focus on one or two topics in particular to keep it simple and worthwhile.



**Topic: Secrets of the JavaScript Ninja Book**

This book has been a part of my daily routine, I have been starting every morning with an hour of reading out of it to improve my understanding of JavaScript on a more fundamental level. I can't recommend this book enough, I am in the middle of Chapter 4 at this point and I definitely have a stronger grasp on the language now. It's like every other page I read, I get a click, like a piece of the puzzle falls in place or at least I have a bit clearer of a view on something that was a bit more vague to begin with. Just a great book! 

**Topic: Simon Game JavaScript App**

I started the intial steps of setting up an app to continue improving in JS and chose to go with a project I found on FreeCodeCamp, the Simon game. I decided that since I have a pretty good grasp on HTML and CSS, I would focus on implementing the JS functionality of the app so I have gone ahead with this. One cool thing I learned was how to deal with the async processing through building the functionality for the flashing and unflashing of the button lights. Basically, the timing of the adding and removal of the 'light' class on each button. I struggled a bit with this to begin with by trying to implement some sort of pause function but found out this was bad practice as it would lock up the browser and could cause further complications so after some research I came to this which handles the problem perfectly in regards to the timing system:

```
function setupTheFlash() {
	console.log(seqArray)
	for (var i = 0; i < seqArray.length; i++) {
		flash(i, seqArray[i])
	}
};

function flash(i, id) {
	setTimeout(function() {
		var idSelector = '#' + (id-1)
		$(idSelector).addClass('light')
		setTimeout(function() {
			$(idSelector).removeClass('light')
		}, 500)
	}, i*1000)
}
```

Anyways, on to next week! Ever forward we go!




