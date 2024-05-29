# R&D Process and Technique
The more I engage in industrial coding environment, the more I realise coding is solely 20% of the process while the majority relies on a good documentation. 
The hardest framework to learn is always those who do not have an official available reference.

A well written documentation can facilitate other people to comprehend one's code and thus making the code outlive the original creator.

Here are the techniques that I have learnt:

## Data flow Diagram
  Dataflow diagram provides a visual overview of an application's mechanism. Swim lane diagram is a great tool to present the application to nontechnical personnel.

## Wireframe Diagram
  Wireframe visualizes the design. And it is much easier to alter than css. I highly recommend Figma.
  
## Framework Documentation
  Indicate what framework you are using. Which version and the link to the official documentation. I also like to provide package.json snippet.

## Feature List
A list feature for the nontechnical personnel.

## src Documentation
I like to use windows `tree /F`

## Hierarchy Diagram
Which file is root, which file imports which file

## Library Documentation
Every method, every function, with their args and default args and usage.


# R&D steps
Monday.com is a good tool.
- Assessment
- Development
- Testing and Validation
- Project Launch and Development
- Post-Mortem and Maintenance

# React web structure
```
│   App.css
│   App.js
│   index.js
│
├───asset
│
├───component
│       logo.jsx
│
├───cssFolder
│
├───layout
│       layout.jsx
│
├───pages
│   ├───action-pages
│   │   
│   ├───auth-pages
│   │       loginPage.jsx
│   │
│   ├───board-pages
│   │   │   mainPage.jsx
│   │   │
│   │   └───mainPage-component
│   │
│   └───utility-page
├───routes
│       routeList.jsx
│
└───utils
```


```
/public/index.html
│
├───/index.js
    ├───/App.js
    ├───/App.css 
    ├───##bootstrap css
        ├───/routes/routeList.jsx
            ├─── /pages/auth-pages/loginPage.jsx
            ├───/layout/layout.jsx
                ├───/component/navbar
                ├─── /pages/board-pages/mainPage.jsx
                    ├───/pages/board-pages/mainPage-component

                ├─── /pages/action-pages/createPage.jsx
                    ├───/pages/board-pages/createPage-component

                ├─── /pages/action-pages/ratePage.jsx
                    ├───/pages/board-pages/ratePage-component

                ├─── /pages/action-pages/approvePage.jsx
                    ├───/pages/board-pages/approvePage-component


```
