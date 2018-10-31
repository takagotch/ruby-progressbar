### ruby-progressbar
---
https://github.com/jfelchner/ruby-progressbar

```sh
progressbar = ProgressBar.create

50.times { progressbar.increment }

progressbar.progress = 50
progressbar.progress += 10
progressbar.progress -= 25
progressbar.progress.total = 50
progressbar.progress.increment
progressbar.progress.decrement 

100.times { progressbar.increment; sleep 0.1 }

```

```ruby
progressbar = ProgressBar.create(format: "\e[0m%t: |%B]\e[0m")
100.times do |i|
  progressbar.increment
  if i == 72
    progressbar.format = "%t: |\e[31m%B\e[0m|"
  end
  sleep 0.1
end

```

```
```


