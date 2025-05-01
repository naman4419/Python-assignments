
class Matrix:
    def __init__(self, lst=[[0,0,0],[0,0,0],[0,0,0]]):
           self.mat=lst
           
    def __add__(self, m2):
        ans=Matrix()
        for i in range(3):
            for j in range(3):
                ans.mat[i][j]=self.mat[i][j]+m2.mat[i][j]
        return ans

    def __mul__(self, m2):
        ans=Matrix()
        for i in range(3):
            for j in range(3):
                ans.mat[i][j]=self.mat[i][0]*m2.mat[0][j] + self.mat[i][1]*m2.mat[1][j]  + self.mat[i][2]*m2.mat[2][j]
        return ans

    def transpose(self, m2):
        ans=Matrix()
        for i in range(3):
            for j in range(3):
                ans.mat[i][j] = self.mat[j][i]
        return ans
    
    def display(self):
        for i in range(3):
            for j in range(3):
                print(self.mat[i][j],end=' ')
            print("\n")

print("Additon")
print()
m1=Matrix([[1,2,3],[4,5,6],[7,8,9]])
m2=Matrix([[9,8,7],[6,5,4],[3,2,1]])
m3=m1+m2
m3.display()
print("Multiplication")
print()
m4=m1 * m2
m4.display()
print("Transpose")
print()
m4=m1.transpose(m2)
m4.display()
