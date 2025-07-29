# r-extension
filename='root.txt'
with open(filename,'w')as f:
    f.write("my full name is kusuma.\n")
with open(filename,'r+')as file:
    print("latest data:")
    print(file.read())
    file.seek(0)
    userinput=input("\n enter text to overwrite from begining..")
    file.write(userinput)
    file.seek(0)
    print("\n file after writed by r+")
    print(file.read())
