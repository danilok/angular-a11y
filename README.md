# A11yP1

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.1.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

# Angular: design de components com acessibilidade

# 01. Preparando o terreno, primeiro componente

- Revisão de estrutura de um componente
- `Input binding` vs `Event Binding`
- O padrão para podermos utilizar `two-way data binding`

# 02. Integração com Reactive Forms

- Como integrar um _custom component_ com `Reactive Forms`
- A _interface_ `ControlValueAccessor`
- O papel do _token_ `NG_VALUE_ACCESSOR`
- A utilizar `ngModel` e `formControlName` com um _custom component_

Na aula foi demonstrado que o componente é compatível com `ngModel` e `formControlName`. Caso fosse necessário apenas manter o acesso via `formControlName`, o que é necessário retirar são os `Input()` e `Output()` do `value` do componente. Desta forma, não seria mais possível usar o `[(ngModel)]` para acessar/alterar valores do componente. Se pretende utilizar com `ngModel`, não esquecer de importar o `FormsModule` no módulo do componente.
