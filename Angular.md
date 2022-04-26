1. What is two-way binding in Angular?
2. What are directives?
3. What are the types of directives?
4. Is Component a directive?
5. What are pipes?
6. Difference between pure and impure pipes.
7. How to send data from parent component to a child component?
8. How to send data from a child component to the parent component?
9. What is @Input and @Output ?
10. What is NgModule ?
11. What is a service?
12. What are providers ?
13. What are entryComponents ?
14. Difference between AOT compilation and JIT compilation.
15. Explain Angular component lifecycle hooks.
16. Difference between Observables and Promises.
17. Difference between constructor and ngOnInit.
18. Is implementing the OnInit interface mandatory?
19. What are sass files?
20. How to generate components, services and modules using angular-cli? 
21. forroot vs forchild
22. What is NGRX ?
23. Observable vs Promise
24. When to use observables or promises ?
25. switchMap vs mergemap.real time uses for switchMap and Mergemap
11. Services structure in Angular project.
12. Angular lifeCycle hooks
13. ngOnchanges
14. Testing framework
15. End to end test case
16. Jest & cypress
17. Reactive Forms vs template driven form ?
18. Upgrade Angular 6 to Angular 8 ?
17. Why is the constructor always private ?
→> anything marked as private cannot be accessed by the component’s template either. (Private members can be accessed when using JIT, such as at development time, but not when using AOT, such as for production.)
So in your template, you could only do *ngIf='carService.isValid' if the injected service was marked as public.
But actually, best practice is to wrap any service properties/methods in a component property/method anyway and have the template bind to/call the component’s property or method.
