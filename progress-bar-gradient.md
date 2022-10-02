An Angular module to render a linear or segmented gradient progress bar on the app.

### Installing the package

```$ npm i angular-gradient-progressbar --save```

```import { AngularGradientProgressbarModule } from "angular-gradient-progressbar";
@NgModule({
  declarations: [ ... ],
  imports: [AngularGradientProgressbarModule ]
})
export class YourModule {}
```

### Add progress bar component to the app
```// segmented
<angular-gradient-progressbar [type]="1"></angular-gradient-progressbar>
// linear
<angular-gradient-progressbar [type]="2"></angular-gradient-progressbar>
```

### Customize the progress gradient bar
```// 50%
<angular-gradient-progressbar [type]="1" [value] ="50"]> </angular-gradient-progressbar>

// custom colors
<angular-gradient-progressbar [type]="1" lowTextColor="red"> </angular-gradient-progressbar>
<angular-gradient-progressbar [type]="1" mediumTextColor="orange"> </angular-gradient-progressbar>
<angular-gradient-progressbar [type]="1" highTextColor="green"> </angular-gradient-progressbar>

// width =5
<angular-gradient-progressbar [type]="1" [progressBarWidth]="5"]> </angular-gradient-progressbar>

// number of bars
<angular-gradient-progressbar [type]="1" [barCount] ="5"]> </angular-gradient-progressbar>

// shows tooltip
<angular-gradient-progressbar [type]="1" [quartileValueLow]="4" [quartileValueHigh]="7"]> </angular-gradient-progressbar>

// second value
<angular-gradient-progressbar [type]="2" [secondValue]="75"]> </angular-gradient-progressbar>```
