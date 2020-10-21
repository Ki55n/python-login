# python-login



from tkinter import *
import tkinter.message as mb

class loginak(Frame):
    def __inti__(self,master):
        super().__init__(master)
        self.label_username=Label(self,text='Username', font=("Times new roman", 15))
        self.label_password=Label(self,text='Password', font=("Times new roman", 15))
        
        self.entry_username=Entry(self)
        self.entry_password=Entry(self)
        
        self.label_username.grid(row=0,sticky=E)
        self.label_password.grid(row=0,sticky=E)
        self.entry_username.grid(row=0,column=1)
        self.enrty_password.grid(row=1,column=1)
        
        self.button=Button(self,text='login', command=self.login)
        self.button.grid(columnspan=2)
        
        self.pack()
        
        def login(self):
            username=self.entry_username.get()
            password=self.enrty_password.get()
            
            if(username=='AK' and password=='Admin'):
                mb.showinfo("Login", 'Login_successfully')
            
            else:
                mb.showinfo('Login','Login failed')
                
                
                
ak=Tk()
login=Loginak(ak)
ak.mainloop()
            
            
        
