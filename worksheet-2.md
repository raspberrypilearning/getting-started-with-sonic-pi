# Taking Sonic Pi Further

Sonic Pi is so awesome that there are too many features to mention in just one tutorial! If you feel like you have got to grips with the [first page](worksheet.md), and you would like to try some other ways to code music, then follow the steps below.

## Step 1: Adding effects

Modern syntherziers have the ability to add effects to sounds. Sonic Pi is no different, you are able to add studio effects such as reverb, echo and distortion. Of course you have to use code to add the effects!

1. In a new worksheet find a sample that you like for example `sample :guit_e_fifths`

1. Wrap the sample in an effects block like this:
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```
    
1. You can add effects on top of effects like this:

    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```
    
1. Play around with some effects and add them to your music. Remember that a complete list of effects can be found in the help section of Sonic Pi under **FX**.

## Step 2: Modifying Parameters

On occasion, you might like to make sounds play for a longer time or at a different rate. This can be achieved easily by modifying the parameters of the code you are using.

Take `play 60`, for example.

1. Click on **help** to open the help documents, then select **lang** on the left hand side, and scroll down to **play**. You will see some examples of its use. So far you have used `play` without any parameters; let's use some now.
1. In a new worksheet type:

    ```ruby
    play 60, attack: 1, release: 3
    ```
    
1. Press the **play** button to hear how that one note sounds. Attack and release control the amplitude of a note over time.

1. Now change the values for attack and release to see how those parameters affect the note.

There are lots of parameters that can also change the way samples or synths sound. Try changing the values for `cutoff:`, `pan:`, `rate:` or `amp:`. For a full list of parameters for each sample click on the **Help** icon, followed by **Samples**, select a sample and scroll down to see a full explanation for each type of paramter that can be used with that sample. Same goes for synths!

For a full list of parameters for each sample, click on the **Help** icon, followed by **Samples**. Select a sample and scroll down to see a full explanation for each type of parameter that can be used with that sample. The same applies for synths!

## Step 3: Using rrand

Sonic Pi includes a number of functions that can add more interesting elements to your music. A really fun function is `rrand`, which will return a value between two specified numbers. For a cool effect, use `rrand` to make the cutoff bounce around.

### Activity Checklist

1. In a blank worksheet type:

    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```
    
1. Instead of passing  a number like `80` to the cutoff value, try `rrand(40, 120)` like this:

    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```
    
1. Then you can start to experiment using `rrand` with other parameters. For example, add `pan: rrand(-1, 1)` to the play chord line and then press **play**.    
