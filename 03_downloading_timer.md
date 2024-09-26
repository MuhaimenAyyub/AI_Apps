# Timer
## Instructions
- We want to create a program to calculate the time it takes to download a file  .
- We ask the user 2 questions. File size in megabytes and internet speed in megabits/second.
- Convert the file size to megabits (1 megabyte = 8 megabits), then calculate the download time
- Display the number of seconds the download will take
- Use your countdown timer to display the download process taking place  
End with printing "download complete!" 

```py
from time import *

file_size = int(input("What is the file size in megabytes?"))
internet_speed = int(input("What is your internet speed in megabits/second?"))

file_size *= 8
download_time = file_size/internet_speed

print("Time to complete download:", round(download_time), "seconds")

countdown = round(download_time)
while countdown > 0:
    print(countdown)
    countdown -= 1
    sleep(1)
print("Download completed!")
```