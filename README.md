<h1 align="center">
  <img src="https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/overvue-icons/apple-icon-72x72.png">
  <br/>
  OverVue (Beta)
</h1>

<p align="center"><b>Prototyping Tool for Vue Developers</b></p>

<p>OverVue is a prototyping tool that allows developers to <em>dynamically</em> create and visualize a Vue application, implementing a real-time intuitive <em>tree display</em> of component hierarchy and a live-generated <em>code preview</em>. The resulting boilerplate can be <em>exported</em> as a template for further development.</p>

<p>这个程序能帮你生成Vue 组件, 设置 routes , 也可以帮你显像Component Parent-Child组件树。你只要做一些小配置然后可以下载code boilerplate. 这样你就可以很方便简洁地生成Vue前台APP了！</p>

![](https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/gifs/screenshot.png)

#### Features
+ Upload frontend mockup images for each route
+ Visualize draggable and resizable components
+ Create parent-child hierarchy of components
+ Add html elements to components
+ Create routes to be used by Vue Router
+ Live-generated previewable code snippets for each component
+ Live-generated tree view to aid in visualizing parent-child hierarchy
+ Save projects and open previous projects
+ Export full boilerplate code for a working frontend
+ Undo/redo functionality

###### OverVue 2020 new features and fixes

+ Ability to nest HTML elements
+ Ability to navigate into HTML elements from a selected Vue component
~~+ Ability to have one image per route~~
+ Can now set Vue components to specific layers
+ Improved hierarchy tree rendering
+ Improved Route addition and deletion
+ Improved UI to be more informative
+ UI is more reactive, code snippets update dynamically, Component children menu is consistent with children list at time of creation
+ Extensive bug fixing for Vue component and HTML element deletion behavior, exporting and saving.
+ Will now load route images along with project
+ Windows compatibility for uploading mockup images.

#### How to use
+ Opening the application will create by default a root App component and a root route called "HomeView"
+ Upload a mockup from your filesystem if you'd like. Remove the mockup and choose a new one if needed.
![](https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/gifs/upload-image-drawers.gif)

+ To add a new component, type its name in the component name box and select any HTML elements that should be rendered by that component.
+ HTML elements can also be added after creation by selecting the component in the display, then selecting HTML elements.
+ Select a parent component for the new component if needed.
+ After adding, you can move and resize the component in the display.
![alt text](https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/gifs/component_creation.gif)

+ You can also add children to components by right-clicking the component to add children to, and you can see the tree re-render as you create new components or change the hierarchy.
![](https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/gifs/HTML-elements-tree-rerender.gif)

+ The dashboard shows info about each component (code snippets and HTML elements). Click a component in the display to see its properties.                                               
![](https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/gifs/snippets-active-component.gif)

+ You can add new routes and view all components and routes in the sidebar.
![](https://raw.githubusercontent.com/jeisele2/OverVue/master/src/assets/gifs/sidebar-components-routes.gif)

+ When finished creating, you can export to a file location of your choice. Below is the exported file structure:

```
public/
  index.html
src/
  assets/
  components/
    UserCreatedComponent1.vue
    UserCreatedComponent2.vue
    ...
  views/
    HomeView.vue
    UserCreatedRouteComponent1.vue
    UserCreatedRouteComponent2.vue
    ...
  App.vue
  main.js
  router.js
babel.config.js
package.json
```
###### OverVue 2020 How to
+ Undo/Redo feature has been added to the top right of the program, you can also use CTRL+z and CTRL+y respectively.

+ You can nest html elements in two different ways:
 1. Upon creating a component and adding an html element into it, Select the component to make it the active component.
 Go to the html elements tab and then double click on the html element you wish to be the target for your new elements.
 Once the html element is selected, use the left hand panel and start adding elements like you were adding it to a component.
 2. Similar to above, but instead of double clicking, you can press the down arrow icon on the html element button to enter it.
 From there the view will change to the contents of that particular HTML element.
 You can then add html elements like you would for a component using the left hand side

+ Setting layers on a component is done by right clicking the desired component on the component display and using the menu option
  All components start on layer 1 by default.







#### Running a local version
This app was developed using the Quasar framework, so first you will need to install the Quasar cli
```
npm i -g @quasar/cli
```
Install dependencies
```
npm i
```
To run electron app in dev mode
```
quasar dev -m electron
```
To build a new .dmg
```
quasar build -m electron
```

#### Contributing
We'd love for you to test this application out and submit any issues you encounter. Also feel free to fork to your own repo and submit PRs.
Here are some features we're thinking about adding:
+ Vuex state prototyping and boilerplate export
+ Option to export files in TypeScript
+ Ability to place child components into HTML elements
+ Integration with Storybook
+ Removal of NPM Dependencies
+ Ability to add a copy of an existing component from another route to a new route
+ Fix the incorrect resizing of components when maximizing and minimizing while the compoenent is active.

#### Authors
```
Contributors:
Joseph Eisele @jeisele2
Dean Chung @deanfchung
Dean Ohashi @dnohashi
Drew Nguyen @drewngyen
Alexander Havas @LOLDragoon
Keriann Lin @keliphan
Allison Pratt @allisons11 
              @JojuOlaode
```
Inspired by [PreVue](https://github.com/open-source-labs/PreVue)
