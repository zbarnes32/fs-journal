# Managing the Fullstack Application

1. Describe the two ways to bind Data in Vue?

  > Text interpolation (aka mustache brackets) and directives.

2. The `SPA` acronym stands for what?

  > Single Page Application

3. What are some of the advantages/uses of a `SPA` over a traditional one?

  > SPAs supports client-facing functionality without having to reload the page. SPAs are also generally faster than traditional when it comes to load times.

4. What does the `onMounted` method in Vue do?

  > Similar to when we used the constructor to draw in MVC, onMounted loads on page load.

5. What is the `v-model` attribute in Vue for, and when might you use it?

  > The v-model is used on a component to implement a two-way binding. Using it on a form's input would allow you to bind that data that was in entered in the value. 

6. What is the package.json file used for?

  > The package.json file is the manifest file of any Node.js project and contains the metadata of the project.

7. Which Vue attributes(directives) could you use to conditionally render elements on a page?

  > v-if and v-else. I believe that there is also a v-else-if.

8. What is the purpose of the `key` attribute when using `v-for` on an element?

  > It is so Vue can tell the elements apart properly.

9. What is the `<slot>` element and what is it used for?

  > The <slot> element is a slot outlet that indicates where the parent-provided slot content should be rendered. In some cases, we may want to pass a template fragment to a child component, and let the child component render the fragment within its own template.
