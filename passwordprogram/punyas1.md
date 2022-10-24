str=input('enter passward')
special=['$','#','*','@']
value=True
l_count=0
d_count=0
s_count=0
u_count=0
if(len(str)<=5):
    value=False
for ch in str:
    if(ch.isupper()):
        u_count+=1
    if(ch.islower()):
        l_count+=1
    if(ch.isalnum()):
        d_count+=1
    if ch in special:
        s_count+=1
if(s_count<1 or d_count<1 or l_count<1 or u_count<1):
    value=False
if(value==False):
    print('invalid')
else:
    print('vaild')


output:
![WhatsApp Image 2022-10-24 at 12 30 37 PM](https://user-images.githubusercontent.com/86178972/197466506-89ec0c54-77f0-4413-a371-5b90d6edf021.jpeg)
![WhatsApp Image 2022-10-24 at 12 30 38 PM](https://user-images.githubusercontent.com/86178972/197466512-68804d0e-1599-48cd-8e65-6e46f1d0975c.jpeg)
