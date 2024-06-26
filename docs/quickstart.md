# Quickstart

## Install xng-breadcrumb

```javascript
npm install xng-breadcrumb
pnpm add xng-breadcrumbs
yarn add xng-breadcrumb
```

## Standalone Components

**app.component.ts**

```javascript
import { BreadcrumbComponent, BreadcrumbItemDirective } from 'xng-breadcrumb';

@Component({
  standalone: true,
  imports: [RouterModule, BreadcrumbComponent, BreadcrumbItemDirective],
  templateUrl: './app.component.html',
  ...
})
export class AppComponent {}
```

**app.component.html**

```html
<xng-breadcrumb></xng-breadcrumb>
```

## Angular < 17, BreadcrumbModule

```javascript
import {BreadcrumbModule} from 'xng-breadcrumb';

@NgModule({
  imports: [BreadcrumbModule],
  ...
})
export class AppModule { }
```

**Add xng-breadcrumb selector anywhere in the app, Usually it is added in app.component.html**

```html
<xng-breadcrumb></xng-breadcrumb>
```

🎉🎉 That's it. You should see auto-generated breadcrumbs appearing for each route.
