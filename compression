def compress(text):
  compressed=""
  count=1
  for i in range(1,len(text)):
    if text[i]==text[i-1]:
      count+=1
    else:
      compressed+=str(count)+text[i-1]
      count=1
  compressed+=text[-1]+str(count)
  return compressed
with open("inputs.txt","w") as f: # Changed mode from "r" to "w"
  f.write("AAGGTTT66")
with open("inputs.txt","r") as f:
  data=f.read()
compressed_data=compress(data)
with open("compressed.txt","w") as f:
  f.write(compressed_data)
  print("original:",data)
  print("compressed:",compressed_data)
