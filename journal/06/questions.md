# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > main.js

02. What is the difference between a vue `component` and `page`?

  > Components are files that we can create that is great for reusable code where as a Vue page is similar to a view in MVC.

03. What is ***Component-Based Architecture***?

  > Component-based architecture is a framework for building software based on reusable parts.

04. What are the three tags that make up a Vue component?

  > Script, Template, and Style

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > Lifecycle hooks are functions that allow users the opportunity to add their own code at specific stages.

06. Which component in Vue does the vue-router use to mount pages onto?

  > RouterLink

07. What is the difference between the `AppState` and the state object within a component?

  > The AppState is global while a state object within a component is local.

08. What is the responsibility of `Services` in our Vue projects?

  > The same as in our MVC project. It handles the business logic.

09. What are ***props*** and how are they used? Provide an example

  > Props is a configuration option in Vue. With props we can pass data to the components via custom attributes to the component tag. An example could be when we use the defineProps function and create a prop with a key/value pair with access to the attributes.

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > watchEffect
