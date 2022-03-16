# Class02 Reading Notes
---
[React Lifescycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093#id_token=eyJhbGciOiJSUzI1NiIsImtpZCI6ImQ2M2RiZTczYWFkODhjODU0ZGUwZDhkNmMwMTRjMzZkYzI1YzQyOTIiLCJ0eXAiOiJKV1QifQ.eyJpc3MiOiJodHRwczovL2FjY291bnRzLmdvb2dsZS5jb20iLCJuYmYiOjE2NDczODYwNzYsImF1ZCI6IjIxNjI5NjAzNTgzNC1rMWs2cWUwNjBzMnRwMmEyamFtNGxqZGNtczAwc3R0Zy5hcHBzLmdvb2dsZXVzZXJjb250ZW50LmNvbSIsInN1YiI6IjExMzc3NjQzNjI1NjY3ODIzNTg1OCIsImVtYWlsIjoibWljaGVsbGVzYWxhemFyMDEwQGdtYWlsLmNvbSIsImVtYWlsX3ZlcmlmaWVkIjp0cnVlLCJhenAiOiIyMTYyOTYwMzU4MzQtazFrNnFlMDYwczJ0cDJhMmphbTRsamRjbXMwMHN0dGcuYXBwcy5nb29nbGV1c2VyY29udGVudC5jb20iLCJuYW1lIjoiTWljaGVsbGUgU2FsYXphciIsInBpY3R1cmUiOiJodHRwczovL2xoMy5nb29nbGV1c2VyY29udGVudC5jb20vYS9BQVRYQUp6NGtKXzlqZjF3OGdSUkp2QXM4RkNXWFVVelJPaVdjVE9jc0xiSD1zOTYtYyIsImdpdmVuX25hbWUiOiJNaWNoZWxsZSIsImZhbWlseV9uYW1lIjoiU2FsYXphciIsImlhdCI6MTY0NzM4NjM3NiwiZXhwIjoxNjQ3Mzg5OTc2LCJqdGkiOiIyMDA3Y2I3NmQ2NDA4MGQzMWI2ZDdhZmVmNWNhMGFhNmRiMzY1NjQyIn0.BYk_G_Z8-avzGm8JGHcJ2rUsEv0toadtJdtjtTOIPzt4hRuOSw3Cfg131yULb3ZQ_A-164uBFhUrYWMW5BwfJP5XJiQy9QV5dLyaYGVILjKT-UrwaIEncyYIN-f764xwjSt5y-e5S8oM2u-q4TBMrlklMvADr_znnMSevMtHDwTHl1pWX-LfmvBFaUvuzrelAmAYZzDwuM-aXPtUctqc88rhyOKab8gwwJkj6rrgPJ01pzMiPolkdkIYIFMrJo5CH4r13IIZMDeJNs6i-gIkKzpiTVRMvNdlLy3XUEoUJQcZZvoMzkuQWe-dVEKuSf6NncUi-0tXvkYO3FBLUScwYw)

### Questions
1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? ***The render method happens first.***   
2. What is the very first thing to happen in the lifecycle of React? ***The first thing to happen is mounting.***   
3. Put the following things in the order that they happen:   
* constructor
* render
* React Updates
* componentDidMount
* componentWillUnmount

4.  What does componentDidMount do?   

[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)
### Questions
1. What types of things can you pass in the props?
  the parts of the constructor, data
2. What is the big difference between props and state?
  props you pass into a component and handled outside of the component, state is handled inside the component. 
3. When do we re-render our application?
  when the state changes
4. What are some examples of things that we could store in state? form data that needs to be stored

### Notes
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events.   

props are passed down from parent and do not change in the component. 

State should be used when the information will be handled only inside the component 

![React Lifecycle](https://miro.medium.com/max/1244/1*4y9V5936WdJKaIeVPFEa3w.png)
----
## Things I want to know more about


---
### [Home](https://github.com/MISalz/301_Reading_Notes)