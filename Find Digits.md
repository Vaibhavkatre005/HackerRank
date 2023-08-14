https://www.hackerrank.com/challenges/find-digits/problem?isFullScreen=false&utm_campaign=challenge-recommendation&utm_medium=email&utm_source=24-hour-campaign

![screencapture-hackerrank-challenges-find-digits-problem-2023-08-14-22_13_40](https://github.com/Vaibhavkatre005/HackerRank/assets/67364186/f432b54b-c968-4313-9223-617652d40785)

def findDigits(n):
    # Write your code here
    count=0
    str_n=str(n)
    for i in str_n:
        if (int(i)!=0):
            
            if (n%int(i)==0):
                count+=1

    return count
