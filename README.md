            

Aim:
To calculate the maximum range of a radar system using the Radar Range Equation and verify the results through Scilab programming.


Apparatus Required

Scilab
Laptop

Theory:
The Radar Range Equation is a fundamental formula used in radar system design to determine the maximum range at which a radar can detect a target. It is given by:

<img width="457" height="528" alt="image" src="https://github.com/user-attachments/assets/a04cf396-8a33-4f05-9b91-f927ea31ef85" />


Program 
`````
Gt=40;
Gr=50;
lambda=0.03;
sigma=1;
Pmin=1e-10;
Pt=[1 2 3 4 5 6 7 8 9 10];
Rmax1=((Pt.*Gt.*Gr.*lambda^2.*sigma)./((4*3.14)^3.*Pmin)).^(1/4);
subplot(2,1,1);
plot(Pt,Rmax1);
xgrid
Pmin2=1e-12:1e-12:1e-9;
Pt2=50;
Rmax2=((Pt2.*Gt.*Gr.*lambda^2.*sigma)./((4*3.14)^3.*Pmin2)).^(1/4);
subplot(2,1,2);
plot(Pmin2,Rmax2);
xgrid


`````
Out Put Graph
<img width="1919" height="1126" alt="image" src="https://github.com/user-attachments/assets/0b6da26a-42e5-4e26-be72-7fe6e74c8e67" />

Table Calculation 

<img width="1600" height="936" alt="image" src="https://github.com/user-attachments/assets/b3182c4f-9e7b-4823-94de-4bbd22640f5b" />
<img width="1335" height="1600" alt="image" src="https://github.com/user-attachments/assets/0c7b78e2-abd8-475c-b753-50d964df19ee" />


Result:

Thus, the maximum range of a radar system using the Radar Range Equation is verified through a Python program.
