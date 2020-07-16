**To run in irb console with default parameters:**
```
require './refactored_task'
FileParser.new.work
```

or you can set input and output filenames
```
FileParser.new('input_filename.txt', 'output_filename.json').work
```


**To run with benchmark:**
```
require 'benchmark'
Benchmark.bm do |x|
  x.report do
    FileParser.new.work
  end
end
```

**Result:**
```
user        system      total       real
153.723993  11.145321   164.869314  (173.480371)
```
