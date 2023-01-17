# nltk
pip install nltk
import nltk
nltk.download('punkt')
from nltk.probability import FreqDist
text1="India will play against Australia this summner . It will be an exciting series" 
print(text1)
word_tokens=nltk.word_tokenize(text1)
print(word_tokens)
len(word_tokens)
text1=FreqDist(word_tokens)
print(text1)
text1.most_common(10)
text1.freq("India")
import matplotlib.pyplot as plt
fig, ax=plt.subplots(figsize=(10,5))
text1.plot(10)
pip install wordcloud
from wordcloud import WordCloud, STOPWORDS
pip install wikipedia
import wikipedia
pip install PIL
from PIL import Image
stop_w=set(STOPWORDS)
info=("Artificial Intelligence and Machine Learning")
print(info)
word_cloud=WordCloud(stopwords=stop_w).generate(info)
img=word_cloud.to_image() 
img.show()
 
