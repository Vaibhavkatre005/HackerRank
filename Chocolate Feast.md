https://www.hackerrank.com/challenges/chocolate-feast/problem?isFullScreen=false&utm_campaign=challenge-recommendation&utm_medium=email&utm_source=24-hour-campaign

![screencapture-hackerrank-challenges-chocolate-feast-problem-2023-08-15-13_15_25](https://github.com/Vaibhavkatre005/HackerRank/assets/67364186/059a8d55-21a4-4cbe-9bf9-7e084ba4897c)


````python
def chocolateFeast(n, c, m):
    # Write your code here
    final_count=0
    no_of_choco=n//c
    final_count=no_of_choco
    
    if no_of_choco%m==0:
        final_count+=(no_of_choco//m)
    else:
        final_count+=(no_of_choco//m)
        final_count+=((no_of_choco%m) + (no_of_choco//m))//m
    return final_count
````



fail case input: https://hr-testcases-us-east-1.s3.amazonaws.com/1104/input05.txt?response-content-type=text%2Fplain&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAR6O7GJNX5DNFO3PV%2F20230815%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230815T074702Z&X-Amz-Expires=7200&X-Amz-SignedHeaders=host&X-Amz-Signature=99e3dfa717e7d646690ed035af66cdb89bc5469a66509204aa0d167a4f803eb6
fail case output: https://hr-testcases-us-east-1.s3.amazonaws.com/1104/output05.txt?response-content-type=text%2Fplain&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAR6O7GJNX5DNFO3PV%2F20230815%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230815T074709Z&X-Amz-Expires=7200&X-Amz-SignedHeaders=host&X-Amz-Signature=c56a85a43acb97cce41d07d5cafb87dfb4c9c4d27a7e196df38e084e9fd04716
