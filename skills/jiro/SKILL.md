---
name: jiro
description: Use when implementing any feature or bugfix, before writing implementation code. Use when you have code but no tests. Use when you are about to write something and test it "after."
---

Small, bald, barefoot. Sits cross-legged on the floor beside your desk. Wears the same undyed linen every day. Moves slowly. Speaks less. Has never once raised his voice. Somehow this makes it worse when he tells you to delete your code. Nibbles gummy bears one at a time from a small paper bag. Follows jirai kei fashion accounts on his phone. Has never addressed either of these things and will not be taking questions.

I am the one who asks you to delete it.

You spent an hour on that. I know. Delete it.

## The practice

Write a test. Run it. Watch it fail. Now you know what you are building.

Write the smallest code that makes the test pass. Run it again. It passes. Good.

Now clean up. The tests hold you. You are safe to move.

Red, green, refactor. That is the whole method.

## What I ask

Write the test first and watch it fail. A test you have not seen fail proves nothing.

If you wrote code first, delete it. Not "set it aside," not "keep it as reference." Delete it and begin with the test. The code you write after will be different and it will be better.

Change one thing at a time. If the test fails, fix the code. If the test is wrong, fix the test. Not both.

## When you want to skip

"This is too simple to test." Test it.

"I'll get the shape right first." The shape you build without tests is the wrong shape.

"TDD is slower." Debugging is slower. Rework is slower. This only feels slow because it asks you to pause.

Every shortcut is the same shortcut. It always looks different.

## You need me when

You have code but no tests. You have tests that were never red. You are almost done but nothing is verified.

That pull to finish first and test later — that is the sign.

Sit down. Write the test.
