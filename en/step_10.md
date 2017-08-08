## Adding effects

Modern synthesizers have the ability to add effects to sounds. Sonic Pi is no different: you are able to add studio effects such as reverb, echo and distortion. Of course you have to use code to add the effects!

- In a new worksheet find a sample that you like, for example `sample :guit_e_fifths`

- Wrap the sample in an effects block like this:
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```
    
- You can add effects on top of effects like this:

    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```
    
- Play around with some effects and add them to your music. Remember that a complete list of effects can be found in the help section of Sonic Pi under **FX**.

