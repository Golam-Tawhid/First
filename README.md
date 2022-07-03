# First
This is just for practice.
class Author:
  def __init__(self,nm="Default",*bk):
    self.name=nm
    self.book=[]
    for i in bk:
      self.book.append(i)
  def addBooks(self,*new):
    for i in new:
      self.book.append(i)
  def printDetails(self):
    print("Author Name: ",self.name)
    print("--------")
    print("List of Books:")
    for i in self.book:
      print(i)
  def changeName(self,nm):
    self.name=nm
  
auth1 = Author('Humayun Ahmed')
auth1.addBooks('Deyal', 'Megher Opor Bari')
auth1.printDetails()
print("===================")
auth2 = Author()
print(auth2.name)
auth2.changeName('Mario Puzo')
auth2.addBooks('The Godfather', 'Omerta', 'The Sicilian')
print("===================")
auth2.printDetails()
print("===================")
auth3 = Author('Paolo Coelho', 'The Alchemist', 'The Fifth Mountain')
auth3.printDetails()
