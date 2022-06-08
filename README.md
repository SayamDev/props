
![image](https://user-images.githubusercontent.com/101875083/172724696-1db1188b-132d-455a-8e3e-6158ca552abc.png)



-Can pass props downwards - like a tree
-Cannot pass props upwards to parents.
-Props are read only, therefore cannot modify the prop in the child component, if we want to modify it, have to modify it in the top component first using state



What I have done in App.js is created a component called Product which will have 3 props = name, description, price.
And what i have done in the Product.js is , first of all created a component called Product and passed props into the parameter and also passed the 3 props i created in the App.js
Here 
![image](https://user-images.githubusercontent.com/101875083/172724733-f7b92692-1cb1-4e39-bb9e-08630ec9a53f.png)


With this now, i can use the one component and use it over and over again all over the application
![image](https://user-images.githubusercontent.com/101875083/172724757-575b80e1-f134-43d9-8883-90f6453f0f4b.png)









We can also object desctrucutre the object and grab the element directly and then rerender it
![image](https://user-images.githubusercontent.com/101875083/172724782-387096f1-ae77-4739-a6ba-8f6e409d96bb.png)








And now what we need to do now is create a sub component called ItemDescription and pass the props down to that one (remember tree structure can only pass down prop)





Therefore I created a sub component called ItemDescription and i am only passing the name and the description since i want the name & the description to appear on the product
![image](https://user-images.githubusercontent.com/101875083/172724803-178bf088-5d2f-4013-9282-ffaf14b4acf5.png)





Here i have passed the props into the ItemDescription component in the ItemDescription.js but havent passed the props in the Product.js
![image](https://user-images.githubusercontent.com/101875083/172724826-c5ce2bb7-9208-42bd-a1c3-78e17c06e495.png)







Passed the 1st prop into the 
![image](https://user-images.githubusercontent.com/101875083/172724854-8bc63957-d526-4eef-afde-672747cd48ba.png)




2nd prop passed from the 2nd component 
![image](https://user-images.githubusercontent.com/101875083/172724881-2612bf6d-28ad-4c1f-a2ca-b41bde25b9f9.png)




The price prop was not used in the ItemDescription sub component, so we just called it like this
![image](https://user-images.githubusercontent.com/101875083/172724895-af08027f-c38b-4cbd-a2fc-7dbd4cc0149c.png)


