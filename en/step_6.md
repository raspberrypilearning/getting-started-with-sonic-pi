## Using rrand

Sonic Pi includes a number of functions that can add more interesting elements to your music. A really fun function is `rrand`, which will return a value between two specified numbers. For a cool effect, use `rrand` to make the cutoff bounce around.

- In a blank worksheet type:

    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```
    
- Instead of passing  a number like `80` to the cutoff value, try `rrand(40, 120)` like this:

    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```
    
- Then you can start to experiment using `rrand` with other parameters. For example, add `pan: rrand(-1, 1)` to the play chord line and then press **play**.    

