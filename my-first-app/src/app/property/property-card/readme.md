## how to create a component angular.js

#### first create folder structure in `src/app`
`mkdir property/property-card`

#### and go into that folder
`cd property/property-card`

#### create file called  `property-card.component.ts`
`touch property-card.component.ts`

#### add this details to the `property-card.component.ts`
```
import {Component} from "@angular/core";

@Component({
  selector: 'app-property-card',
  template: '<h1>I am a Card</h1>'
})
export class PropertyCardComponent{

}
```

#### add this component to the `src/app/app.component.html`
```
<app-property-card></app-property-card>
```

#### add the component to module in this `src/app/app.module.ts`
```
import {PropertyCardComponent} from './property/property-card/property-card.component.ts'

@NgComponent({
  declarations:[
    PropertyCardComponent
  ],
})

```
