https://www.hackerrank.com/challenges/the-time-in-words/problem?isFullScreen=false&utm_campaign=challenge-recommendation&utm_medium=email&utm_source=24-hour-campaign
![screencapture-hackerrank-challenges-the-time-in-words-problem-2023-08-14-22_58_00](https://github.com/Vaibhavkatre005/HackerRank/assets/67364186/065b79ce-4a5b-477e-8b56-8b3aef53ccee)

'''
def timeInWords(h, m):
    num_to_words = {
    1: 'one', 2: 'two', 3: 'three', 4: 'four', 5: 'five',
    6: 'six', 7: 'seven', 8: 'eight', 9: 'nine', 10: 'ten',
    11: 'eleven', 12: 'twelve', 13: 'thirteen', 14: 'fourteen', 15: 'fifteen',
    16: 'sixteen', 17: 'seventeen', 18: 'eighteen',
    19: 'nineteen', 20: 'twenty', 21: 'twenty one',
    22: 'twenty two', 23: 'twenty three', 24: 'twenty four',
    25: 'twenty five', 26: 'twenty six', 27: 'twenty seven',
    28: 'twenty eight', 29: 'twenty nine'
    }
    # Write your code here
    timeinword=""
    if (m==1):
        timeinword=(num_to_words[m]+" minute past "+num_to_words[h])
    elif (m>1 and m<15):
        timeinword=(num_to_words[m]+" minutes past "+num_to_words[h])
    elif(m==15):
        timeinword=("quarter past "+num_to_words[h])
    elif(m>15 and m<30):
        timeinword=(num_to_words[m]+" minutes past "+num_to_words[h])
    elif(m==30):
        timeinword=("half past "+num_to_words[h])
    elif((m>30 and m<45)or (m>45 and m<60)):
        timeinword=(num_to_words[(60-m)]+ " minutes to "+num_to_words[h+1])
    elif(m==45):
        timeinword=("quarter to "+num_to_words[h+1])
    else:
        timeinword=(num_to_words[h]+" o' clock")
    return timeinword
'''
