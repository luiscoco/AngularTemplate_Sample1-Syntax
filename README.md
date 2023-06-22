# Template-Syntax

https://angular.io/guide/template-syntax

In Angular, the template syntax refers to the way you write and interact with the HTML templates in your Angular components. The template syntax includes a set of directives, interpolation, binding, and other features that allow you to build dynamic and interactive user interfaces.

In Angular, a template is a chunk of HTML. Use special syntax within a template to build on many of Angular's features.

Before learning template syntax, you should be familiar with the following: Angular concepts, JavaScript, HTML, CSS

Each Angular template in your application is a section of HTML to include as a part of the page that the browser displays. An Angular HTML template renders a view, or user interface, in the browser, just like regular HTML, but with a lot more functionality.

When you generate an Angular application with the Angular CLI, the app.component.html file is the default template containing placeholder HTML.

The template syntax guides show you how to control the UX/UI by coordinating data between the class and the template.

Extend the HTML vocabulary of your applications With special Angular syntax in your templates. For example, Angular helps you get and set DOM (Document Object Model) values dynamically with features such as built-in template functions, variables, event listening, and data binding.

Almost all HTML syntax is valid template syntax. However, because an Angular template is part of an overall webpage, and not the entire page, you don't need to include elements such as html, body, or base, and can focus exclusively on the part of the page you are developing.

To eliminate the risk of script injection attacks, Angular does not support the script element in templates. Angular ignores the script tag and outputs a warning to the browser console. For more information, see the Security page.

Here are some examples of the template syntax in Angular:

## Interpolation:
Interpolation is denoted by double curly braces ({{}}) and allows you to insert dynamic values from your component into the template. For example:

```typescript
<h1>Welcome, {{ username }}!</h1>
```

In this example, the value of the username property from the component will be dynamically inserted into the template.

## Property Binding:
Property binding allows you to bind the value of a property from your component to an attribute or property of an HTML element. It is denoted by square brackets ([]). For example:

```typescript
<input [value]="userInput">
```

In this example, the value of the userInput property from the component will be bound to the value attribute of the input element.

## Event Binding:
Event binding allows you to bind an event from an HTML element to a method in your component. It is denoted by parentheses (()). For example:

```typescript
<button (click)="submitForm()">Submit</button>
```

In this example, when the button is clicked, the submitForm() method from the component will be called.
 
## Structural Directives:
Structural directives allow you to conditionally render or manipulate the structure of the DOM. Some common structural directives in Angular are ngIf, ngFor, and ngSwitch. For example:

```typescript
<div *ngIf="isLoggedIn">Logged in!</div>
<ul>
  <li *ngFor="let item of items">{{ item }}</li>
</ul>
```

In this example, the ngIf directive conditionally renders the div element based on the value of the isLoggedIn property. The ngFor directive loops over the items array and generates a li element for each item.

These are just a few examples of the template syntax in Angular. Angular provides a rich set of features and directives that enable you to build dynamic and interactive web applications.

https://angular.io/guide/template-syntax
## More on template syntax
You might also be interested in the following:

## Interpolation:	
Learn how to use interpolation and expressions in HTML.
## Template statements:	
Respond to events in your templates.
## Binding syntax:	
Use binding to coordinate values in your application.
## Property binding:	
Set properties of target elements or directive @Input() decorators.
## Attribute, class, and style bindings:	
Set the value of attributes, classes, and styles.
## Event binding:	
Listen for events and your HTML.
## Two-way binding:	
Share data between a class and its template.
## Built-in directives:	
Listen to and modify the behavior and layout of HTML.
## Template reference variables:	
Use special variables to reference a DOM element within a template.
## Inputs and Outputs:	
Share data between the parent context and child directives or components
## Template expression operators:	
Learn about the pipe operator (|), and protect against null or undefined values in your HTML.
## SVG in templates:	
Dynamically generate interactive graphics.
