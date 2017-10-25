# テクノロジー（藤原）10/25授業

```
shin4050:~/workspace $ [ ! -f ~/.ssh/id_rsa ] && ssh-keygen -t rsa
shin4050:~/workspace $ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCubGCyOSjKH+rxT3hA2zBFLz9NiHmQUZUJVQSDHeMACTjoNEjYKg3y9hVjzFp+NljMkWd+ktoItT/65Ti/UGJoArRI/BiqXwJs/uNvsG7Zc5B9bFIP2RR9KrA/TKtuiMGgORcpWP91ce0aVVHI0zYU5bYR7jm4qFKHdDEKRJmP6DbBvOsgaqW8VR/qobJEuk4f1u/aoS9hUhHfNTDfLM/B4GWYmjU0fUcM5hvxf67on26TxIVMBOfCKceI+2MWYziNaft4AsdBtEpaQ9jowoAdX/lKCTTIzSIPlJCCNPvYXCj+f2GtwJE8MbIitLjulLCb4i702a+Age4/Mx84+u1euYt2FJsaVra2gUNRG7p6ZbxM/XideD5f6kMRUvlS5Y7O4LuoLfLn0ICdbIKNTaVXqEmMNUAk4106Sl+uIiWl1DFWpXOp9qjnsYaJspDM4RWul/SKS75nwA+irT5vXHO/8d4CsQOry7Qabvh7ijYTFx5ICqLzLJSaPt4rIh6juKtTgbRDBSRFNGKeifWDDUy6pe60bRK1hj4gA5AIFmTZRhLh3AZ1Ae5oMNPwA1LKba6BI2nb/I2JVFOjbCUuABZSjf0492UDQmYYbW6FuIKB1sgsrMmn7OikeniAh/elC+nUxHJj+/Ge9ij0+3WzWKQ9iP63EHGDfe8/2Gtj77pKfQ== kd1261465@st.kobedenshi.ac.jp
shin4050:~/workspace $ ssh -T git@github.com
Warning: Permanently added 'github.com,192.30.255.113' (RSA) to the list of known hosts.
Hi shin4050! You've successfully authenticated, but GitHub does not provide shell access.
shin4050:~/workspace $ ssh -T git@github.com
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
Hi shin4050! You've successfully authenticated, but GitHub does not provide shell access.
shin4050:~/workspace $
shin4050:~/workspace $ ssh -T git@github.com
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
Hi shin4050! You've successfully authenticated, but GitHub does not provide shell access.
shin4050:~/workspace $ git clone git@github.com:shin4050/lecture-1025.git
Cloning into 'lecture-1025'...
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
remote: Counting objects: 6, done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 0), reused 6 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.
shin4050:~/workspace $ git clone https://github.com/shin4050/project2-server-app.git
Cloning into 'project2-server-app'...
remote: Counting objects: 7, done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 7 (delta 0), reused 7 (delta 0), pack-reused 0
Unpacking objects: 100% (7/7), done.
shin4050:~/workspace $ 
shin4050:~/workspace $ pry
[1] pry(main)> puts "こんにちは"
こんにちは
=> nil
[2] pry(main)> print "こんにちは"
こんにちは=> nil
[3] pry(main)> p "こんにちは"
"こんにちは"
=> "こんにちは
[4] pry(main)> message = "こんにちは"
=> "こんにちは"
[5] pry(main)> puts message
こんにちは
=> nil
[6] pry(main)> num = 123
=> 123
[7] pry(main)> puts num
123
=> nil
[8] pry(main)> puts message.length
5
=> nil
[10] pry(main)> 1234
=> 1234
[11] pry(main)> 1234.class
=> Integer
[12] pry(main)> 3.14.class
=> Float
[13] pry(main)> (3.14).class
=> Float
[14] pry(main)> 1234 #Integer
=> 1234
[15] pry(main)> 1234.class
=> Integer
[16] pry(main)> Math::PI
=> 3.141592653589793
[17] pry(main)> 'こんにちは'
=> "こんにちは"
[18] pry(main)> "さようなら"
=> "さようなら"
[19] pry(main)> 'ぐり'+'と'+'ぐら'
=> "ぐりとぐら"
[20] pry(main)> name='いまにし'
=> "いまにし"
[21] pry(main)> puts "#[name]さん、こんにちは"
#[name]さん、こんにちは
=> nil
[22] pry(main)> puts "#{name}さん、こんにちは"
いまにしさん、こんにちは
=> nil
[23] pry(main)> puts "\nさようなら\n"

さようなら
=> nil
[24] pry(main)> a=4;b="9"
=> "9"
[25] pry(main)> a;b
=> "9"
[26] pry(main)> a+b
TypeError: String can't be coerced into Integer
from (pry):26:in `+'
[27] pry(main)> a=4; b="9"
=> "9"
[28] pry(main)> a+b
TypeError: String can't be coerced into Integer
from (pry):28:in `+'
[30] pry(main)> a.to_s+b
=> "49"
[34] pry(main)> (a.to_s + b).class                                          
=> String
[35] pry(main)> a+b.to_i
=> 13
[36] pry(main)> (a+b.to_i)
=> 13
[38] pry(main)> (a+b.to_i).class
=> Integer
[39] pry(main)> animals=["いぬ","ねこ","ぞう"]
=> ["いぬ", "ねこ", "ぞう"]
[40] pry(main)> animals
=> ["いぬ", "ねこ", "ぞう"]
[41] pry(main)> animals[0]
=> "いぬ"
[42] pry(main)> animals[1]
=> "ねこ"
[43] pry(main)> animals[1]="こうもり"
=> "こうもり"
[44] pry(main)> animals
=> ["いぬ", "こうもり", "ぞう"]
[45] pry(main)> animals[3]
=> nil
[46] pry(main)> animals.push("くじら")
=> ["いぬ", "こうもり", "ぞう", "くじら"]
[47] pry(main)> animals
=> ["いぬ", "こうもり", "ぞう", "くじら"]
[48] pry(main)> animals.pop
=> "くじら"
[49] pry(main)> animals
=> ["いぬ", "こうもり", "ぞう"]
[52] pry(main)> colors=[]
=> []
[53] pry(main)> colors.empty?
=> true
[54] pry(main)> colors.length
=> 0
[55] pry(main)> colors=["赤","青","黄","ピンク"]
=> ["赤", "青", "黄", "ピンク"]
[56] pry(main)> colors.empty?
=> false
[57] pry(main)> colors.length
=> 4
```