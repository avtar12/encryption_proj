# encryption_proj Source Code

alphabets='abcdefghijklmnopqrstuvwxyz'
key= 4
new_message =''

message= input('Please enter the message:')

for character in message:
  if character in alphabets:
   position= alphabets.find(character)
   newposition = (position+key)%26

   newchrac= alphabets[newposition]

   new_message += newchrac
   
   
print('your new Message is',new_message)
