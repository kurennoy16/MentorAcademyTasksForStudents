CONCURRENCY TASK:
Requirements

1. Create two goroutine’s
    * The first goroutine - sender\client
    * The other - receiver\server
2. The sender, sends every few seconds (specific interval of time) the following data:
    * current time stamp
    * a custom string message
3. The receiver gets the data every 5 seconds and print it.
4. The time interval to send the requests should be set in a config file, and should be in seconds

***Bonus Points:***
* create another goroutine’s that stop the sender and receiver after one min using `context.Context`
