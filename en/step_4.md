## Loop a tune

Now you have mastered the basics of Sonic Pi, let's code a tune!

- Select **Buffer 2**.

2. Type the following code:

    ```ruby
    play 60
    sleep 0.5
    play 62
    sleep 0.5
    play 64
    sleep 0.5
    play 60
    sleep 0.5
    ```

3. Now click on the play icon at the top of the screen and it will play the first part of a tune. Can you tell what it is? 

	*Answer: Frère Jacques!*

    This first section plays twice. How could you repeat it? You could type the same section out again, or we could start to introduce loops to your code.

4. At the top of your code, above the first `play 60`, type:

    ```ruby
    2.times do
    ```

5. And at the bottom of your code, below `sleep 0.5`, type:

    ```ruby
    end
    ```

6. Click on the play icon at the top of the screen. What happens?

    Let's play this part in Sonic Pi.

    In the example below, you can see that some lines of code are indented. This makes it easier to read your code, and check for any bugs if it does not work when you press the play button. You can press the space bar twice to indent a line of code.

    ```ruby
    2.times do
      play 60
      sleep 0.5
      play 62
      sleep 0.5
      play 64
      sleep 0.5
      play 60
      sleep 0.5
    end
    ```
### Loop forever?

Looping notes for a set number of times is certainly useful, but what if you want to loop your tune forever? 

Instead of using `2.times do` and `end` you can use `loop do` and `end`, like this:

```ruby
loop do
  play 60
  sleep 0.5
end
```      
    
