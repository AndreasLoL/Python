import heapq


tekst = open("Carcosa.txt", "r")
temp1 = tekst.read()
tekst.close()
temp1 = temp1.lower()
dict1 = {}
dict2 = {}
list3 = []
for k in temp1:
	if k.isalpha() == True or k.isdigit() == True:
		if k not in dict1:
			dict1[k] = 1
		else: 
			dict1[k] += 1
list1 = heapq.nlargest(10, dict1, key=dict1.get)
print("Kõige levinumad tähed: ")
for i in range(len(list1)):
	print(str(list1[i]) + " : " + str(dict1[list1[i]]))

temp2 = temp1.split()
for j in temp2:
	if j.isalpha() == True:
		if j not in dict2:
			dict2[j] = 1
		else:
			dict2[j] += 1
list2 = heapq.nlargest(10, dict2, key=dict2.get)
print("Kõige levinumad sõnad: ")
for l in range(len(list2)):
	list3.append(str(list2[l] + ": " +str(dict2[list2[l]])))
print(sorted(list3))
