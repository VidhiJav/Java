In this Program, we are generating random text. 
We are using a training text to randomly select keys, where key is an individual word or set of words.
For that particular keys we generate an array List of words which follows it in training text.
from that arrayList of words we randomly select a word to follow key.
That randomly selected word becomes key and we repeat whole process till we have generated enough text.

Main methods used are getfollows and get random text.

get follows method: here we are generating an arryaList of words followed by key.
get random text method: here we are randomly selecting a key and using get follows method to generate next best word to follow.
                         Next word becomes key and process repeats till we reach end.
                         
 Efficient Markov: Since we were iterating a lot while looking for following word, we decided instead to make a hashmap 
                    This map has all keys and following word's arrayList stored . When we generate text using random text method 
                     and call getfollow method, it simply looks in map and return us its following value.It saves lot of time.
                     
                     
