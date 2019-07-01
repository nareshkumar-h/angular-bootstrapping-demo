# Bootstrap Angular Project

#### Angular Default Module/Component
* app.module.ts
* app.component.(html/ts)

#### Bootstrapping App Module
* main.ts
```
import { enableProdMode } from '@angular/core';
import { platformBrowserDynamic } from '@angular/platform-browser-dynamic';

import { AppModule } from './app/app.module';
import { environment } from './environments/environment';

if (environment.production) {
  enableProdMode();
}

platformBrowserDynamic().bootstrapModule(AppModule)
  .catch(err => console.error(err));
```

#### Run Application in DEV mode (Default)
* ng serve
* Browser Console Output:
```
Angular is running in the development mode. Call enableProdMode() to enable the production mode.
```

#### Run Application in PROD mode (Default)
* ng serve --prod
