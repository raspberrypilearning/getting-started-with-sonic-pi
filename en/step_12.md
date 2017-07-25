## Use samples

Not only can you create music in Sonic Pi using single notes, you can also create music with samples. Samples are pre-recorded sounds or tunes that you can bring into your music. This is a really simple way to make your music sound amazing!

To use a sample, you need to add the code `sample :name of sample` in the sequence of your music program where you want it to play.

In this example, `loop_amen` is the name of the sample:

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Samples to try

There are lots of samples included with Sonic Pi. To find the names of them, click on **help** followed by **samples** on the left hand side of the help window. Click on any of the sample names to get more information on how to use it. 

