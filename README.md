# Exercise3
while True:
    try:
        UserInput= input("請輸入正整數（按enter離開):")
        
        if UserInput=='':
             break
        if int(UserInput)<=0:
            print('請輸入正整數')
            continue
        factors=[]
        for i in range(1,int(UserInput)+1):#UserInput+1=UserInput(電腦從零算起)
            if int(UserInput)%i==0:
                factors.append(i)
        print(f"{int(UserInput)} 的因數是: {factors}")
        
    except ValueError:
        print('請輸入有效正整數')
print('程式結束')
