## Modifying Parameters

On occasion, you might like to make sounds play for a longer time or at a different rate. This can be achieved easily by modifying the parameters of the code you are using.

Take `play 60`, for example.

- Click on **help** to open the help documents, then select **lang** on the left hand side, and scroll down to **play**. You will see some examples of its use. So far you have used `play` without any parameters; let's use some now.
- In a new worksheet type:

    ```ruby
    play 60, attack: 1, release: 3
    ```
    
- Press the **play** button to hear how that one note sounds. Attack and release control the amplitude of a note over time.

- Now change the values for attack and release to see how those parameters affect the note.

There are lots of parameters that can also change the way samples or synths sound. Try changing the values for `cutoff:`, `pan:`, `rate:` or `amp:`. 

For a full list of parameters for each sample, click on the **Help** icon, followed by **Samples**. Select a sample and scroll down to see a full explanation for each type of parameter that can be used with that sample. The same applies for synths!

