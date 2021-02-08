# #4 MapReduce Basics


__1. What commands did you use to run each script?__

```python3.5 FirstJob.py -r hadoop hdfs:///Data/ > Output_first.csv```

```python3.5 SecondJob.py -r hadoop hdfs:///Data/ > Output_second.csv```

```python3.5 ThirdJob.py -r hadoop hdfs:///Data/ > Output_third.csv```

```python3.5 FourthJob.py -r hadoop hdfs:///Data/ > Output_fourth.csv```


__2. What technical errors did you experience?__ 

I kept getting the `Retrying connect to server` error. I force stopped the execution and retried for 1 or 2 more times, and it worked fine.
I tried restarting the docker multiple times, but have not found a solution yet.


__3. What conceptual difficulties did you experience?__

I was not familiar with `jar` or `class` files, so using them like functions was new to me.  


__4. How much time did you spend on each part of the assignment? Track your time according to the following items: Gitlab & Git, Docker setup/usage, actual reflection work, etc.__

Gitlab & Git: 5 minutes

Docker setup/usage: 1 hour

Actual reflection work: 4~5 days


__5. What was the hardest part of this assignment?__

The hardest part was waiting the execution to be over. It was so slow to check if my function was working correctly with hadoop, which took most of my time on this project.


__6. What was the easiest part of this assignment?__

Creating `Word.txt` file

__7. What did you actually learn from doing this assignment?__

I learned how to make `Mapper()` and `Reducer()` functions run on the hadoop system, that uses STDIN and STDOUT to read the data.
Also, by using the open source framework `MrJob` that wraps the `Hadoop streaming` job, it made process a lot simpler to do MapReduce jobs on Hadoop.


__8. Why does what I learned matter both academically and practically?__ 

MapReduce job is a standard procedure that has been used in a big companies for years since it came out. `MrJob` opensource was created to make tasks simpler. This means there is a huge market that uses MapReduce in small to giant companies. 
This is important as a Data Scientist to realize how big data is managed in the server, and be able to handle them.  