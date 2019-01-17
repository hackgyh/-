#＃ - 
#python编写英汉词典
with open("dict.txt",encoding="utf8") as fp:
    a=fp.read()
    b=input("输入单词：")
    c=0
    d=""
    e=""
    while c<len(a):
        if a[c]=="#":
            c+=1
            while a[c]!="\n":
                d+=a[c]
                c+=1
            c+=1
            while a[c]!="\n":
                e+=a[c]
                c+=1
            if b==d:
                print(e)
                break
            d=""
            e=""
        c+=1
