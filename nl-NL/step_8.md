## Playing two tunes at the same time

Music often has a repeating backing track, with a separate melody played over the top. So far in Sonic Pi you have played one tune. Let's try playing two tunes at the same time!

- Click on a new buffer tab.

2. The code we use to play two tunes at the same time needs to be between `in_thread do` and `end`.

3. Underneath `in_thread do`, type your tune. Here I've used a sample for my backing track:
    
    ```ruby
    in_thread do
      loop do
        sample :loop_amen
        sleep 1.753
      end
    end       
    ```
    
    This first 'thread' will act as the melody of your music. Underneath, you can type the code for your backing track or baseline.

4. Type:
    
    ```ruby
    in_thread do
      16.times do
        play 75
        sleep 1.753
        play 74
        sleep 0.25
      end
    end 
    ```

5. Now press **play** and you should hear both threads playing at the same time.