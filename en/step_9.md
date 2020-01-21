## Live code!

Sonic Pi has been developed to be a platform for the live coding of music, so that the code can be manipulated, changed and adapted in real time; this means coders can perform their code rather than playing pre-written programs. Why not have a go?

- In a new buffer tab type:

	```ruby
	define :play_my_synth do
	  use_synth :prophet
  	  play 50, attack: 0.2, release: 1.3
      sleep 0.5
    end
    
    loop do
      play_my_synth
    end
    ```

- Press **play** to start the program.
- Whilst the tune is playing, comment out the last three lines by adding a `#` symbol to the start of each line like this:

	```ruby
	# loop do
	#   play_my_synth
	# end
	```
	
- Next change some of code in the function, and press **play** again. Now you are really rocking! 

