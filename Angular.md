**1. What is two-way binding in Angular?**

  Two-way binding gives components in your application a way to share data.
  Use two-way binding to listen for events and update values simultaneously between parent and child components.


**2.What are directives?**

  Directives are classes that add additional behavior to elements in your Angular applications. 
  Use Angular's built-in directives to manage forms, lists, styles, and what users see.

**3. What are the types of directives?**

  There are three types of Angular directives are as follows:

    1.Component: Used with a template. This type of directive is the most common directive type.

    2.Attribute directives : Change the appearance or behavior of an element, component, or another directive.

    3.Structural directives:Change the DOM layout by adding and removing DOM elements.

**4. Is Component a directive?**

  Yes, componet is a directive.
   
**5. What are pipes?**

  Pipes are simple functions to use in template expressions to accept an input value and return a transformed value.
 
  Pipes are useful because you can use them throughout your application, while only declaring each pipe once.

**6. Difference between pure and impure pipes.**

 A pure pipe is only called when Angular detects a change in the value or the parameters passed to a pipe.

 An impure pipe is called for every change detection cycle no matter whether the value or parameter(s)
**7. How to send data from parent component to a child component?**
Pass data from parent to child component using @Input() decorator, which allows data to pass through templates.

**8. How to send data from a child component to the parent component?**

  Pass data from child to parent component using @Output() decorator with the help of Event Emitter.

**9. What is @Input and @Output ?**

@Input() and @Output() allow Angular to share data between the parent context and child directives or components. 

An @Input() property is writable while an @Output() property is observable.

**10. What is NgModule ?**

An NgModule is a class marked by the @NgModule decorator. @NgModule takes a metadata object that describes how to compile a component's template and how to create an injector at runtime. It identifies the module's own components, directives, and pipes, making some of them public, through the exports property, so that external components can use them. @NgModule can also add service providers to the application dependency injectors.

**11. What is a service?**

    Services are objects that provide common functionality to support other building blocks in an application, such as directives, components, and pipes. What’s important about services is the way that they are used, which is through a process called dependency injection. Using services can increase the flexibility and scalability of an Angular application, but dependency injection can be a difficult topic to understand.” (Pro Angular (chapter 20))
Actually services can manage to distribute objects as services using by dependency injection.

**12. What are providers ?**

A provider is an object declared to Angular so that it can be injected in the constructor of your components, directives and other classes instantiated by Angular.


A Service is a JavaScript object that exists in your application, and a Provider is the way you gain access to that object. The two are not the same thing, but they work together to make your Service accessible from other places. You can't get your Service without a Provider, and a Provider needs something to provide.

**13. What are entryComponents ?**

An entry component is any component that Angular loads imperatively, (which means you're not referencing it in the template), by type. You specify an entry component by bootstrapping it in an NgModule, or including it in a routing definition.

**14. Difference between AOT compilation and JIT compilation.**

JIT downloads the compiler and compiles code exactly before Displaying in the browser. AOT has already complied with the code while building your application, so it doesn't have to compile at runtime. Loading in JIT is slower than the AOT because it needs to compile your application at runtime.

**15. Explain Angular component lifecycle hooks.**

constructor
This is invoked when Angular creates a component or directive by calling new on the class.

ngOnChanges
Invoked every time there is a change in one of th input properties of the component.

ngOnInit
Invoked when given component has been initialized.
This hook is only called once after the first ngOnChanges

ngDoCheck
Invoked when the change detector of the given component is invoked. It allows us to implement our own change detection algorithm for the given component.

Important
ngDoCheck and ngOnChanges should not be implemented together on the same component.
Note
We will cover this hook in more detail in the Advanced Components section at the end of this course.
ngOnDestroy
This method will be invoked just before Angular destroys the component.
Use this hook to unsubscribe observables and detach event handlers to avoid memory leaks.

Hooks for the Component’s Children
These hooks are only called for components and not directives.

ngAfterContentInit
Invoked after Angular performs any content projection into the component’s view (see the previous lecture on Content Projection for more info).

ngAfterContentChecked
Invoked each time the content of the given component has been checked by the change detection mechanism of Angular.

ngAfterViewInit
Invoked when the component’s view has been fully initialized.

ngAfterViewChecked
Invoked each time the view of the given component has been checked by the change detection mechanism of Angular.


**17. Difference between Observables and Promises.**
**18. Difference between constructor and ngOnInit.**

ngOnInit() will be called when it finishes rendering the component. So the first main difference between constructor and ngOnInit method is constructor called by JavaScript engine whereas ngOnInit() called by Angular.

**19. Is implementing the OnInit interface mandatory?**

No its not mandatory. you don't want to use then no need to implement but if you want to do something when component render then you have only one place for do constructor.

21. What are sass files?
22. How to generate components, services and modules using angular-cli? 
23. forroot vs forchild
24. What is NGRX ?
25. Observable vs Promise
26. When to use observables or promises ?
27. switchMap vs mergemap.real time uses for switchMap and Mergemap
28. Services structure in Angular project.
30. Testing framework
31. End to end test case
32. Jest & cypress
33. Reactive Forms vs template driven form ?
34. Upgrade Angular 6 to Angular 8 ?
35. Why is the constructor always private ?
→> anything marked as private cannot be accessed by the component’s template either. (Private members can be accessed when using JIT, such as at development time, but not when using AOT, such as for production.)
So in your template, you could only do *ngIf='carService.isValid' if the injected service was marked as public.
But actually, best practice is to wrap any service properties/methods in a component property/method anyway and have the template bind to/call the component’s property or method.

**20.What is the difference between declarations and entryComponents?**

entryComponents are used to register components for offline computation in a module. These components are referenced here as they not referenced anywhere else in HTML template. Declarations are used to make Directives(components, pipes etc.) in a specific module.

**Methods of improving the performance**
1.Using AoT Compilation.
2.Using OnPush Change Detection Strategy.
3.Using Pure Pipes.
4.Unsubscribe from Observables.
5.Lazy Loading.
6.Use trackBy option for For Loop.
7.Avoid computation in template files.
8.Usage of Web Workers.

https://www.xenonstack.com/blog/performance-optimization-in-angular

**Secure Angular Application**
1.Prevent an application from Cross-Site Scripting (XSS) 
2.Use Route guards when required.
3.Implement CSP (Content Security Policies).
4.Do not use DOM's APIs directly.
5.Prevent CSRF (Cross-site request forgery).
6.Prevent Cross-Site Script Inclusion (XSSI).
7.Keep current with the latest Angular library releases	
8.Don't modify your copy of Angular	Private.
9.Avoid Angular APIs marked in the documentation as "Security Risk
