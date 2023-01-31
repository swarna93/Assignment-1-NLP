from nltk.corpus import wordnet as wn

try:
    from utils.med import levenshtein
except:
    from med import levenshtein


    
def return_s(incorrectw):
    dic = {}
    for w in wn.words():
        dic[w]=levenshtein(incorrectw,w)
    sorted_dic = sorted(dic.items(), key=lambda x:x[1])
    top1={}
    for i in range(1):
        top1[i]=sorted_dic[i][0]
    top5={}
    for i in range(5):
        top5[i]=sorted_dic[i][0]
    top10={}
    for i in range(10):
        top10[i]=sorted_dic[i][0]
    return top1, top5, top10
