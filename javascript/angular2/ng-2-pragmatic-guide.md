# Angular 2 with TypeScript for Beginners - The Pragmatic Guide

## 1. Getting Started

### Architecture

Building blocks
- Component
  - Selector
  - Template
  - Directives
  - Providers (services)
- Directive
- Service
- Router

### Setup Environment
- install typescript (global)
- install typings (global)

```
npm install -g angular-cli

ng new <my-project>
ng serve
```

## 3. Displaying Data and Handling Events

### Property Binding

Property binding is one way binding. Component --> view

3 ways
```
<img src='{{imgUrl}}' />    // interpolation
<img [src]='imgUrl' />      // square brackets
<img bind-src='imgUrl' />   // prefix-bind

```

### Class binding

```
[class.active]="isActive"

```
