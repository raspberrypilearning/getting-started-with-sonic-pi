## Change the sounds

It's time to make your tune sound more interesting! We can do this by changing the synthesizer sounds it is using. The default Sonic Pi synth is called `beep`.

To use a different synth, you need to add the code `use_synth :name of synth` above the sequence of code you want to use it in.

In this example, `fm` is the name of the synth:

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Synths to try

There are lots of cool-sounding synths included with Sonic Pi. To find the names of them, click on the **help** icon at the top of the screen so that the help documents window appears. Then select **Synths** from the tabs along the left hand side of the help window. Click on any of the synth names to get more information on how to use it.

