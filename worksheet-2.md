# Taking Sonic Pi 2 Further

Sonic Pi 2 is so awesome, that there are just too many features to mention in just one tutorial! If you are feeling like you have got to grips with the [first page](worksheet.md) and you would like to try some other ways to code music then follow the steps below.

## Step 1: Adding effects
Modern syntherziers have the ability to add effects to sounds. Sonic Pi 2 is no different, you are able to add studio effects such as reverb, echo and distortion. Of course you have to use code to add the effects!

### Activity Checklist
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
1. Play around with some effects and add them to your music, remember that a complete list of effects can be found in the help section of Sonic Pi 2 under **FX**

## Step 2: Modifying Parameters
On occasion you might like to make sounds play longer, or at a different rate. This can be achieved easily by modifying the parameters of the code you are using.

Take `play 60` for example. 

###Activity Checklist
1. Click on **help** to open the help documents, then select **lang** on the left hand side, and scroll down to **play**. You will see some examples of it's use. So far you have used `play` wuthout any parameters. Let's use some now.
1. In a new worksheet type:

    ```ruby
    play 60, attack: 1, release: 3
    ```
1. Press the **play** button to hear how that one note sounds. Attack and release control the amplitude of a note over time.
1. Now change the values for attack and release to see how those parameters affect the note.

