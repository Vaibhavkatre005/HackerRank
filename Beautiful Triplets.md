https://www.hackerrank.com/challenges/beautiful-triplets/problem?isFullScreen=false&utm_campaign=challenge-recommendation&utm_medium=email&utm_source=24-hour-campaign
![image](https://github.com/Vaibhavkatre005/HackerRank/assets/67364186/49b942d0-2e02-45d9-b97b-2fdc167bb9e9)

````python
def beautifulTriplets(d, arr):
    # Write your code here
    count=0
    
    for i in range(0, len(arr)):
        local_count=0
        last_index=i
        print("local_count:last_index::",local_count, last_index)
        for j in range(0,3):
            print("\t",j, end="=>")
            if local_count==2:
                count+=1
            print("arr[last_index]+d",arr[last_index]+d)
            if (arr[last_index]+d) in arr:
                last_index=arr.index(arr[i]+d)
                local_count+=1
            else:
                local_count+=0
            
    return count

````
